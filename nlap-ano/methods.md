# Methods

To annotate the transcriptome of the dog whelk, *Nucella lapillus*, I used Blastx v 2.2.29+ to annotate contigs against the UniProtKB Swiss-prot database, applying an E-value cut-off of 1E-20.

The transcriptome of *N. lapillus* was obtained from the Dryad Digital Repository (http://dx.doi.org/10.5061/dryad.610dd) specified in Chu et al. (2014). Blastx was downloaded from the National Center for Biotechnology Information website (http://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) as a stand-alone version. The UniProtKB Swiss-prot database was downloaded from the Universal Protein Resource website (http://www.uniprot.org/downloads). For Blastx, the query sequence was the transcriptome of *N. lapillus* and the database for comparison was the UniprotKB Swiss-prot database. 
 

------------------------------------------------------------------

## QUESTIONS: 
hummingbird OS, verison, etc.? 

## outline, other details
1. main goal
2. query sequence: N. lapillus transcriptome from Chu et al
	- downloaded point and click style on Will's PC, then git hubbed to Hummingbird
	- Dryad Digital Repository. http://dx.doi.org/10.5061/dryad.610dd
	- downloaded 12 Jan 2015 on Windows 7 from Dryad 
2.5 working in srlab hummingbird
3. blast x info
	- blast stand-alone from NCBI
	- blastx installed in hummingbird
	- blastx: 2.2.29+
	- Package: blast 2.2.29, build Dec 10 2013 15:51:59
	- was previously configured so that you can use blast commands anywhere in hummingbird, doesn't have to be /bin directory
4. uniprot info
	- uniprotKB swiss-prot .fasta file from uniprot website
	- downloaded into hummingbird:~ srlab/willbigdata on 1/21/15 
5. get .tab file, and then...?
