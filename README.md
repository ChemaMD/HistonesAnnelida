# The evolution and developmental dynamics of histone-based chromatin regulation in Annelida - Supplementary Data
This GitHub repository contains the supplementary data and the custom code used in the publication cited below.

## How to use and cite these files and code
All files and code are made publicly available and can be used for further research and other applications. However, if you use these resources in your work, we kindly ask you to cite our original publication.
> **The evolution and developmental dynamics of histone-based chromatin regulation in Annelida.**
> Francisco M. Martín-Zamora, Joby Cole, Rory D. Donnellan, Kero Guynes, Allan M. Carrillo-Baltodano, Mark Dickman, Paul J. Hurd, José M. Martín-Durán.
> Manuscript in preparation.

## Author contact
- [José M. Martín-Durán](mailto:chema.martin@qmul.ac.uk) (senior author, corresponding author)
- [Francisco M. Martín-Zamora](mailto:fmartinzamora@altoslabs.com) (first author, corresponding author)
- Lab website: [martinduranlab.com](https://www.martinduranlab.com)

## How to download data files
The files inside this repository are all compressed `.tar.gz` files stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) which will need to be decompressed. To view them, select the `.tar.gz` file you are interested in (e.g. [05-Evolutionary_analysis_H2AX_variants.tar.gz](05-Evolutionary_analysis_H2AX_variants.tar.gz)), click on *Download* and the file will be downloaded to your device.

> :warning: **Some files are very heavy and download might take time to begin:** :warning: Be patient, they are correctly stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) and your download will eventually start.

## How to download code files
The code in this repository is all stored in the [00-Code](00-Code) folder, and can be downloaded as described above. Most scripts were built in R or Python and are therefore in `.R`, `.py` or `.ipynb` format, which can be visualised in your IDE of choice (e.g., RStudio, Visual Studio Code, etc.). Some of them, specially those that combine multiple steps across different programming languages or softwares called in the command line terminal, were put together in `.txt` or `.docx` files, from which the different code chunks can be copied.

> We believe that the script file names and the comments in the scripts make them self-explanatory, but please do not hesitate to reach out if you have any doubts or questions.

## Index of data files contents
[01-Updated_genomes.tar.gz](01-Updated_genomes.tar.gz) contains all the relevant genome annotation files and gene models for the three different species after our manual histone gene mining. For each species:
- **<Species_name>_genome_annotation_report_v1_deleted_entries.xlsx** contains a report detailing the list of gene models that were removed from the original genome annotation files and are now replaced by manually curated histone genes.
- **<Species_name>_genome_annotation_v2.gff3** contains the `.gff3` file with the full genome annotation, including the manually curated histone genes.
- **<Species_name>_genome_annotation_mRNA_v2.fa**, **<Species_name>_genome_annotation_CDS_v2.fa** and **<Species_name>_genome_annotation_proteins_v2.fa** contain the sequences in `.fasta`/`.fa` format of the transcripts/mRNAs, the coding sequences (CDS) of said transcripts, and the protein sequences, respectively, of the gene models contained in the `.gff3` file.
- **<Species_name>_genome_annotation_mRNA_report_v2.xlsx** contains the report with the full list of gene models after including the manually curated histone genes. This matches the genome annotation from the `.gff3` file and contains many relevant annotations, such as GO terms, PFAM domains, best BLAST hits, PANTHER hits, mRNA and protein sequence, etc.


[02-Histone_genes_mining.tar.gz](02-Histone_genes_mining.tar.gz) contains the core histones gene models in `.gff3` format and the histone mRNA and protein sequences files in `.fasta`/`.fa` format for *O. fusiformis*, *C. teleta*, and *D. gyrociliatus*. For both *O. fusiformis* and *C. teleta* there are two different gene model files, which match each of the genome assemblies: one at scaffold level, and another one at chromosome level. For each species:
- **<Species_name>core_histones_annotation.gff3** contains the gene models of the core histone genes.
- **<Species_name>_mRNA.fa** contains the mRNA/transcript sequences of the core histone genes.
- **<Species_name>_protein.fa** contains the protein sequences of the core histone genes.


[03-Histone_genes_orthology_assignment.tar.gz](03-Histone_genes_orthology_assignment.tar.gz) contains the multiple sequence alignment files in `.fasta`/`.fa` and `.pdf` formats (and `.nexus`, where applicable) we used to assign the orthology of the core histone genes, as well as a report on the amino acid changes observed in the core histone genes (and pseudogenes).
- **Core_histones_alignment.fa** and **Core_histones_alignment.nexus** contain the multiple sequence alignments associated to the maximum likelihood and Bayesian phylogenetic analyses we used to assign the orthology of core histone genes.
- **Core_histones_alignment.pdf** is a graphic visualisation of the files described above.
- **Histone_sequence_differences.docx** and **Histone_sequence_differences.pdf** are reports containing the amino acid differences and their potential impact on hPTM presence between eukaryotic model organisms and annelid histone genes, both canonical and variant, and the identified pseudogenic sequences.


