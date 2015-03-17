## Methods for *Nucella lapillus* transcriptome annotation

To annotate the transcriptome of the dog whelk, *Nucella lapillus* [`Nlapillus.fa`], I used `Blastx v 2.2.29+` to annotate contigs against the UniProtKB Swiss-prot database [`uniprot_sprot.fasta.gz`], applying an E-value cut-off of 1E-20 to create a `blastx` output file [`Nlap_uniprot_blastx.tab`]. 

The transcriptome of *N. lapillus* was obtained online as specified in Chu et al. (2014). `Blastx` was downloaded from the National Center for Biotechnology Information website as a stand-alone version. The UniProtKB Swiss-prot database was downloaded from the Universal Protein Resource website. For `Blastx`, the query sequence was the transcriptome of *N. lapillus* and the database for comparison was the UniprotKB Swiss-prot database. 

To annotate the contigs with protein information, I joined the `Blastx` output dataset with corresponding Gene Ontology (GO) information and protein names using `SQLShare`.

The Gene Ontology information was obtained from datasets available on `SQLShare` that link Uniprot SwissProt ascension numbers to GO identification codes [`SPID and GO Numbers`] to GOSlim identification codes [`GO_to_GOSlim`]. Similarly, protein information was obtained from a dataset available on `SQLShare` that links Uniprot SwissProt ascension numbers to protein names [`UniprotNamesNamesReviewed_yes20130610`]. Joins resulted in datasets of contigs with corresponding Gene ontology information [`Nlap_annotated_GO.csv`] and protein names [`Nlap_annotated_proteinnames.csv`]. Using these files, I also created subset datasets containing only information for contigs related to stress response [`Nlap_annotated_GO_stress.csv`; `Nlap_annotated_proteinnames_stress.csv`].

Counts [`Nlap_GOSlim_counts_allaspects.png`] and proportions [`Nlap_GOSlim_pie.png`] by protein functions of contigs were plotted. Plots separated by Gene Ontology aspects [`Nlap_GOSlim_counts_biologicalprocess.png`, `Nlap_GOSlim_counts_cellularcomponent.png`, and `Nlap_GOSlim_counts_molecularfunction.png`] were also generated. All plots were generated in Microsoft Excel. 

-------------------------------------------

Information on datasets included in these methods are available in the `Data_Records.md` file (available [here](./Data_Records.md)) and are matched by the bracketed file names.

The workflow of this project can be found [here](../workflow.md).