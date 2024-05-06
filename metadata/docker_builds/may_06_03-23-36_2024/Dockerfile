FROM ghcr.io/compbiocore/dennery_singlecell_reanalysis:may_06_01-57-18_2024
#RUN R -e 'install.packages(c("broom", "corrplot", "car", "cowplot", "MASS", "fitdistrplus", "future", "future.apply", "ggrepel", "ggridges", "hdf5r", "httr", "ica", "igraph", "irlba", "jsonlite", "leiden", "lmtest", "matrixStats", "miniUI", "patchwork", "pbapply", "plotly", "png", "RANN", "Rcpp", "RcppAnnoy", "reticulate", "ROCR", "rsvd", "Rtsne", "sctransform", "shiny", "spatstat", "tidyverse", "uwot", "RcppEigen", "RcppProgress", "RColorBrewer", "viridis", "spatstat", "rstatix"), dependencies=TRUE, repos="http://cran.rstudio.com/", ask = FALSE)' \
RUN R -e 'BiocManager::install(c( "minfi", "BiocGenerics", "DelayedArray", "DelayedMatrixStats", "limma", "S4Vectors", "SingleCellExperiment", "SummarizedExperiment", "batchelor", "AnnotationHub", "biomaRt", "clusterProfiler", "enrichplot", "batchelor", "Biobase", "limma", "rhdf5filters", "XVector", "GenomeInfoDb", "sparseMatrixStats", "BiocNeighbors", "DelayedArray", "rhdf5", "DOSE", "beachmat", "GenomicRanges", "ResidualMatrix", "HDF5Array", "BiocSingular", "scuttle"),  update = FALSE, ask = FALSE)' \

#RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/spatstat/spatstat_1.64-1.tar.gz"", repos=NULL,type="source")' \
#RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/Seurat/Seurat_3.2.1.tar.gz", repos = NULL, type = "source")' \
#RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/rstatix/rstatix_0.6.0.tar.gz", repos = NULL, type = "source")' \
#RUN R -e 'install.packages("https://cran.r-project.org/src/contrib/Archive/sctransform/sctransform_0.2.1.tar.gz", repos = NULL, type = "source")' \

#RUN R -e 'devtools::install_github("cole-trapnell-lab/leidenbase")' \
#RUN R -e 'devtools::install_github("cole-trapnell-lab/monocle3")' 
