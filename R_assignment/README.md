# BCB546_R_Hwk_Chatt
The files are:

1. `fang_et_al_genotypes.txt`: a published SNP data set including maize, teosinte (i.e., wild maize), and Tripsacum (a close outgroup to the genus _Zea_) individuals


 
2. `snp_position.txt`: an additional data file that includes the SNP id (first column), chromosome location (third column), nucleotide location (fourth column) and other information for the SNPs genotyped in the `fang_et_al_genotypes.txt` file

## Part I Data Processing

All files are formatted such that the first column is "SNP_ID", the second column is "Chromosome", the third column is "Position", and subsequent columns are genotype data from either maize or teosinte individuals.

For maize (Group = ZMMIL, ZMMLR, and ZMMMR in the third column of the `fang_et_al_genotypes.txt` file) we want 20 files in total:

* 10 files (1 for each chromosome) with SNPs ordered based on increasing position values and with missing data encoded by this symbol: ?
	Found in the directory "maize_snp_by_chr"

* 10 files (1 for each chromosome) with SNPs ordered based on decreasing position values and with missing data encoded by this symbol: -  
	Found in the directory "maize_snp_by_chr"

For teosinte (Group = ZMPBA, ZMPIL, and ZMPJA in the third column of the `fang_et_al_genotypes.txt` file) we want 20 files in total:

* 10 files (1 for each chromosome) with SNPs ordered based on increasing position values and with missing data encoded by this symbol: ?  
	Found in the directory "teosinte_snp_by_chr"

* 10 files (1 for each chromosome) with SNPs ordered based on decreasing position values and with missing data encoded by this symbol: -  
	Found in the directory "teosinte_snp_by_chr"

## Part II

### _SNPs per chromosome_
Plot the total number of SNPs in our dataset on each chromosome. What groups contribute most of these SNPs?

### _Missing data and amount of heterozygosity_
Create a new column to indicate whether a particular site is homozygous (has the same nucleotide on both chromosomes (i.e., A/A, C/C, G/G, T/T) or heterozygous (otherwise)).  Recode the missing data as NA. Sort your dataframe using Group and Species_ID values. Make a graph that shows the proportion of homozygous and heterozygous sites as well as missing data in each species (you won't be able to see species names) and each group.  For groups normalize the height of individual bars using one of the ggplot "position adjustments" options.

### _Your own visualization_
Visualize one other feature of the dataset. The choice is up to you!

