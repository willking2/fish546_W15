#Get UniprotKB Swiss-prot dataset

# download from internet
`hummingbird:willbigdata srlab$ pwd
/Users/srlab/willbigdata
hummingbird:willbigdata srlab$ curl -o uniprot_sprot.fasta.gz ftp://ftp.uniprot
.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot
.fasta.gz`

# unzip

`hummingbird:willbigdata srlab$ pwd
/Users/srlab/willbigdata
hummingbird:willbigdata srlab$ ls
uniprot_sprot.fasta.gz
hummingbird:willbigdata srlab$ gzip -d uniprot_sprot.fasta.gz
hummingbird:willbigdata srlab$ ls
uniprot_sprot.fasta
hummingbird:willbigdata srlab$`

