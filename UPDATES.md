# Updates

A chronological log of your updates and work on the projects should go here.

## March 2026

### Dockerfile base image update (fix multi-arch build errors)

**Problem:** Building with `docker buildx build --platform linux/amd64,linux/arm64` against the previous base image (`ghcr.io/compbiocore/ccv_bootcamp_scrna:may_13_11-46-27_2024`) produced three errors:

1. `pak` failed to build `hdf5r 1.3.9` with _"staged installation is only possible with locking"_ – Docker's overlay filesystem does not support the POSIX file locks that `pak`'s staged-install mode requires.
2. R library I/O error (`cannot open .../tools/Meta/nsInfo.rds`) – overlay filesystem corruption during the QEMU-emulated arm64 build.
3. Docker buildkit overlay I/O error (`write .../metadata_v2.db: input/output error`) – disk/filesystem pressure from building two platforms simultaneously under QEMU emulation.

**Fix:**
- Replaced the 2024 base image with `rocker/rstudio:4.4.2`, which ships native manifests for both `linux/amd64` and `linux/arm64`, eliminating QEMU emulation and the associated overlay filesystem issues.
- Added `ENV R_INSTALL_STAGED=false` so that `pak` (and `install.packages`) skip staged installation entirely, resolving the locking error.
- Restored the full package installation chain (system libraries, CRAN packages, Bioconductor packages, archived pinned versions, and GitHub-hosted packages) directly in the Dockerfile so the image is self-contained.
