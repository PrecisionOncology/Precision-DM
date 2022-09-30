---
layout: default
title: MTB Recs Followup
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 15
---

# MTB Recommendations Followup Profile

This profile includes 8 data elements to capture all the details about the MTB review (date and recommendation) and the steps taken after that. In case the MTB recommendations have been followed, it will collect the date they were enacted. When the MTB report is generated, it will be attached to this profile's implementation.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
mtb_review_date|Date|The MTB review date|N/A|Required
mtb_report|Attachment|MTB report file upload|N/A|Required
mtb_recs|CodeableConcept|One or more recommendations by MTB|Code Set|Required
mtb_follow_up|CodeableConcept|Marks the acceptance of the MTB recommendations|Code Set|Required
date_mtb_rec_enacted|Date|Date MTB recommendation was enacted|N/A|Required
time_to_impl|Decimal|The time from the initial recommendation to the enaction date (in days)|N/A|Required
date_cur_mtb_recs|Date|Date of curation|N/A|Required
cur_by_mtb_recs|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>