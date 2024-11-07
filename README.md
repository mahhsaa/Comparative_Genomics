# *Comparative_Genomics*: Detection of Duplicated Genes and Tandemly Arrayed Genes (TAGs)
This repository contains a project for detecting duplicated genes and identifying Tandemly Arrayed Genes (TAGs) in the Vigna radiata (mung bean) genome. The analysis is based on the protein sequences in the Vigna_radiata.Vradiata_ver6.pep.all.fa file. This project is part of a university research initiative aimed at exploring gene duplication patterns in plants, particularly focusing on tandemly arrayed genes, which play essential roles in gene expression and adaptation.
## Project Goals
1. **Identify Duplicated Genes**: Detect duplicated genes within the Vigna radiata genome.
2. **Detect Tandemly Arrayed Genes (TAGs)**: TAGs are genes positioned consecutively on a chromosome, often with similar sequences and functions. These genes can be significant in certain plant tissues and environmental conditions, where high gene expression levels or specific gene functions are needed.
## Methodology
The project workflow involves the following steps:
1. **Prepare the Input File**: Start with a protein FASTA file, Vigna_radiata.Vradiata_ver6.pep.all.fa contains all Vigna radiata protein sequences.
2. **Run BLAST**: Perform a BLAST search to identify homologous proteins. This helps in finding candidate duplicated genes and TAGs.

- Use BLASTP (protein-protein BLAST) to compare each protein sequence against others in the dataset.
- Save the results to a blast.txt file.
3. **Extract Gene Information**:

- For each BLAST result, extract the gene accession numbers for both the protein query and protein subject.
- Add these details to the blast.txt file for further analysis.
4.**Calculate Protein Lengths**:

- Compute the length of each protein sequence for both query and subject genes.
- Append this information to the blast.txt file to facilitate identification of similar-length genes, which is often a characteristic of tandem duplicates.

## File Structure

## About Tandemly Arrayed Genes (TAGs)
Tandemly Arrayed Genes" (TAGs) are clusters of genes located sequentially on a chromosome, often with high sequence similarity and similar functions. These genes are frequently observed in plants and animals, where multiple copies of the same gene may be required in specific tissues or environmental conditions. TAGs contribute to gene expression versatility and provide evolutionary advantages by allowing organisms to rapidly adapt to their environment.

## Usage
