## Extract_spike_gene

This workflow extracts spike (glycoprotein) gene portions from SARS-CoV-2 whole genome sequences.
Same principle can be applied while extracting gene sequences from longer genomes.

## Tools 
1. blast command-line tool. Download from [here](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/)
2. Python 3.9.5

## Test Data
The test dataset contains a set of SARS-CoV-2 complete genome sequences downloaded from [GISAID](https://www.gisaid.org) database.
This multi-fasta file is referred as seqfile in the subsequent steps. The query file contains a single fasta sequence - in here the 
surface glycoprotein gene sequence from SARS-CoV-2 [Wuhan strain](https://www.ncbi.nlm.nih.gov/nuccore/NC_045512.2)

## Workflow
1. Create a database of the whole genome sequences.
2. Align spike query sequence to blast database. Use mapping coordinates to extract the target gene sequences from database.

## Steps

Lauch the workflow console within LatchBio using this [link](https://console.latch.bio/explore/61979/info).
Create an account once prompted.

1. Load a single spike gene sequence as `query_sequence`
2. Load metafile containing full genome sequences as `seq_data`
3. Execute the pipeline


Link to the code [here](https://github.com/mikemwanga/wf-sars_cov_spike_gene/blob/main/wf/__init__.py)

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)