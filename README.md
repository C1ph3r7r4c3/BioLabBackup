Hey folks,

this bio lab environment contains several programs for different purposes in the field 
of lifesciences - but be aware this is optimized for the use of monocle3 - it is an older prog and 
if new packages get installed in R within micromamba it is more often that it wants to update existent
packages, there you have to choose n or 3 for none or the R environment for using monocle3 will break,
caused by dependency issues between old and new.

I did seperate the lab environment from the deb system to avoid complications between updates and lib's.
You have to install micromamba and create an environment (env) where you can use the .yaml for and 
everything will be installed. Also you have to make an ~/.R/Makevars file with ~/.Rprofile to get the old progs
within the environment used by R working. The files are also in the repository.

It is a work in progress where several usable and good to get known progs will follow soonly.
The setup is made in Debian cause of its longterm stability, some progs I will mark with * are not installable
within micromamba, cause they are not existent in bioconda or conda-forge.
 
🧬 Categories - Overvies of the BioLabEnvironment

🧬 1) Quality Control (QC)

    fastp — QC + Trimming

    fastqc — QC Reports

    multiqc — QC Aggregation

    trimmomatic — Read Trimming

🧬 2) Read Alignment / Mapping

    bwa — Short‑read alignment

    bwa‑mem2 — Optimized BWA

    bowtie2 — Short‑read alignment

    hisat2 — RNA‑seq alignment

    minimap2 — Long‑read alignment

    subread — RNA‑seq alignment (featureCounts)

🧬 3) Variant Calling

    bcftools — VCF processing

    freebayes — Variant caller

    lofreq — Low‑frequency variant caller

    vcflib — VCF utilities

🧬 4) Metagenomics

    kraken2 — Taxonomic classification

    bracken — Abundance estimation

    centrifuge — Metagenomic classification

🧬 5) Transcriptomics / RNA‑seq

    kallisto — Pseudoalignment quantification

    salmon — Quantification

    scanpy — scRNA‑seq analysis (Python)

    anndata — scRNA‑seq data structure

    ivar — Amplicon trimming (viral)

🧬 6) Assembly

    spades — Genome assembly

    velvet — Short‑read assembly

    flye — Long‑read assembly

🧬 7) Phylogeny / Evolution

    fasttree — Phylogenetic trees

    muscle — Multiple sequence alignment

    clustalo — Multiple sequence alignment

🧬 8) Sequence Utilities / General Bioinformatics

    bedtools — Genomic interval operations

    samtools — BAM/CRAM tools

    pybedtools — Python interface to bedtools

    pyfaidx — FASTA indexing

    pyfastx — FASTA/FASTQ parsing

    pysam — Python SAM/BAM/VCF API

    edlib — Edit distance

    emboss — Classic sequence analysis suite

    blast — Sequence similarity search

🧬 9) Workflow Engines

    nextflow — Workflow orchestration

    snakemake — Workflow management

🧬 10) Python Scientific Stack

    python

    numpy

    pandas

    scipy

    scikit‑learn

    seaborn

    matplotlib‑base

🧬 11) R Bioinformatics & Statistics

    r-base

    r-ape — Phylogeny

    r-phangorn — Phylogenetics

    r-vegan — Ecology

    r-leidenbase — Clustering

    r-sf — Spatial data

    r-stars — Raster data

    r-terra — GIS

    r-xgboost — ML

    r-ranger — Random Forest

    r-tidyverse — Data science

    r-tidymodels — ML

    r-caret — ML

    r-data.table

    r-devtools

    r-rmarkdown

    r-knitr

    r-ggrastr

    r-plotly

🧬 12) GIS / Geospatial

    gdal

    geos

    proj

    udunits2

    r-sf

    r-stars

    r-terra

🧬 13) Visualization / Graphics

    matplotlib-base

    seaborn

    pymol-open-source

    r-plotly

    r-ggrastr

🧬 14) Jupyter / Notebook

    ipykernel

    jupyterlab

🧬 15) System / Utility

    sqlite

    pip

    libxml2

    libiconv

    expat

    cairo
