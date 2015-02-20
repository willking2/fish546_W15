# make uniprot into a blast database

	hummingbird:willbigdata srlab$ pwd
	/Users/srlab/willbigdata
	hummingbird:willbigdata srlab$ ls
	uniprot_sprot.fasta
	hummingbird:willbigdata srlab$ makeblastdb -in uniprot_sprot.fasta -dbtype -out uniprot_sprot_21JAN2015
	
	
	Building a new DB, current time: 01/21/2015 20:48:51
	New DB name:   uniprot_sprot_21JAN2015
	New DB title:  uniprot_sprot.fasta
	Sequence type: Protein
	Keep Linkouts: T
	Keep MBits: T
	Maximum file size: 1000000000B
	Adding sequences from FASTA; added 547357 sequences in 54.0656 seconds.