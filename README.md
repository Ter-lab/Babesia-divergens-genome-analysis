README

Overview

This repository contains scripts for high-throughput sequencing analysis and read quality assessment tailored for genomic research projects such as the UK_Bdiv23B and 24B studies. These scripts facilitate comprehensive read alignment, assembly, and quality control processes.

Scripts

1. Sequencing Analysis Pipeline

Description: A script designed for sequencing read alignment and processing, including reference genome indexing and extraction of unmapped reads.

Key Tools:

Bowtie2: Short read aligner.

Samtools: Manipulates SAM/BAM files.

SPAdes: De novo assembler.

SeqKit: Processes FASTA/Q files.

spray-and-pray.py: Sequence identification tool.

QUAST: Assesses genome assembly quality.

Main Features:

Command guide for alignment and extraction.

Downloading and indexing reference genomes.

Clear output structure.

2. Read Quality Assessment Script

Description: A bash script for performing quality control of paired-end reads using FastQC and generating summary reports with MultiQC.

Key Tools:

FastQC: Quality control for sequencing reads.

MultiQC: Combines FastQC results into a single report.

Main Features:

Automated processing of all FASTQ files in a directory.

Creation of output folders for organized analysis.

Comprehensive summary report generation.

Usage

Running the Scripts

Apart from the quality assessment bash script, the rest of commands used in this analysis were run as individual scripts, though you could prepare your bash script if you can.

Rename the fastqc_multiqc scripts with a .sh extension. Note that the use of bash script is only applicable to the quality assessment file using FastQC and MultiQC.

Make the scripts executable using chmod +x filename.sh.

Run the scripts:

Follow the provided comments for path definitions and tool installations.

Execute the scripts and individual commands in the appropriate directories.

Output

Sequencing analysis: Alignment files, assembly results, quality reports.

Quality assessment: Individual FastQC reports and an aggregated MultiQC report.

Prerequisites

Ensure that all required tools (e.g., Bowtie2, Samtools, SPAdes, FastQC, MultiQC) are installed and accessible via the command line.
