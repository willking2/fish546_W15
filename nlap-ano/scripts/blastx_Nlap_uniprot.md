#blastx 

	hummingbird:willbigdata srlab$ pwd
	/Users/srlab/willbigdata
	hummingbird:willbigdata srlab$ ls
	uniprot_sprot.fasta             uniprot_sprot_21JAN2015.pin
	uniprot_sprot_21JAN2015.phr     uniprot_sprot_21JAN2015.psq
	hummingbird:willbigdata srlab$ blastx -query /Users/srlab/fish546_W15/nlap-ano/
	data/N_lapillus.fa -db uniprot_sprot_21JAN2015 -out Nlap_uniprot_blastx.tab -evalue 1E-20 -max_target_seqs 1 -outfmt 6