# mtDNA VLM


### Last Updated
This README was last updated on 21/03/2025


## Description

This repository provides tools for calculating mtDNA Variant Load Scores (VLS), or the sum of pathogenicitic probability for all mitochondrial DNA (mtDNA) variants present in a patient. The tool is designed to facilitate the analysis of mtDNA variations using the mitochondrial variant load model.


## Contents

1. Variant load score calculator with Gradio GUI [./VLS_calculator/]
- The Jupyter notebook loads a user-friendly interface for calculating the variant load score across all protein-encoding genes in mtDNA.
- The following files are required to run the tool:
	* Patient data:
		A FASTA or .txt file containing unaligned patient mtDNA genomes OR 
		A .txt file containing patient variants.
	* If a file is provided for patient mtDNA genomes, upload a FASTA, .txt, or .gb file containing a mtDNA reference genome.
	* A .csv file for pathogenic score lookup. Before uploading a lookup table ensure the mtDNA variant lookup table has the following four column headings: Position, Reference, Mutation, Pathogenicity_Score


2. FASTA reverse engineering from patient variant data [./converting_variants_to_fasta/]
-This script reconstructs FASTA files from patient variant information.
-The following files are required as input:
	* A .txt file containing patient variant information
	* Revised Cambridge Reference Sequence (rCRS) of the Human Mitochondrial DNA


3. Scripts to plot a correlation matrix or heatmap of patient variant loads [./plotting_scripts/]
These scripts are used to generate correlation matrices and heatmaps of patient variant loads for data interpretation.


## Acknowledgements
Project by Joanna Elson, Wasim Iqbal and Erin Chee.
