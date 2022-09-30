---
layout: default
title: Treatment Surgery
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 12
---

# Treatment Surgery Profile

This profile includes 11 data elements to capture detailed information on patient's surgery (if applicable).


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
isa_second_primary_surgery|Boolean|This is or is not a therapy for a second primary cancer|N/A|Required
isa_third_primary_surgery|Boolean|This is or is not a therapy for a third primary cancer|N/A|Required
surgery_yn|Boolean|The patient had a surgical resection, either curative or palliative|N/A|Required
surgery_code|CodeableConcept|Code for the surgical procedure performed|SNOMED CT|Required if known
surgical_resection_date|Date|The date of the surgical resection|N/A|Required if known
surgery_site|CodeableConcept|The body location(s) where the procedure was performed|SNOMED CT|Required
surgery_laterality|CodeableConcept|Body side of the body location, if needed to distinguish from a similar location on the other side of the body|SNOMED CT|Required
surgery_intent|CodeableConcept|The purpose of the medication, either curative or palliative|SNOMED CT|Required if known
surgery_reference|CodeableConcept|Reference to a primary or secondary cancer condition|Code Set|Required if known
date_cur_treat_surg|Date|Date of curation|N/A|Required if known
cur_by_treat_surg|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>