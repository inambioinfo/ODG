# ODG: Omics Database Generator

## Introduction

Welcome. This project is in near-publication stage. Please follow this project for announcements or e-mail me (guhli007 at umn.edu) and ask to be mailed when the initial release is out.

## What this does

This program takes genome files and output from various programs to create a graph database for querying genomic data across domains. This program is stable and database structure is well defined.

Feel free to ask questions or make suggestions.

## Usage

Download and run appropriate programs to create the output. Please see run-new.sh to see what types of files are necessary.

### All Platforms
Download and extract one of the available releases.

Place files for each of your genomes in the data/ directory, one directory for each genome and genome version, or accession (strain). For Example:

    data/
         Arabidopsis_thaliana_10/
             assembly.fasta
             genes.gff3
             proteins.fasta
             ipscan_results.tsv
         Oryza_sativa_2/
             assembly.fasta
             genes.gff3
             proteins.fasta
             ipscan_results.tsv
         E_coli_1/
             assembly.fasta
             genes.gff3
             proteins.fasta
             ipscan_results.tsv

         
### For Windows
To begin the configuration program double click "odg-config.bat" and set your browser to http://localhost:33333 after the server has started, usually a few minutes after starting.
To compile the database, once all intervening software has been run you can run "odg-generate.bat" and wait, usually a half hour to a few hours depending on the size of your dataset.
To run the query server, run "odg-query.bat" and point your web browser to http://localhost:6789

### For *nix Systems
To begin the configuration program run "./odg-config.sh" and set your browser to http://localhost:33333 after the server has started, usually a few minutes after starting.
To compile the database, once all intervening software has been run you can run "./odg-generate.sh" and wait, usually a half hour to a few hours depending on the size of your dataset.
To run the query server, run "./odg-query.sh" and point your web browser to http://localhost:6789

## For More Information
Please see the user guide, available [[here]]

## License

Copyright � 2017 Joseph Guhlin