Then, for each core histone family, that is, H2A, H2B, H3, and H4:
- **<Histone_family>_family_alignment.fa** contains the multiple sequence alignments used to investigate amino acid changes in each histone gene (and pseudogene).
- **<Histone_family>_family_alignment.pdf** is a graphic visualisation of the file described above.


[04-Gene_expression_profiling.tar.gz](04-Gene_expression_profiling.tar.gz) contains the gene expression matrices in `.txt` format in transcripts-per-million (TPM) and after DESeq2 normalisation of the developmental RNA-seq time courses of *O. fusiformis*, *C. teleta*, and *D. gyrociliatus*. These contain all transcripts (i.e., all isoforms per gene model), both split by biological replicates and averaged by developmental stage, after the re-profiling with the updated gene models containing the curated core histone genes. For each species:
- **RNAseq_<Species_name>_TPM_replicates.txt** is the gene expression matrix of all transcripts in TPM split by replicates.
- **RNAseq_<Species_name>_TPM_average.txt** is the gene expression matrix of all transcripts in TPM averaged by developmental stage.
- **RNAseq_<Species_name>_DESeq2_replicates.txt** is the gene expression matrix of all transcripts in DESeq2 normalised values split by replicates.
- **RNAseq_<Species_name>_DESeq2_average.txt** is the gene expression matrix of all transcripts in DESeq2 normalised values averaged by developmental stage.


All files contain a suffix of the form **_vDDMMYY** that stands for version and the date in which the re-profiling took place.


[05-Evolutionary_analysis_H2AX_variants.tar.gz](05-Evolutionary_analysis_H2AX_variants.tar.gz) contains the multiple sequence alignment files in `.fasta`/`.fa` and Clustal `.aln` formats (and `.pdf`, where applicable) we used during the evolutionary analyses of H2A.X variants across Eukarya.
- **H2A.X_selected_species_alignment.fa** and **H2A.X_selected_speices_alignment.nexus** contain the multiple sequence alignments shown to highlight the variability of the position 142 in H2A.X proteins.
- **H2A.X_selected_species_alignment.pdf** is a graphic visualisation of the files described above.
- **H2A.X_PHI-BLAST_Eukarya_alignment.fa** and **H2A.X_PHI-BLAST_Eukarya_alignment.aln** contain the multiple sequence alignments associated to the maximum likelihood analyses we used to understand the evolution of the C-terminus of H2A.X variants.


Then, for each eukaryotic clade, namely Chordata, Spiralia, Arthropoda, Streptophyta, and Eukarya(_curated):
- **H2A.X_terminal_motif_alignment_<clade>.fa** and **H2A.X_terminal_motif_alignment_<clade>.aln** contain the alignments corresponding to the C-termini of selected eukaryotic H2A.X sequences that were used to generate the C-terminal motif logos.


[06-Histone_modifier_genes_orthology_assignment.tar.gz](06-Histone_modifier_genes_orthology_assignment.tar.gz) contains the multiple sequence alignment files in `.fasta`/`.fa` and Clustal `.aln` formats, as well as in `.pdf`, that we used to assign the orthology of the histone-modifying enzymes genes. For each of the six superfamily alignments, i.e., HDAC, HDM, HAT_typeA, HAT_typeB, KMT, and PRMT:
- **<Superfamily>_superfamily_alignment.fa** and **<Superfamily>_superfamily_alignment.nexus** contain the multiple sequence alignments associated to the maximum likelihood and Bayesian phylogenetic analyses we used to assign the orthology of the histone-modifying enzymes genes.
- **<Superfamily>_superfamily_alignment.pdf** is a graphic visualisation of the files described above.

[07-PRMT6_sequence_architecture_analysis.tar.gz](07-PRMT6_sequence_architecture_analysis.tar.gz) contains the multiple sequence alignment in `.fasta`/`.fa` and Clustal `.aln` format, as well as in `.pdf`, which we used to analyse the sequence conservation of the annelid PRMT6 orthologs.
- **PRMT6_alignment.fa** and **PRMT6_alignment.nexus** contain the multiple sequence alignments shown to highlight the variability of the substrate and cofactor-binding residues, as well as the critical regions of the enzyme, in the annelid PRMT6 orthologs.
- **PRMT6_alignment.pdf** is a graphic visualisation of the files described above.

[08-AlphaFold_Server_predictions.tar.gz](08-AlphaFold_Server_predictions.tar.gz) contains the folders with the output files from the structural predictions of the [AlphaFold3 server](https://alphafoldserver.com) for the annelid H2A.X and PRMT6 proteins. See their website for more info about the AlphaFold outputs.