# Shift from acute to persistent viruses in wastewater during COVID-19 restrictions

<img width="2400" height="1800" alt="tax_tree_human_years" src="https://github.com/user-attachments/assets/eac31a95-24fb-46de-b16a-02d8610b99a3" />

Repository contains the code and data used to produce the analyses and figures in the manuscript **"Shift from acute to persistent viruses in wastewater during COVID-19 restrictions"**. Input data is a combined results table containing all samples and annotations accompanied by file describing sample metadata. Raw sequences are available at NCBI SRA, BioProject ID PRJNA1421147, with access codes SAMN55289260-SAMN55289379.



## Repository contains:
data: Data required for reproducing analyses and fiugres.
scripts: Scripts for producing the analysis and figures presented, separated by theme.
figures: Figures presented in the related mansucript.

**Data**
`Esviritu_HostDiseaseGenotypeV5.tsv`: EsViritu results with genometype, host and tropism annotations and corresponding references.

`MaAsLin3_significant_species.tsv`: Life-style and infection type annotations for significant species identified in MaAsLin3 analysis.

`Rhinovirus_cases.tsv`: Clinical case data for rhinovirus A

`sample_metadata.csv`: associated metadata for each sample

**Scripts**

`Alpha_diversity.Rmd`
Calculation of alpha diversity metrics, analyses for related metrics and producing figures Fig2B, C, D.


`Beta_diversity.Rmd`
Calculation of Bray-Curtis distance, PERMANOVA tests, figure Fig2E.


`DAA_MaAsLin3.Rmd`
MaAsLin3 analyses, figures Fig4A, B, C. Requires file MaAsLin3_significant_species_annotations.tsv as an input in addition to Esviritu_HostDiseaseGenotypeV5.ts and sample_metadata.csv.


`Overview_of_sampling_time.Rmd`
Producing figures Fig3E, F, G, H.


`Pie_plots.Rmd`
Producing figures Fig1F, G and Fig3A, B, C, D.


`Sequencing_statistics.Rmd`
Producing figures Fig1A, B, C, D and related analyses.


`Taxonomic_tree.Rmd`
Producing figures Fig1E and Fig2A.


`Rhinovirus_cases.Rmd`
Producing supplementary figure FigS1. Requires Rhinovirus_cases.csv as an input data.


`Sampling_site_map.Rmd`
Producing figure Fig5.

# Reproducing figures and analyses

1.) git clone this repo

2.) open the .Rproj file in RStudio 

3.) use renv to install the necessary libraries: renv::restore()

4.) Define appropriate _data_path_ and _output_path_ variables

5.) Run scripts in any desired order

