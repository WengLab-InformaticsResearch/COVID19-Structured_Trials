# COVID19-Structured_Trials
An OMOP Common Data Model-Compliant Annotated Corpus for COVID-19 Clinical Trials  
This README file describes the dataset accompanying the above publication. 

## 700_annotated_trials
It includes the original free text eligibility criteria (.txt) and annotations (.ann) for each trial. The  annotation file (.ann）can be opened by [Brat](https://brat.nlplab.org/).

## key_criteria_corpus
Six commonly used criteria across all COVID-19 trials about current age, high-risk status (e.g., hospital worker), COVID-19 status (e.g., yes, cleared, no), days since diagnosis (if relevant), current hospitalization or intensive care unit (ICU) admission, and pregnancy status are specified as “key criteria” and recorded in this .CSV table.

## all_trials_corpus
Metadata information of each trial are included in this .CSV file, such title, location, study type, phase and etc. 

## all_criteria_corpus
Structured eligibility criteria with normalized concepts are included in this .CSV file.  
Main columns:  
 	  **nct_id**: clinical trial ID in clinicaltrials.gov  
 	  **entity_source_text**: segment of the original description of the entity in the clinical trial eligibility criteria source text  
 	  **start_index**: the position in the criteria source text where the entity starts  
 	  **end_index**: the position in the criteria source text where the entity ends  
 	  **concept_id**: mapped concept ID in the standard vocabulary of the entity  
 	  **concept_name**: mapped concept name in the standard vocabulary of the entity  
 	  **domain**: domain ('Drug','Condition','Procedure','Device','Measurement') of the concept   
 	  **temporal_source_text**: segment of the corresponded temporal attribute of the entity in original criteria text  
 	  **days**: normalized temporal attribute as the number of days   
 	  **numeric_source_text**: segment of the corresponded numerical attribute of the entity in original criteria text  
 	  **numeric_att_min**: lower bound of the normalized numerical attribute  
 	  **numeric_att_max**: upper bound of the normalized numerical attribute  
 	  **is_exclusion**: '1' for exclusion criteria and '0' for inclusion criteria  
