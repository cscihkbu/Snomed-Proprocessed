# Snomed-Proprocessed

This repository contains preprocessed Snomed relations files that connect drugs and diagnoses from MIMIC-III to Snomed. Formulary CD and ICD code are used for represent drugs and diagnoses respectively. And Snomed ID is used for represent other medical entities like finding sites.





#### Drug_relations.txt
Each row is a triplet that connect a drug from MIMIC-III to a entity from Snomed-

	Drug_formulary_CD Relationship_ID Snomed_Entity_ID Direction
	
For Direction column, if it is 0, means Drug_formulary_CD -> Snomed_Entity_ID and vise versa.
	
#### Diagnosis_relations.txt
Each row is a triplet  that connect a diagnosis from MIMIC-III to a entity from Snomed-

	Diagnosis_ICD Relationship_ID Snomed_Entity_ID Direction
	
#### Snomed_entity_relations.txt
Each row is a triplet that connect entities from Snomed-

	Snomed_ICD Relationship_ID Snomed_Entity_ID Direction


#### snomedId_to_names.txt-

each row map a Snomed_Entity_ID or Relationship_ID to name- 

	(Snomed_Entity_ID or Relationship_ID)  Name


