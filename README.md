# Project name: Directory Template

## Description

A short sentence describing the project. For example, this repository serves as a template for the directory structure of future projects.

### Goal

A paragraph discussing the goal and results of the project. For example, in order to increase the computational reproducibility of my projects, I have created this template repository for future projects. I believe that creating a directory structure that is adaptable and scales up well is important to creating reproducible code, and hope this will be useful. I find this structure useful because it has space for both simple R scripts (load, analyze, and visualize data) and it has a simple mechanism to source those R scripts for sharing with collaborators in a bookdown format. Specifically, the R scripts live within the `src` directory and can be separated into directories for discrete analyses. Each script will be numbered in the order in which they are intended to be sourced. Finally, the `docs` directory contains a simple file (`index.Rmd`) that can be `knit`ed to a bookdown format by sequentially sourcing each R script within a code chunk. Analyses that take a non-trivial amount of time do not need to be evaluated during the `knit` process. Simply include the chunk option `eval = FALSE`. The code from the script will be printed into the document, but not executed. Finally once the document is `knit`, GitHub Pages will build the a share-able bookdown report from the files within the `doc` directory and the book will be available at `username.github.io/repo_name` (_e.g._ [https://tsoleary.github.io/template_Rproject/](https://tsoleary.github.io/template_Rproject/]).

### Project structure

This project is organized into the following directory structure:

- `data/` - all data used in code
  - `raw/` - all raw data
  - `processed/` - all processed data
- `src/` - source code used for analyses -- files saved with numerical prefix
  - `starwars/` - source code related to starwars data
  - `iris/` - source code related to iris data
- `output/` - all output files 
  - `figs/` - all figures generated
- `docs/` - files assembled for external sharing
- `scratch/` - any temporary or extraneous files and information
  
    
