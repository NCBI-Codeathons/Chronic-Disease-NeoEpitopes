# Chronic-Disease-NeoEpitopes
General information flow
![Flowchart](Slide1.jpg)
Detailed information to make the final table
![Flowchart2](Slide2.jpg)

# Instructions for Use:
NEO antigens
![Flowchart3](neo_spoon.jpeg)
There is no spoon

# Introduction:
There’s just so much data coming out of next-gen sequencing platforms that no human could possibly parse it all on their own. The raw data to discover new insights of the disease states is there but not in an actionable format. Filtering and selection of the most relevant aspects of the genomic data will allow the user to narrow down exactly what they want to test in clinical research experiments. 

What are the relevant aspects we need to collect for this queryable database? We need to gather information for a disease of interest: 1) NCBI Bioproject can give us SRA datasets that yield certain SRA-IDs, 2) using those SRA-IDs we can probe GWAS Catalog data for the SNPs that were found in that RNAseq experiment, 3) then using updated forms of SC3 and PSST to probe MAGIC-BLAST to correlate the SNP IDs with the expression levels, 4) combining these data into one table sorted on the disease of interest, will yield an incredibly useful database that can be searched not only by disease, but by expression levels or SNPs of interest as well. This new tool will allow the user to add new disease related data as needed so the database can be expanded as new experiments are performed, making it a renewable resource of correlation data that gets better and better as it is filled with more contributions. There is also the possibility of adding more protein data to the table, such as whether the protein has been crystallized or otherwise structurally modeled, what sort of post-translational modifications it harbors, and localization of the protein to specific organelles in disease versus healthy states. 

For the average researcher, they could query the database based on their disease of choice, and pull out a list of the SNPs present in the disease state, as well as a ranking of how highly expressed each one is. But what if this same researcher has an unknown condition and only knows of SNPs that are consistently identified in infected patients. They can search by that too, and pull out what diseases are also associated with these SNPs and possibly make a more informed diagnosis. Further characterization of the disease state in this manner will help to create protein/SNP-translation profiles for disorders that currently plague humanity, and lead up towards new treatments that would not have been possible without this wide of a scope of information readily available.

# Methods:
For the creation of this database, we first selected diseases that are known autoimmune disorders such as Rheumatoid Arthritis, Type I Diabetes, and Asthma. Then we searched NCBI Bioproject for RNAseq datasets and collected the SRA-IDs using (updated) SC3. From here we took those SRA-IDs and searched the GWAS Catalog for SNPs related to the disease. Then using an updated PSST, which runs MAGIC-BLAST, we connected the SNPs to their expression levels in the associated disease experiments. From here the SNPs can be converted to protein sequences using Ensembl. Combining these data in the following order: Disease, Tissue, Gene, SNP, Protein, Expression Levels, into a dataframe object and then to a SQL database; allows us to build an exceptionally useful database that can be queried by any researcher with ease. 

# Results:
put the things here

# Discussion:
SAVE THE WORLD A LOT

