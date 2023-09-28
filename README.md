# Histone-based regulation of annelid development and life cycle heterochronies - Supplementary Data
This GitHub repository contains the supplementary data and the custom code used in the publication cited below.

## How to use and cite these files and code
All files and code are made publicly available and can be used for further research and other applications. However, if you use these resources in your work, we kindly ask you to cite our original publication.
> **Histone-based regulation of annelid development and life cycle heterochronies.**
> Francisco M. Martín-Zamora, Joby Cole, Nancy Ellis, Rory D. Donnellan, Kero Guynes, Allan M. Carrillo-Baltodano, Mark Dickman, Paul J. Hurd, José M. Martín-Durán.
> Manuscript in preparation.

## Author contact
- [José M. Martín-Durán](mailto:chema.martin@qmul.ac.uk) (senior author, corresponding author)
- [Francisco M. Martín-Zamora](mailto:f.m.martinzamora@qmul.ac.uk) (first author, corresponding author)
- Lab website: [martinduranlab.com](https://www.martinduranlab.com)

## How to download data files
The files inside this repository are all compressed `.tar.gz` files stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) which will need to be decompressed. To view them, select the `.tar.gz` file you are interested in (e.g. [05-Evolutionary_analysis_H2AX_variants.tar.gz](05-Evolutionary_analysis_H2AX_variants.tar.gz)), click on *Download* and the file will be downloaded to your device.

> :warning: **Some files are very heavy and download might take time to begin:** :warning: Be patient, they are correctly stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) and your download will eventually start.

## How to download code files
The code in this repository is all stored in the [00-Code](00-Code) folder, and can be downloaded as described above. Most scripts were built in R or Python and are therefore in `.R`, `.py` or `.ipynb` format, which can be visualised in your IDE of choice (e.g., RStudio, Visual Studio Code, etc.). Some of them, specially those that combine multiple steps across different programming languages or softwares called in the command line terminal, were put together in `.txt` or `.docx` files, from which the different code chunks can be copied.

> We believe that the script file names and the comments in the scripts make them self-explanatory, but please do not hesitate to reach out if you have any doubts or questions.

## Index of data files contents
[02-Histone_genes_mining.tar.gz](02-Histone_genes_mining.tar.gz) contains the core histones gene models in `.gff3` format and the histone mRNA and protein sequences files in `.fasta`/`.fa` format for *O. fusiformis*, *C. teleta*, and *D. gyrociliatus*. For both *O. fusiformis* and *C. teleta* there are two different gene model files, which match each of the genome assemblies: one at scaffold level, and another one at chromosome level. For each species:
- **<Species_name>core_histones_annotation.gff3** contains the gene models of the core histone genes.
- **<Species_name>_mRNA.fa** contains the mRNA/transcript sequences of the core histone genes.
- **<Species_name>_protein.fa** contains the protein sequences of the core histone genes.

[03-Histone_genes_orthology_assignment.tar.gz](03-Histone_genes_orthology_assignment.tar.gz) contains the multiple sequence alignment files in `.fasta`/`.fa` and `.pdf` formats (and `.nexus`, where applicable) we used to assign the orthology of the core histone genes, as well as a report on the amino acid changes observed in the core histone genes (and pseudogenes).
- **Core_histones_alignment.fa** and **Core_histones_alignment.nexus** contain the multiple sequence alignments associated to the maximum likelihood and Bayesian phylogenetic analyses we used to assign the orthology of core histone genes.
- **Core_histones_alignment.pdf** is a graphic visualisation of the files described above.
Then, for each core histone family, that is, H2A, H2B, H3, and H4:
- **<Histone_family>_family_alignment.fa** contains the multiple sequence alignments used to investigate amino acid changes in each histone gene (and pseudogene).
- **<Histone_family>_family_alignment.pdf** is a graphic visualisation of the file described above.
  Lastly, 
