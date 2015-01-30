# Workflow

- tab delimited output file from blastx
- upload blastx output to SQLshare
- join with sr320's [SPID and GO numbers](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/SPID%20and%20GO%20Numbers), make new table
- join product from step 3 with sr320's [GO to GOslim table](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/GO_to_GOslim)
- download super file, this is the annotated transcriptome

-------------------------------------------------------
# 1) download uniprot swissprot dataset

## download from internet

`hummingbird:willbigdata srlab$ pwd
/Users/srlab/willbigdata
hummingbird:willbigdata srlab$ curl -o uniprot_sprot.fasta.gz ftp://ftp.uniprot
.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot
.fasta.gz`

## unzip

`hummingbird:willbigdata srlab$ pwd
/Users/srlab/willbigdata
hummingbird:willbigdata srlab$ ls
uniprot_sprot.fasta.gz
hummingbird:willbigdata srlab$ gzip -d uniprot_sprot.fasta.gz
hummingbird:willbigdata srlab$ ls
uniprot_sprot.fasta
hummingbird:willbigdata srlab$`

# 2) make uniprot into a blast database

`hummingbird:willbigdata srlab$ pwd
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
Adding sequences from FASTA; added 547357 sequences in 54.0656 seconds.`

# 3) run blastx

`hummingbird:willbigdata srlab$ pwd
/Users/srlab/willbigdata
hummingbird:willbigdata srlab$ ls
uniprot_sprot.fasta             uniprot_sprot_21JAN2015.pin
uniprot_sprot_21JAN2015.phr     uniprot_sprot_21JAN2015.psq
hummingbird:willbigdata srlab$ blastx -query /Users/srlab/fish546_W15/nlap-ano/
data/N_lapillus.fa -db uniprot_sprot_21JAN2015 -out Nlap_uniprot_blastx.tab -evalue 1E-20 -max_target_seqs 1 -outfmt 6`

# 4)
