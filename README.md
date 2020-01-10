# Chronic-Disease-NeoEpitopes



NEO antigens

![Flowchart3](neo_spoon.jpeg)

There is no spoon

Paper citation/DOI here

# Introduction:


## What is the problem that needs solved?

Finding a list of SNPs present in RNAseq data is currently feasible, but the more actionable information is the proteins that are made when these SNP-containing transcripts are translated into proteins.

## How will we solve the problem?

We will solve the problem by combining and updating the already-available tools named PSST and SC3, and incorporating SNP-transcript translation using Ensembl. We will have multiple tables that when combined and converted to an SQL database, will be queryable but also able to be added to, should the researcher want to contribute to it. 

## What is <the software>?

General information flow
![Flowchart](Slide1.jpg)

## Software design diagram:

Detailed information to make the final table
![Flowchart2](Slide2.jpg)

## Entity Relationship Diagram

x

# Instructions for Use:

## Use 1: Searching the existing database for information

If you want to see the SNP/Protein profile of a certain disease, here's an example query:

`SELECT * FROM combined_table WHERE disease='Arthritis'`


## Use 2: Running your own experiment and contributing to the database

You will need: BioprojectID for your disease of interest, a list of SNPs, and the dependencies needed to run PSST.
You will run SC3.sh (which contains PSST.sh) using the BioprojectID, which will output a list of SNPs.

# Results:
x

# Discussion:
x

