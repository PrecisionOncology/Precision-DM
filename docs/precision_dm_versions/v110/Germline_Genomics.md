---
layout: default
title: Germline Genomics
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 3
---

# Germline Genomics Profile

This profile inlcudes 22 data elements to capture the results from germline testing. The "Cytogenetic Location" sub-profile (not shown here) groups the elements for the cytogenetic location of the germline variant detected.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
germ_report_case_id_genomic|String|The ID number from the germline report|N/A|Required
germ_gene_name_hgnc|CodeableConcept|The gene name|HGNC|Required
germ_gene_id_hgnc_id|CodeableConcept|The gene id|HGNC|Required if known
germ_genome_assembly|CodeableConcept|The genome assembly|HGNC|Required if known
germ_cytogen_loc|String|The full cytogenetic location|N/A|Required if known
germ_cytogen_loc_chrom|CodeableConcept|The cytogenetic location  (chromosome) |Code Set|Required
germ_cytogen_loc_start_pos|Integer|The cytogenetic location (start position)|N/A|Required
germ_cytogen_loc_end_pos|Integer|The cytogenetic (end position)|N/A|Required
germ_reference_allele|CodeableConcept|Reference Allele (A, T, C, G)|Code Set|Required
germ_altered_allele|CodeableConcept|Altered Allele (A, T, C, G)|Code Set|Required
germ_refseq_id|CodeableConcept|Range(s) of DNA sequence examined|NCBI RefSeq|Required if known
germ_ensembl_id|CodeableConcept|The Ensembl ID|Ensembl|Required if known
germ_mutation_class|CodeableConcept|The mutation classification|Code Set|Required
germ_nucleot_change_hgvs|CodeableConcept|The symbolic representation of a genetic variant reported using HGVS nomenclature (gHGVS)|HGVS|Required
germ_cdna_change_hgvs|String|The change in the coding DNA|N/A|Required
germ_aa_change_hgvs|CodeableConcept|The symbolic representation of an amino acid variant reported using HGVS nomenclature (pHGVS)|HGVS|Required
germ_dbsnp|CodeableConcept|The variation ID assigned by DBSNP|NCBI dbSNP|Required
germ_clinvar|CodeableConcept|The variation ID assigned by ClinVar|NCBI ClinVar|Required
germ_allelic_state|CodeableConcept|The classification of allelic state using one of the five provided codes|LOINC|Required
germline_variant_id|CodeableConcept|The classification of a germline variant according to pathogenicity|LOINC|Required
date_cur_germ_prof_gen|Date|Date of curation|N/A|Required if known
cur_by_germ_prof_gen|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>