---
layout: default
title: Patient Information
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 0
---

# Patient Information Profile

This profile inlcudes 40 data elements to capture the cancer patient’s demographics, contact information, performance status, tests performed, and referring physician. Five sub-profiles (not shown here) organize some of these elements into relevant groups (Address, Referring Physician. Testing Performed, ECOG Performance Status, and Karnofsky Performance Status).


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
record_id|Integer|Record id in the database|N/A|Required
dob|Date|Date of birth for the individual|N/A|Required
gender|CodeableConcept|A gender classification used for administrative purposes, not necessarily the same as a biological description or a sex identity|FHIR|Required
sex|CodeableConcept|The sex the patient was given at birth|Code Set|Required
pt_address_zipcode|String|The postal (zip) code of the physical home address of the patient|N/A|Required if known
pt_address|String|The street name and number or P.O. box of the physical home address of the patient|N/A|Required if known
pt_address_city|String|Name of city of the physical home address of the patient|N/A|Required if known
pt_address_state|String|Name of state of the physical home address of the patient|N/A|Required if known
pt_address_period|Period|Time period address has been in use|N/A|Required if known
mrn|String|Medical record number|N/A|Required
first_name|String|The given name(s) of the patient|N/A|Required
last_name|String|The family name of the patient|N/A|Required
race|CodeableConcept|Text code for patient's race|Code Set|Required
ethnicity|CodeableConcept|Text code patient's ethnicity|Code Set|Required
physician_name|String|First and last name of physician submitting the request, e.g., Joe Doe|N/A|Required
physician_contact|String|Physician's email|N/A|Required if known
physician_institution|String|Physician's institution|N/A|Required if known
other_physician_name|String|First and last name of other physician submitting the request, e.g., Joe Doe|N/A|Required if known
other_physician_contact|String|Other physician's email|N/A|Required if known
other_physician_institution|String|Other physician's institution|N/A|Required if known
germline|CodeableConcept|Germline test performed|Code Set|Required
tissue|CodeableConcept|Tisssue NGS performed|Code Set|Required
liquid_biopsy|CodeableConcept|Liquid biopsy performed|Code Set|Required
other_mol_test|CodeableConcept|Other molecular testing performed|Code Set|Required
ngs_report_1|Attachment|Upload the first NGS report|N/A|Required
ngs_report_2|Attachment|Upload the second NGS report|N/A|Required
ngs_report_3|Attachment|Upload the third NGS report|N/A|Required
other_mol_test_report|Attachment|Upload any other molecular testing report|N/A|Required
question_for_mtb|String|A detailed question to the MTB group|N/A|Required
smoking_status|CodeableConcept|Text code for patient's smoking status|SNOMED CT|Required
pack_years|Decimal|Number with one decimal place for pack-years|N/A|Required
other_exposures|CodeableConcept|Check one or more other exposures|Code Set|Required if known
ecog|CodeableConcept|Patient's performance status according to the ECOG score|ECOG Performance Status Score|Required
ecogps_interpretation|CodeableConcept|A categorical assessment of the ECOG score|ECOG Performance Status Scale|Required if known
ecog_date_full|Date|Date the ECOG status was assessed (closest to the MTB review date)|N/A|Required
karnofsky|CodeableConcept|Patient's performance status using the Karnofsky score|Code Set|Required
kps_interpretation|CodeableConcept|A categorical assessment of the Karnofsky score |Karnofsky Performance Status Scale|Required if known
karnofsky_date|Date|Date the Karnofsky status assessed (closest to the MTB review date)|N/A|Required
date_cur_pt_info|Date|Date of curation|N/A|Required if known
cur_by_pt_info|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is not repeatable and one record is expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>