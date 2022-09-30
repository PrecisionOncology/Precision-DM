---
layout: default
title: Disease Diagnosis
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 4
---

# Disease Diagnosis Profile

This profile inlcudes 28 data elements to capture information on the category of the primary tumor, based on its size and extent identified through physical examination, imaging, and/or biopsy. Three sub-profiles (not shown here) organize some of these elements to describe primary and secondary cancer conditions (Primary Cancer and Secondary Cancer).


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
isa_second_primary|Boolean|The diagnosis is for a second primary cancer|N/A|Required
isa_third_primary|Boolean|The diagnosis is for a third primary cancer|N/A|Required
primary_ca_path_dx_dt_full|Date|Date of primary cancer pathologic Dx|N/A|Required
primary_path_dx|String|Description from pathology report|N/A|Required
primary_cancer_type|String|Primary malignant neoplastic disease as reported in EPIC|N/A|Required
primary_cancer_type_nci|CodeableConcept|Select the NCI code for the primary malignant neoplastic disease|NCIt|Required if known
primary_laterality|CodeableConcept|Body side of the primary body location|SNOMED CT|Required
local_recurrence_dt|Date|Date of local recurrence|N/A|Required if known
metdx_dt_full|Date|Date of metastatic Dx|N/A|Required
primary_grade|String|Grade for the morphologic and behavioral characteristics of the primary cancer|N/A|Required
primary_verif_status|CodeableConcept|A flag indicating the status of the primary condition|FHIR|Required if known
path_stage_at_dx|CodeableConcept|The category describing the extent of the primary disease, according to the TNM staging rules (path stage)|TNM|Required
p_t|CodeableConcept|Category of the primary tumor according to TNM staging rules (path stage)|TNM|Required
p_n|CodeableConcept|Category of regional lymph nodes for the primary condition according to TNM staging rules (path stage)|TNM|Required
p_m|CodeableConcept|Category of distant metastases for the primary condition according to TNM staging rules. (path stage)|TNM|Required
clinical_stage_at_dx|CodeableConcept|The category describing the extent of the primary disease, according to the TNM staging rules (clinical stage)|TNM|Required
c_t|CodeableConcept|Category of the primary tumor according to TNM staging rules (clinical stage)|TNM|Required
c_n|CodeableConcept|Category of regional lymph nodes for the primary condition according to TNM staging rules (clinical stage)|TNM|Required
c_m|CodeableConcept|Category of distant metastases for the primary condition according to TNM staging rules (clinical stage)|TNM|Required
secondary_ca_path_dx_dt_full|Date|Date of secondary cancer pathologic Dx|N/A|Required
secondary_path_dx|String|Description from pathology report|N/A|Required
sec_cancer_type|String|Secondary malignant neoplastic disease as reported in EPIC|N/A|Required
sec_cancer_type_nci|CodeableConcept|Select the NCI code for the secondary malignant neoplastic disease|NCIt|Required if known
sec_laterality|CodeableConcept|Body side of the body location, if needed to distinguish from a similar location on the other side of the body.|SNOMED CT|Required
sec_grade|String|A description of the morphologic and behavioral characteristics of the cancer|N/A|Required
sec_verif_status|CodeableConcept|A flag indicating whether the condition is unconfirmed, provisional, differential, confirmed, refuted, or entered-in-error|FHIR|Required if known
date_cur_disease_dx|Date|Date of curation|N/A|Required if known
cur_by_disease_dx|String|The name of the curator who modified the instrument|N/A|Required if known


### Note
<em>1. This profile is repeatable and more than one records can be expected per patient</em>