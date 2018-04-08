# Venn-Diagram
Script for R. An automated way of plotting venn diagram (upto 8 sets) from a list of genes in xlsx format

R-script for making un-weighted venn diagrams form upto 8 sets of gene lists.
The gene list should be in .xlsx format with each condition occupying only one column. Duplicate entries in each sets will be ignored.Do not keep any headers mentioning the set name. the file should not contain anything other than the gene list.
This script Requires Perl and packages: gdata, vennerable and gplots.

To install "vennerable" run the following commands:
   source("https://bioconductor.org/biocLite.R"); biocLite(c("RBGL","graph"))
   
   install.packages("devtools"); library(devtools);
   
   install_github("js229/Vennerable")
   
Other packages can be installed from cran.

The Excel file should be in the working directory. The resultant txt file containing the list of common genes and uniques genes from each set will be saved in the working directory.
