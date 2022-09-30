---
layout: default
title: Germline Profiling Data
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 2
---

# Germline Profiling Data Profile

This profile inlcudes 12 data elements to capture genetic counseling and germline assay specifications.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
genetic_couns|CodeableConcept|Genetic counseling visit occurred|Code Set|Required
gen_date_full|Date|The date of the genetic counseling visit|N/A|Required
germ_test_rec|Boolean|Genetic counseling recommended germline testing|N/A|Required
germline_report|Attachment|Upload the germline report|N/A|Required
germ_report_case_id|String|The ID number from the germline report|N/A|Required
germline_test_provider|CodeableConcept|Name of the germline test provider (select from a list)|Code Set|Required
germline_test_prov_name|String|Name of the germline test provider (if not included in the list)|N/A|Required if known
germline_assay|CodeableConcept|The range(s) of the DNA sequence examined|Code Set|Required
germline_other_assay|String|Additional description if "Other" is selected in the "Germline Test Assay" question|N/A|Required
gtest_date_full|Date|The date of the germline test|N/A|Required
date_cur_germ_prof|Date|Date of curation|N/A|Required if known
cur_by_germ_prof|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>