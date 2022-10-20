---
layout: default
title: Somatic Genomics
parent: Precision-DM 1.1.0
grand_parent: Precision-DM Versions
nav_order: 7
---

# Genomics Profile

This profile inlcudes 37 data elements to capture all information for the gene and variant as retrieved from the genomic report and processed and annotated by the bioinformatics pipelines. The "Cytogenetic Location" sub-profile (not shown here) groups the elements for the cytogenetic location of the variant detected.


| Data Element | Data Type     | Description | Terminology| Required
|:-------------|:--------------|:------------|:--------|:--------|
surg_path_id_genomic|String|The ID number from the surgical pathology report|N/A|Required
tumor_prof_case_id_genomic|String|The tumor profiling case ID|N/A|Required
gene_name_hgnc|CodeableConcept|The gene name|HGNC|Required
gene_id_hgnc_id|CodeableConcept|The gene id|HGNC|Required if known
mutation_type|CodeableConcept|Is the mutation reported as a sequence or structural alteration (amplification, deletion or fusion/rearrangement)?|Code Set|Required
structural_type|CodeableConcept|Type of structural mutation|Code Set|Required
five_prime_partner|String|5' fusion partner|N/A|Required
three_prime_partner|String|3' fusion partner|N/A|Required
fusion_breakpoint|String|Exact breakpoint or any information from NGS report|N/A|Required
genome_assembly|CodeableConcept|The genome assembly|HGNC|Required if known
cytogen_loc|String|The full cytogenetic location|N/A|Required if known
cytogen_loc_chromosome|CodeableConcept|The cytogenetic location  (chromosome) |Code Set|Required
cytogen_loc_start_pos|Integer|The cytogenetic location (start position)|N/A|Required
cytogen_loc_end_pos|Integer|The cytogenetic (end position)|N/A|Required
reference_allele|CodeableConcept|Reference Allele (A, T, C, G)|Code Set|Required
altered_allele|CodeableConcept|Altered Allele (A, T, C, G)|Code Set|Required
refseq_id|CodeableConcept|Reference sequence ID by NCBI|NCBI RefSeq|Required if known
ensembl_id|CodeableConcept|The Ensembl ID|Ensembl|Required
mutation_class|CodeableConcept|The mutation classification based on the provided codes|Code Set|Required
nucleotide_change_hgvs|CodeableConcept|The symbolic representation of a genetic structural variant reported using HGVS nomenclature (gHGVS)|HGVS|Required
cosmic|CodeableConcept|The variation ID assigned by Cosmic|COSMIC|Required
cdna_change_hgvs|String|The change in the coding DNA|N/A|Required
amino_acid_change_hgvs|CodeableConcept|The symbolic representation of an amino acid variant reported using HGVS nomenclature (pHGVS)|HGVS|Required
dbsnp|CodeableConcept|The variation ID assigned by DBSNP|NCBI dbSNP|Required
clinvar|CodeableConcept|The variation ID assigned by ClinVar|NCBI ClinVar|Required
allelic_state|CodeableConcept|The classification of allelic state using one of the five provided codes|LOINC|Required
mutation_vaf|Percentage|The allele frequency represents the incidence of a gene variant in a population|N/A|Required
cn_fold|Integer|The genomic trait involving the number of copies of a particular gene present in the genome of an individual|N/A|Required
variant_origin|CodeableConcept|The genomic class of the specimen being analyzed, for example, germline|Code Set|Required
genomics_germline_disc|Boolean|Record whether the MTB discussed the potential germline finding|N/A|Required if known
genomics_clonal_heme_disc|Boolean|Record whether the MTB discussed the potential germline finding|N/A|Required if known
variant_clin_significance|CodeableConcept|The variant clinical significance depending on pathogenicity|Code Set|Required
genomics_mtb_recs|CodeableConcept|MTB's recommendation based on the genomic findings|Code Set|Required
genomics_report_recs|CodeableConcept|The recommendation listed on NGS report|Code Set|Required
vus|Boolean|The mutation is listed as a VUS in the NGS report|N/A|Required
date_cur_genomics|Date|Date of curation|N/A|Required
cur_by_genomics|String|The name of the curator who modified the instrument|N/A|Required if known


### Notes
<em>1. This profile is repeatable and more than one records can be expected per patient</em>\
<em>2. The "Code Set" is a custom set of codes defined by the JHU Team</em>