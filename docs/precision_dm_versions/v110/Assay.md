---
layout: default
title: Assay
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 6
---

# Assay Profile

This profile inlcudes 16 data elements to represent the molecular assay specifications.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
tumor_prof_report|Attachment|Upload tumor profiling report|N/A|Required
date_tumor_prof_rept|Date|The date/time this report was issued|N/A|Required
tumor_test_type|CodeableConcept|The method used to perform the genetic test.  Examples include Fluorescent in situ hybridization (FISH), polymerase chain reaction-based assays (PCR), and next-generation sequencing (NGS).|Code Set|Required
tumor_prof_provider|CodeableConcept|The name of the organization producing the report|Code Set|Required
assay|CodeableConcept|The range(s) of the DNA sequence examined|Code Set|Required
other_assay|String|Additional description if "Other" is selected in the "Test Assay" question|N/A|Required
surg_path_id_assay|String|The ID number from the surgical pathology report|N/A|Required
tumor_prof_case_id|String|The tumor profiling case ID|N/A|Required
coverage|String|Sequencing depth|N/A|Required
tmb|Integer|The total number of mutations (changes) found in the DNA of cancer cells|N/A|Required
loh|String|The genomic loss of heterozygosity|N/A|Required
loh_assay|String|The assay loss of heterozygosity|N/A|Required
msi_status|CodeableConcept|Microsatellite status|Code Set|Required
msi_date|Date|MSI date|N/A|Required
date_cur_assay|Date|Date of curation|N/A|Required if known
cur_by_assay|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>