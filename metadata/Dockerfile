FROM ghcr.io/compbiocore/dennery_singlecell_reanalysis:may_06_03-23-36_2024
RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/spatstat/spatstat_1.64-1.tar.gz"", repos=NULL,type="source")' \
RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/Seurat/Seurat_3.2.1.tar.gz", repos = NULL, type = "source")' \
#RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/rstatix/rstatix_0.6.0.tar.gz", repos = NULL, type = "source")' \
RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/sctransform/sctransform_0.2.1.tar.gz", repos = NULL, type = "source")' \
