---
layout: default
title: Treatment Radiation
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 13
---

# Treatment Radiation Profile

This profile includes 20 data elements to capture detailed information on any radiotherapy the patient received (if applicable).


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
isa_second_primary_rad|Boolean|This is or is not a therapy for a second primary cancer|N/A|Required
isa_third_primary_rad|Boolean|This is or is not a therapy for a third primary cancer|N/A|Required
rad_yn|Boolean|The patient received radiation therapy|N/A|Required
rad_therapy|CodeableConcept|Code for the radiation therapy procedure performed|Code Set|Required
ext_beam_rad_ther_del|CodeableConcept|Type of delivery of the external beam radiation therapy|Code Set|Required if known
ext_beam_rad_ther_modality|CodeableConcept|Type of modality of the external beam radiation therapy|Code Set|Required if known
brachy_rad_ther_modality|CodeableConcept|Type of modality of brachytherapy radiation therapy|Code Set|Required if known
radiation_technique|CodeableConcept|Technique used in radiation therapy|Code Set|Required if known
rad_ther_no_sessions|Integer|The number of sessions in a course of radiotherapy|N/A|Required if known
rad_ther_total_dose|Decimal|The total amount of radiation delivered to this volume within the scope of this dose delivery in cGy|N/A|Required
rad_ther_fractions|Integer|The number of fractions delivered to this volume|N/A|Required
radiat_start_date_full|Date|The start date for radiation therapy|N/A|Required
radiat_end_date_full|Date|The end date for radiation therapy|N/A|Required
rad_discontinue|Boolean|Radiation therapy discontinued|N/A|Required
rad_discontinue_reason|CodeableConcept|A code explaining unplanned or premature termination of a radiation therapy|Code Set|Required
rad_site|CodeableConcept|The body location(s) where the procedure was performed|SNOMED CT|Required
rad_laterality|CodeableConcept|Body side of the body location, if needed to distinguish from a similar location on the other side of the body|SNOMED CT|Required
rad_intent|CodeableConcept|The purpose of the medication, either curative or palliative|SNOMED CT|Required
date_cur_treat_rad|Date|Date of curation|N/A|Required if known
cur_by_treat_rad|String|The name of the curator who modified the instrument|N/A|Required


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>