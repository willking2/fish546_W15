# Methods

To annotate the transcriptome of the dog whelk, *Nucella lapillus* [a], I used `Blastx v 2.2.29+` to annotate contigs against the UniProtKB Swiss-prot database [b], applying an E-value cut-off of 1E-20 to create a `blastx` output file [c]. 

The transcriptome of *N. lapillus* was obtained online as specified in Chu et al. (2014). `Blastx` was downloaded from the National Center for Biotechnology Information website as a stand-alone version. The UniProtKB Swiss-prot database was downloaded from the Universal Protein Resource website. For `Blastx`, the query sequence was the transcriptome of *N. lapillus* and the database for comparison was the UniprotKB Swiss-prot database. 

To annotate the contigs with protein information, I joined the `Blastx` output dataset with corresponding Gene Ontology (GO) information and protein names using `SQLShare`.

The Gene Ontology information was obtained from datasets available on `SQLShare` that link Uniprot SwissProt ascension numbers to GO identification codes [d] to GOSlim identification codes [e]. Similarly, the protein information were obtained from a dataset available on `SQLShare` that links Uniprot SwissProt ascension numbers to protein names [f]. Joins resulted in datasets of contigs with corresponding Gene ontology information [g] and protein names [h].

-------------------------------------------

Information on datasets included in these methods are available in the `Data_Records.md` file and can are matched by the bracketed letters.