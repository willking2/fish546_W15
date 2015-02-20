#Subset rows from GO info annotation product file that are related to stress response (GO slim bin)

	$ awk -F"," '/[Ss]tress response/ {print $0}' Nlap_annotated_GO.csv > Nlap_anno
	tated_GO_stress.csv