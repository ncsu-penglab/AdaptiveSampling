# Nanopore Adaptive Sampling Procedures:
To view the protocols listed below, you will need to sign up for an [Oxford Nanopore Account](https://nanoporetech.com/login-register). 
Once an account has been registered, protocols are available through the Oxford Nanopore Community dashboard.

## Contents
- [Sample Preparation](#Sample-Preparation)
- [Library Preparation & Sequencing](#Library-Preparation-&-Sequencing)
- [Sequencing Run Parameters](#Sequencing-Run-Parameters)

## Sample Preparation:
 **1. Extract the sample** <br>
   gDNA samples from a human cell line were extracted following the QIAGEN Puregene Cell Kit protocol recommended by the Human cell line gDNA protocol found under Documentation / Prepare / Extraction Protocols.
   Assess the gDNA input following the Assessing input DNA protocol found under Documentation / Prepare / DNA/RNA Handling / Input DNA/RNA QC.
   We utilized Nanodrop spectrophotometry, Qubit, and pulse-field gel electrophoresis to assess gDNA. <br>
 **2. Check the flow cell** <br>
   Use the Flow Cell Check protocol under Documentation / Sequence / Device Installation & Configuration protocols prior to library preparation.

## Library Preparation & Sequencing:
 **1. Prepare a library for sequencing** <br>
   Follow Genomic DNA by Ligation (SQK-LSK110) protocol found under Documentation / Prepare / Library Prep Protocols. This has since been renamed to Ligation Sequencing gDNA (SQK-LSK110) but will move to legacy in March 2024. <br>
**2. Washing the flow cell** <br>
   After sequencing or before loading another library, the flow cell will need to be washed. This was completed using the Flow Cell Wash Kit (EXP-WSH004) protocol found under Documentation / Prepare / Library Prep Protocols.

## Sequencing Run Parameters:
   **Input data:** One gDNA library, no new library reloading and flow cell wash,
                reference genome fasta file, target regions fasta file
   Parameter | Value 
   ---- | ----
   Run time | 24 hours
   Basecalling | Fast model
   Minimum read length | 1kb
   Basecalling quality score | 8
   Output files | minimap2 SAM file, fastq.gz, fast5 file
