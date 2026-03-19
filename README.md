## Experimental Design and Goals

This repository contains the code to re-analyze single cell RNAseq data previously published here: `Yao, H. et al. Timing and cell specificity of senescence drives postnatal lung development and injury. Nat. Commun. 14, 273 (2023)` 
and here: `Scaffa, A. et al. Single-cell transcriptomics reveals lasting changes in the lung cellular landscape into adulthood after neonatal hyperoxic exposure. Redox Biol. 48, 102091 (2021)`

## Folders

 * **metadata:** Contains Dockerfile to recreate environment for running the notebook.
 * **notebooks:** Contains Analysis.Rmd notebook to reanalyze data and regenerate figures and tables.
 * **data:** Contains intermediate figures and tables for publication.

## How to reproduce

The Dockerfile can be re-built or pulled from Dockerhub at `jwalla12/dennery_scrna_reanalysis:20260319-4`. The `all_data.combined` R object is on Zenodo at https://zenodo.org/records/19118171

```
title:
tags:
analysts:
git_repo_url:
resources_used:
summary:
project_id:
```
