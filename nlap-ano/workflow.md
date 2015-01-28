# Workflow

(steps before these are in "methods.md")
1. tab delimited output file from blastx
2. upload blastx output to SQLshare
3. join with sr320's [SPID and GO numbers](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/SPID%20and%20GO%20Numbers), make new table
4. join product from step 3 with sr320's [GO to GOslim table](https://sqlshare.escience.washington.edu/sqlshare/#s=query/sr320%40washington.edu/GO_to_GOslim)
5. download super file, this is the annotated transcriptome
