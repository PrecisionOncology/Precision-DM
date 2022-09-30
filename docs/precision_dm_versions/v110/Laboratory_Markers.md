---
layout: default
title: Laboratory Markers
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 8
---

# Laboratory Markers Profile

This profile includes 6 data elements to represent basic information on the marker reported by the lab, including name, value, unit, and date of test.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
marker_name|String|The type of tumor marker test|N/A|Required
marker_value|Integer|The result of a tumor marker test, whose data type depends on the specific type of test|N/A|Required
marker_unit|String|The unit used in the tumor market test results|N/A|Required
marker_test_date|Date|The date of the tumor marker test|N/A|Required
date_cur_lab_markers|Date|Date of curation|N/A|Required if known
curated_by_lab_markers|String|The name of the curator who modified the instrument|N/A|Required if known


### Note
<em>1. This profile is repeatable and more than one records can be expected per patient</em>