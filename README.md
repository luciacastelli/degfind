# degfind: An R Package for Introductory Differential Expression Analysis  

As part of my thesis and final project for **CS50’s Introduction to Programming with R (CS50R)**, I developed this R package called **degfind** for transcriptomic analysis of microarray and RNA-seq expression data.  

The package was designed to establish the automation of elementary processes within transcriptomic research workflows, supporting laboratory collaborators with limited programming experience with structured, documented, and reproducible tools for basic differential expression analysis.


## Demonstration  

A video demonstration showing the usage of each function is available on [my YouTube](https://youtu.be/7Vcm609bAac?si=cBIhvW-Qagzl2FEQ).

## Installation and Structure  

The package is compatible with the `devtools::build()` command from the R command line, specifying the path to the project files hosted on GitHub.  

The repository includes:

- A sample `.csv` test dataset located at `testthat/degtable.csv`  
- Function manuals  
- Unit tests  
- License information  
- Documentation in `.Rd` format (standard R documentation format)  

The function documentation can be accessed either through the `degfind/man/` directory or directly in RStudio using the `?function_name` command.

## Implemented Functions  

The package contains eight core functions:

1. **DEG_table**  
   Generates a table of differentially expressed genes.

2. **DEGs**  
   Processes expression data to extract names of differentially expressed genes and generates a Venn diagram distinguishing upregulated and downregulated genes.

3. **gene_names**  
   Processes expression data to extract gene names.

4. **make_lm**  
   Processes expression data to generate a linear model and return results, including Bayesian statistics.

5. **make_toptable**  
   Processes Bayesian statistics from a linear model to generate a data frame similar to the main output tables of the *limma* package, including classification of low- and high-expression genes.

6. **plot_data_quality**  
   Processes expression data to generate and save a violin plot describing data quality.

7. **sample_names**  
   Processes expression data to extract sample names.

8. **volcano**  
   Saves a volcano plot of differential expression results, where the x-axis represents log fold change (logFC) and the y-axis represents the adjusted p-value.

---

**Note:** The package is intended for introductory and educational purposes, as well as for small-scale laboratory workflows. It does not aim to replace advanced or fully customized bioinformatics pipelines.
