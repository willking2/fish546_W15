	    1  pwd
	    2  ls
	    3  cd Desktop/
	    4  ls
	    5  tr '|' '\t' Nlap_uniprot_blastx.tab Nlap_uniprot_blastx2.tab
	    6  tr '|' '\t' Nlap_uniprot_blastx.tab >  Nlap_uniprot_blastx2.tab
	    7  tr --help
	    8  rm Nlap_uniprot_blastx2.tab
	    9  ls
	   10  cat Nlap_uniprot_blastx.tab | tr '|
	' '\t' > Nlap_uniprot_blastx2.tab
	   11  ls
	   12  history
	   13  history > separate_out_SPID.md
