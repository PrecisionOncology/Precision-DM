---
layout: default
title: Outcome
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 14
---

# Outcome Profile

This profile includes 7 data elements to record information on the therapy and intervention outcome with a focus on patient's vital status with the date and cause of death. Also includes the date a patient was last seen alive and the date of the last follow-up.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
vital_status|CodeableConcept|The vital status|Code Set|Required
death_dt_full|Date|An indication that the patient is no longer living, given by a date of death or boolean|N/A|Required
last_seen_alive_date|Date|The date the patient was last seen in the clinic alive|N/A|Required
last_clinical_fup_date|Date|The date of the last follow-up|N/A|Required
cause_death|CodeableConcept|The cause of death|Code Set|Required
date_cur_outcome|Date|Date of curation|N/A|Required
cur_by_outcome|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is not repeatable and only one record is expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>