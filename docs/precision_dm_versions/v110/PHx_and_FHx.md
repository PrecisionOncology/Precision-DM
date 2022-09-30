---
layout: default
title: Personal and Family History
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 1
---

# Personal and Family History Profile

This profile inlcudes 17 data elements to capture cancer patient’s personal medical history of other neoplasms and family history. Five sub-profiles (not shown here) organize some of these elements into relevant groups (Personal History of Other Cancer, Family History, Family History>1st Degree, Family History>2nd Degree, Family History>3rd Degree).


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
personal_cancer_history|Boolean|Personal history of cancer diagnoses, other than the current condition|N/A|Required
personal_cancer_dx|CodeableConcept|Prior cancer diagnosis|NCIt|Required
personal_cancer_age|Decimal|Patient's age when diagnosed with a first cancer|N/A|Required
personal_other_cancer_dx|CodeableConcept|The diagnosis for a second cancer|NCIt|Required
personal_other_cancer_age|Decimal|Patient's age when diagnosed with a second cancer|N/A|Required
fam_hx_cancer|CodeableConcept|Family history of cancer|Code Set|Required
no_first_deg_rel_cancer|Integer|Number of first-degree relatives (parents, siblings, children) with cancer|N/A|Required
first_deg_rel_under_50|Integer|Number of first-degree relatives  (parents, siblings, children) with cancer before the age of 50|N/A|Required
fst_deg_cancer_types|CodeableConcept|List of cancer types in  first-degree relatives|Code Set|Required
no_second_deg_rel_cancer|Integer|Number of second-degree relatives (grandparents, aunts and uncles, nieces and nephews, half-siblings, grandchildren) with cancer|N/A|Required
sec_deg_rel_under_50|Integer|Number of second-degree relatives (grandparents, aunts and uncles, nieces and nephews, half-siblings, grandchildren) with cancer before the age of 50|N/A|Required
snd_deg_cancer_types|CodeableConcept|List of cancer types in second-degree relatives|Code Set|Required
no_third_deg_rel_cancer|Integer|Number of third-degree relatives (first cousins, great aunts and uncles, great grandparents or great grandchildren) with cancer|N/A|Required
third_deg_rel_under_50|Integer|Number of third-degree relatives (first cousins, great aunts and uncles, great grandparents or great grandchildren) with cancer before the age of 50|N/A|Required
trd_deg_cancer_types|CodeableConcept|List of cancer types in third-degree relatives|Code Set|Required
date_cur_fhx|Date|Date of curation|N/A|Required if known
cur_by_fhx|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is not repeatable and one record is expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>