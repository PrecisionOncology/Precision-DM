---
layout: default
title: Treatment Neoadjuvant
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 10
---

# Treatment Neoadjuvant Profile

This profile includes 29 data elements to capture main information on the neoadjuvant treatment (if applicable). The "MedicationRegimen" sub-profile (not shown here) groups the names of all neoadjuvant medications (up to 6) with the start and end dates.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
isa_second_primary_neoadj|Boolean|This is or is not a therapy for a second primary cancer|N/A|Required
isa_third_primary_neoadj|Boolean|This is or is not a therapy for a third primary cancer|N/A|Required
neo_yn|Boolean|The patient received neoadjuvant therapy or not|N/A|Required
med_neoadj_ther_trial_yn|Boolean|The patient received neoadjuvant therapy in a clinical trial or not|N/A|Required
med_neoadj_ther_off_lab_yn|Boolean|The patient received an off-label neoadjuvant therapy|N/A|Required
neo1_therapy|CodeableConcept|The 1st medication of the neoadjuvant regimen|RxNorm|Required
neo2_therapy|CodeableConcept|The 2nd medication of the neoadjuvant regimen|RxNorm|Required
neo3_therapy|CodeableConcept|The 3rd medication of the neoadjuvant regimen|RxNorm|Required
neo4_therapy|CodeableConcept|The 4th medication of the neoadjuvant regimen|RxNorm|Required
neo5_therapy|CodeableConcept|The 5th medication of the neoadjuvant regimen|RxNorm|Required
neo6_therapy|CodeableConcept|The 6th medication of the neoadjuvant regimen|RxNorm|Required
neo1_sd|Date|The start date of the administration of the 1st medication of the neoadjuvant regimen|N/A|Required
neo1_ed|Date|The end date of the administration of the 1st medication of the neoadjuvant regimen|N/A|Required
neo2_sd|Date|The start date of the administration of the 2nd medication of the neoadjuvant regimen|N/A|Required
neo2_ed|Date|The end date of the administration of the 2nd medication of the neoadjuvant regimen|N/A|Required
neo3_sd|Date|The start date of the administration of the 3rd medication of the neoadjuvant regimen|N/A|Required
neo3_ed|Date|The end date of the administration of the 3rd medication of the neoadjuvant regimen|N/A|Required
neo4_sd|Date|The start date of the administration of the 4th medication of the neoadjuvant regimen|N/A|Required
neo4_ed|Date|The end date of the administration of the 4th medication of the neoadjuvant regimen|N/A|Required
neo5_sd|Date|The start date of the administration of the 5th medication of the neoadjuvant regimen|N/A|Required
neo5_ed|Date|The end date of the administration of the 5th medication of the neoadjuvant regimen|N/A|Required
neo6_sd|Date|The start date of the administration of the 6th medication of the neoadjuvant regimen|N/A|Required
neo6_ed|Date|The end date of the administration of the 6th medication of the neoadjuvant regimen|N/A|Required
neo_intent|CodeableConcept|The purpose of the neoadjuvant medication or regimen, either curative or palliative|SNOMED CT|Required if known
neo_discontinue|Boolean|The neoadjuvant medication or regimen discontinued or not|N/A|Required
neo_discontinue_reason|CodeableConcept|A code explaining unplanned or premature termination of the neoadjuvant medication or regimen|Code Set|Required
neo_toxicity|String|Explain the type of toxicity that led to neoadjuvant therapy discontinuation|N/A|Required
date_cur_treat_neoadj|Date|Date of curation|N/A|Required if known
cur_by_treat_neoadj|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>