# Histone-based regulation of annelid development and life cycle heterochronies - Supplementary Data
This GitHub repository contains the supplementary data and the custom code used in the publication cited below.

## How to use and cite these files and code
All files and code are made publicly available and can be used for further research and other applications. However, if you use these resources in your work, we kindly ask you to cite our original publication.
> **Histone-based regulation of annelid development and life cycle heterochronies.**
> Francisco M. Martín-Zamora§, Joby Cole, Nancy Ellis, Rory D. Donnellan, Kero Guynes, Allan M. Carrillo-Baltodano, Mark Dickman, Paul J. Hurd, José M. Martín-Durán.
> Manuscript in preparation.

## Author contact
- [José M. Martín-Durán](mailto:chema.martin@qmul.ac.uk) (senior author, corresponding author)
- [Francisco M. Martín-Zamora](mailto:f.m.martinzamora@qmul.ac.uk) (first author, corresponding author)
- Lab website: [martinduranlab.com](https://www.martinduranlab.com)

## How to download data files
The files inside this repository are all compressed `.tar.gz` files stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) which will need to be decompressed. To view them, select the `.tar.gz` file you are interested in (e.g. [05-Chordin_orthology_assignment.tar.gz](05-Chordin_orthology_assignment.tar.gz)), click on *Download* and the file will be downloaded to your device.

> :warning: **Some files are very heavy and download might take time to begin:** :warning: Be patient, they are correctly stored in [GitHub Large File Storage (LFS)](https://git-lfs.github.com/) and your download will eventually start.

## How to download code files
The code in this repository is all stored in the [00-Code](00-Code) folder, and can be downloaded as described above. Most scripts were built in R or Python and are therefore in `.R`, `.py` or `.ipynb` format, which can be visualised in your IDE of choice (e.g., RStudio, Visual Studio Code, etc.). Some of them, specially those that combine multiple steps across different programming languages or softwares called in the command line terminal, were put together in `.txt` or `.docx` files, from which the different code chunks can be copied.

> We believe that the script file names and the comments in the scripts make them self-explanatory, but please do not hesitate to reach out if you have any doubts or questions.

## Index of data files contents
- [01-Owenia_fusiformis_genome_assemblies.tar.gz](01-Owenia_fusiformis_genome_assemblies.tar.gz) contains the unmasked genome files in `.fasta`/`.fa` format of the two genome assemblies versions we report in the publication:
  - **Scaffold_level_assembly_unmasked.fa**, which is the first high-quality genome assembly that we created, upon which we have based our RNA-seq and ATAC-seq analyses, and all other analyses presented in the original publication (see above).
  - **Chromosome_level_assembly_unmasked.fa**, which is the chromosome-level genome assembly after HiC chromosome-scale scaffolding.
- [02-Genome_annotations.tar.gz](02-Genome_annotations.tar.gz) contains the genome annotation files with all gene models in `.gff3` format and the funcional annotation reports in `.xlsx` format for both *O. fusiformis* and *C. teleta*. Again, as described above for [01-Owenia_fusiformis_genome_assemblies.tar.gz](01-Owenia_fusiformis_genome_assemblies.tar.gz), there are two different annotation files for *O. fusiformis*, which match each of the genome asembly files.
  - **Capitella_teleta_genome_annotation.gff3** contains the new updated gene models of *C. teleta*.
  - **Capitella_teleta_functional_annotation.xlsx** is the functional annotation report of *C. teleta*.
  - **Owenia_fusiformis_genome_annotation_scaffold_assembly.gff3** contains the gene models of *O. fusiformis* corresponding to **Scaffold_level_assembly_unmasked.fa**.


