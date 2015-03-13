# Record of data files used and generated as part of this *Nucella lapillus* transcriptome annotation

## Source files

- [`Nlapillus.fa`]

The *Nucella lapillus* transcriptome (`Nlapillus.fa`) is a dataset of the transcribed nucleotide sequence for the organism created by Chut et al. (2014). It is the dataset that was annotated in this project. The dataset is in `.fa` format and can be obtained from the Dryad Digital Repository ([here](http://dx.doi.org/10.5061/dryad.610dd)) specified in Chu et al. (2014).

- [`uniprot_sprot.fasta.gz`]

The UniprotKB Swissprot dataset (`uniprot_sprot.fasta.gz`) contains protein information including amino acid sequence, protein description, and taxonomic information. It is the dataset against which the *N. lapillus* transcriptome was subject to `Blastx`. The Uniprot Swissprot dataset is in `.fasta` format and can be obtained from the Uniprot website ([here](http://www.uniprot.org/downloads)).

## Intermediary files

- [`Nlap_uniprot_blastx.tab`]

The `blastx` output dataset (`Nlap_uniprot_blastx.tab`) contains the contigs of *N. lapillus*. It is a dataset of proteins that were transcribed in *N. lapillus*, based on its transcriptome. Each contig has a corresponding Uniprot Swissprot ascension number. The dataset is in `.tab` format and is available on `SQLShare` as "`Nlap_uniprot_blastx.tab`". The Swissprot ascension numbers in this file do not have their own column and must be isolated. The dataset with ascension numbers isolated is available on `SQLShare` as "`Nlap_uniprot_blastx2_4.tab`".

- [`SPID and GO Numbers`]

The `SPID and GO Numbers` table contains Uniprot Swissprot ascension numbers and their corresponding Gene Ontology identification codes. It links Swissprot information to full Gene Ontology information. It is available on SQLShare as "`SPID and GO Numbers`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320@washington.edu/SPID_and_GO_Numbers)). It can be downloaded in `.csv` format.

- [`GO_to_GOSlim`]

The `GO_to_GOSlim` table contains Gene Ontology identification codes and their corresponding Gene Ontology Slim codes. As the Gene Ontology is organized hierarchically, this table links full Gene Ontology information to more general Gene Ontology categories. It is available on `SQLShare` as "`GO_toGOSlim`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/GO_to_GOslim)). It can be downloaded in `.csv` format.

- [`UniprotNamesNamesReviewed_yes20130610`]

The `UniprotNamesNamesReviewed_yes20130610` table contains protein names with corresponding Uniprot Swissprot ascension numbers. It links Swissprot information to protein names. It is available on `SQLShare` as "`UniprotNamesNamesReviewed_yes20130610`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/UniprotProtNamesReviewed_yes20130610_immune)). It can be downloaded in `.csv` format. 

## Products

- [`Nlap_annotated_GO.csv`]

The `Nlap_annotated_GO.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has full Gene Ontology information, including Gene Ontology Slim categories. It has information on protein function corresponding to each transcribed contig. It is in `.csv` format. The dataset is available on `GitHub` ([here](https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products)) and `SQLShare` as "`Nlap_annotated`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated)).

The file contains 2,433 rows of contig annotations corresponding to 117 unique Swiss Prot Id's.  


- [`Nlap_annotated_proteinnames.csv`]

The `Nlap_annotated_proteinnames.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has protein names corresponding to each contig. It is in `.csv` format. The dataset is available on `GitHub` ([here](https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products)) and `SQLShare` as "`Nlap_annotated_proteinnames`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated_proteinnames)).

The file contains 145 rows of contig annotations corresponding to 116 protein names. 

- [`Nlap_annotated_GO_stress.csv`]

The`Nlap_annotated_GO_stress.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has full Gene Ontology information, including Gene Ontology Slim categories, for contigs related to stress response only. It has information on protein function corresponding to each transcribed contig. It is in `.csv` format. The dataset is available on `GitHub` ([here](https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products)) and `SQLShare` as "`Nlap_annotated_GO_stress`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated_GO_stress.csv)).  

- [`Nlap_annotated_proteinnames_stress.csv`]

The `Nlap_annotated_proteinnames_stress.csv` file is the annotated *N. lapillus* transcriptome produced from this project that has protein names corresponding to each contig, for contigs related to stress response only. It is in `.csv` format. The dataset is available on `GitHub` ([here](https://github.com/willking2/fish546_W15/tree/master/nlap-ano/products)) and `SQLShare` as "`Nlap_annotated_proteinnames_stress`" ([here](https://sqlshare.escience.washington.edu/sqlshare/#s=query/wking2%40washington.edu/Nlap_annotated_proteinnames_stress)).

- [`Nlap_GOSlim_counts_allaspects.png`]

The `Nlap_GOSlim_counts_allaspects.png` file is a bar plot of the counts of protein functions in the *N. lapillus* transcriptome for all aspects. It is an image (`.png` format) that can be found on `GitHub` ([here](https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_counts_allaspects.png)).

Proteins of "other molecular function" had the highest count.

- [`Nlap_GOSlim_counts_biologicalprocess.png`]

The `Nlap_GOSlim_counts_biologicalprocess.png` file is a bar plot of the counts of protein functions in the *N. lapillus* transcriptome for the GO biological process aspect. It is an image (`.png` format) that can be found on `GitHub` ([here](https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_counts_biologicalprocess.png)).

- [`Nlap_GOSlim_counts_cellularcomponent.png`]
 
The `Nlap_GOSlim_counts_cellularcomponent.png` file is a bar plot of the counts of protein functions in the *N. lapillus* transcriptome for the GO cellular component aspect. It is an image (`.png` format) that can be found on `GitHub` ([here](https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_counts_cellularcomponent.png)).

- [`Nlap_GOSlim_counts_molecularfunction.png`]

The `Nlap_GOSlim_counts_molecularfunction.png` file is a bar plot of the counts of protein functions in the *N. lapillus* transcriptome for the GO molecular function aspect. It is an image (`.png` format) that can be found on `GitHub` ([here](https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_counts_molecularfunction.png)).

- [`Nlap_GOSlim_pie.png`]

The `Nlap_GOSlim_pie.png` file is a pie chart of the proportions (in %) of protein functions in the *N. lapillus* transcriptome. It is an image (`.png` format) that can be found on `GitHub` ([here](https://github.com/willking2/fish546_W15/blob/master/nlap-ano/products/Nlap_GOSlim_pie.png)).

Proteins of "other molecular function" had the highest proportion. 
