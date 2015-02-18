## Source files

[**`Nlapillus.fa`**]

The *Nucella lapillus* transcriptome (`Nlapillus.fa`) is a dataset of the transcribed nucleotide sequence for the organism created by Chut et al. (2014). It is the dataset that was annotated in this project. The dataset is in `.fa` format and can be obtained from the Dryad Digital Repository (`http://dx.doi.org/10.5061/dryad.610dd`) specified in Chu et al. (2014).

[**`uniprot_sprot.fasta.gz`**]

The UniprotKB Swissprot dataset (`uniprot_sprot.fasta.gz`) contains protein information including amino acid sequence, protein description, and taxonomic information. It is the dataset against which the *N. lapillus* transcriptome was subject to `Blastx`. The Uniprot Swissprot dataset is in `.fasta` format and can be obtained from the Uniprot website (`http://www.uniprot.org/downloads`).

## Annotate transcriptome

[**`Nlap_uniprot_blastx.tab`**]

The `blastx` output dataset (`Nlap_uniprot_blastx.tab`) contains the contigs of *N. lapillus*. It is a dataset of proteins that were transcribed in *N. lapillus*, based on its transcriptome. Each contig has a corresponding Uniprot Swissprot ascension number. The dataset is in `.tab` format and is available on `SQLShare` as "`Nlap_uniprot_blastx.tab`". The Swissprot ascension numbers in this file do not have their own column and must be isolated. The dataset with ascension numbers isolated is available on `SQLShare` as "`Nlap_uniprot_blastx2_4.tab`".

[**`SPID and GO Numbers`**]

The `SPID and GO Numbers` table contains Uniprot Swissprot ascension numbers and their corresponding Gene Ontology identification codes. It links Swissprot information to full Gene Ontology information. It is available on SQLShare as "`SPID and GO Numbers`" (`https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320@washington.edu/SPID and GO Numbers`). It can be downloaded in `.csv` format.

[**`GO_to_GOSlim`**]

The `GO_to_GOSlim` table contains Gene Ontology identification codes and their corresponding Gene Ontology Slim codes. As the Gene Ontology is organized hierarchically, this table links full Gene Ontology information to more general Gene Ontology categories. It is available on `SQLShare` as "`GO_toGOSlim`" (`https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/GO_to_GOslim`). It can be downloaded in `.csv` format.

[**`UniprotNamesNamesReviewed_yes20130610`**]

The `UniprotNamesNamesReviewed_yes20130610` table contains protein names with corresponding Uniprot Swissprot ascension numbers. It links Swissprot information to protein names. It is available on `SQLShare` as "`UniprotNamesNamesReviewed_yes20130610`" (`https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/UniprotProtNamesReviewed_yes20130610_immune`). It can be downloaded in `.csv` format. 

## Products

[**`Nlap_annotated_GO.csv`**]

The `Nlap_annotated_GO.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has full Gene Ontology information, including Gene Ontology Slim categories. It has information on protein function corresponding to each transcribed contig. It is in `.csv` format. The dataset is available on `GitHub` (`https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products`) and `SQLShare` as "`Nlap_annotated`" (`https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated`).

[**`Nlap_annotated_proteinnames.csv`**]

The `Nlap_annotated_proteinnames.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has protein names corresponding to each contig. It is in `.csv` format. The dataset is available on `GitHub` (`https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products`) and `SQLShare` as "`Nlap_annotated_proteinnames`" (`https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated_proteinnames`).

[**`Nlap_GOSlim_count.png`**]

The `Nlap_GOSlim_count.png` file is a bar plot of the counts of protein functions in the *N. lapillus* transcriptome. It is an image (`.png` format) that can be found on `GitHub` (`https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_count.png`).

[**`Nlap_GOSlim_percent.png`**]

The `Nlap_GOSlim_percent.png` file is a pie chart of the proportions (in %) of protein functions in the *N. lapillus* transcriptome. It is an image (`.png` format) that can be found on `GitHub` (`https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_percent.png`).