---
layout: default
title: Tumor Sample Information
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 5
---

# Tumor Sample Information Profile

This profile inlcudes 44 data elements to capture anatomic, sample, and testing information for each tumor sample considered. The "Specimen" sub-profile (not shown here) organize some of these elements that characterize the specimen collected for the genomic analysis.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
surg_path_id|String|The ID number from the surgical pathology report|N/A|Required
date_specimen_collected|Date|Date of profile specimen collected|N/A|Required
site_specimen|CodeableConcept|The anatomical collection site|SNOMED CT|Required
spec_type|CodeableConcept|The kind of material that forms the specimen|Code Set|Required
nci_code_sample|codeableConcept|NCI code for the specimen|NCIt|Required if known
spec_laterality|CodeableConcept|Body side of the collection site, if needed to distinguish from a similar location on the other side of the body.|SNOMED CT|Required
immunostain|CodeableConcept|IHC marker tested|Code Set|Required
er_clone|String|The antibody clone used for staining|N/A|Required if known
er_interpretation|CodeableConcept|The IHC interpretation|Code Set|Required if known
er_ihc_score|CodeableConcept|The IHC score|Code Set|Required if known
er_ihc_label|Percentage|The IHC result|N/A|Required if known
pr_clone|String|The antibody clone used for staining|N/A|Required if known
pr_interpretation|CodeableConcept|The IHC interpretation|Code Set|Required if known
pr_ihc_score|CodeableConcept|The IHC score|Code Set|Required if known
pr_ihc_label|Percentage|The IHC result|N/A|Required if known
her_clone|String|The antibody clone used for staining|N/A|Required if known
her_interpretation|CodeableConcept|The IHC interpretation|Code Set|Required if known
her_ihc_score|CodeableConcept|The IHC score|Code Set|Required if known
her_ihc_label|Percentage|The IHC result|N/A|Required if known
ar_clone|String|The antibody clone used for staining|N/A|Required if known
ar_interpretation|CodeableConcept|The IHC interpretation|Code Set|Required if known
ar_ihc_score|CodeableConcept|The IHC score|Code Set|Required if known
ar_ihc_label|Percentage|The IHC result|N/A|Required if known
pdl1_clone|String|The antibody clone used for staining|N/A|Required if known
pdl1_cps|Percentage|PDL1 CPS|N/A|Required
pdl1_ic_label|Percentage|PDL1 IC|N/A|Required
pdl1_tps|String|PDL1 TPS|N/A|Required
pdl1_ics|Percentage|PDL1 ICS|N/A|Required
her2_fish|String|HER2 FISH performed|N/A|Required
her2_fish_ratio|Decimal|HER2 FISH ratio|N/A|Required
her2_fish_interpretation|CodeableConcept|HER2 FISH interpretation|Code Set|Required
mmr_proteins|CodeableConcept|Mismatch repair proteins as assessed by immunohistochemistry|Code Set|Required
mmr_result|CodeableConcept|Mismatch repair protein assessment|Code Set|Required
mmr_protein|CodeableConcept|Impaired mismatch repair protein|Code Set|Required
fish_binary|Boolean|FISH was performed or not performed|N/A|Required
fish_assay|CodeableConcept|FISH assay|Code Set|Required
fish_result|Decimal|Gene to control ratio|N/A|Required
fish_interpretation|CodeableConcept|FISH interpretation|Code Set|Required
tumor_purity|String|The proportion of cancer cells in the tumor tissue|N/A|Required
msi_modality|CodeableConcept|How was MSI measured for this sequenced sample (choose all that apply)?|Code Set|Required
sample_reviewed_mtb|Boolean|Tumor Sample Reviewed at MTB|N/A|Required
date_mtb_disc|Date|Date of review|N/A|Required
date_cur_tumor_sample|Date|Date of curation|N/A|Required if known
cur_by_tumor_sample|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>