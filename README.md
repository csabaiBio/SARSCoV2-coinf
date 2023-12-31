# Systematic detection of co-infection and intra-host recombination in more than 2 million global SARS-CoV-2 samples 

**Orsolya Anna Pipek, Anna Medgyes-Horváth, József Stéger, Krisztián Papp, Dávid Visontai, Marion Koopmans, David Nieuwenhuijse, Bas B. Oude Munnink, VEO Technical Working Group, István Csabai**

>Systematic monitoring of SARS-CoV-2 co-infections between different lineages and assessing the risk of intra-host recombinant emergence are crucial for forecasting viral evolution. Here we present a comprehensive analysis of more than 2 million SARS-CoV-2 raw read datasets submitted to the European COVID-19 Data Portal to identify co-infections and intra-host recombination. Co-infection was observed in 0.35% of the investigated cases. Two independent procedures were implemented to detect intra-host recombination. We show that sensitivity is predominantly determined by the density of lineage-defining mutations along the genome, thus we used an expanded list of mutually exclusive defining mutations of specific variant combinations to increase statistical power. We call attention to multiple challenges rendering recombinant detection difficult and provide guidelines for the reduction of false positives arising from chimeric sequences produced during PCR amplification. Additionally, we identify three recombination hotspots of Delta – Omicron BA.1 intra-host recombinants. 


This repository contains additional data files, supplementary figures and analysis pipelines for the above manuscript.

## Supplementary files

- **Supplementary Figure 1.** The number of samples in the [CoVEO](https://www.covid19dataportal.org/coveo) database. **a.** The number of good-quality
SARS-CoV-2 samples with a human host assigned to different variants in the CoVEO database. **b.** The
relationship between the total number of samples assigned to a specific variant and the number of coinfection
samples containing the variant. The straight black line represents a linear dependence with a slope
of 1 on a log-log graph. R represents the Pearson-correlation coefficient, and the corresponding p-value is derived from a two-sided t-test (n=13 variants). [\[png\]](SuppFigures/SuppFig1.png) [\[pdf\]](SuppFigures/SuppFig1.pdf)
- **Supplementary Figure 2.** Temporal distribution of co-infection samples for variant combinations with more than 50 samples. (The same figures for the top 4 most abundant combinations are shown in Figure 1c of the main manuscript.) Prevalence curves indicate the number of [GISAID](https://gisaid.org/) samples assigned to the respective variants (binned weekly). Blue vertical lines on the bottom panels mark the collection date of co-infection samples of the given variants.  [\[png\]](SuppFigures/SuppFig2.png) [\[pdf\]](SuppFigures/SuppFig2.pdf)
- **Supplementary Figure 3.** Temporal distribution of co-infection samples for countries with at least 1,000 good-quality samples in the database. The top panel on each subfigure depicts the number of samples in the CoVEO database collected each week from the appropriate country. The second panel shows the collection date of co-infection samples identified in the given country. The third panel demonstrates the country-wise weekly prevalence curves of variants in the [GISAID database](https://gisaid.org/) that were included in the study. Coloured curves correspond to the most abundant variants in the whole set of detected co-infection samples (Delta, Omicron (BA.1), Alpha, Iota, Epsilon, 20E), while different shades of grey demonstrate the remaining lineages. For the United States and the United Kingdom, on the fourth panel various measures (the number of concurrently circulating lineages, the cumulative number of lineages and information entropy) of genetic diversity are plotted based on [GISAID](https://gisaid.org/) data from the given country. [\[png\]](SuppFigures/SuppFig3.png) [\[pdf\]](SuppFigures/SuppFig3.pdf)
- **Supplementary Figure 4.** Weekly co-infection rate in the function of genetic diversity. Weekly coinfection
rate was calculated as the percentage of co-infection samples out of all good-quality samples
in the given country, in the given week. Genetic diversity was either defined as the number of linages
concurrently present in the given country in the given week in [GISAID](https://gisaid.org/) data (left panels) or the
information entropy (right panels, see Methods). Only lineages investigated by the present study were
considered. Weeks for which the number of good-quality samples in the CoVEO database did not reach
10 were discarded. Each marker represents the data for a single week. Marker size corresponds to the
number of good-quality samples available. "R" and "p" indicate Pearson-correlation coefficients and respective two-sided t-test p-values (non-significant (p ≥ 0.05) results are not displayed). [\[png\]](SuppFigures/SuppFig4.png) [\[pdf\]](SuppFigures/SuppFig4.pdf)
- **Supplementary Figure 5.** Mutually exclusive defining mutations in [GISAID](https://gisaid.org/) samples assigned to the XD, XF and XS ’Deltacron’ (recombinant Delta and Omicron) lineages. Samples (rows) are listed by their GISAID ID, with their Pango lineage indicated in brackets. Defining mutations (columns) are coloured by their respective variant (blue for Delta and red for Omicron). Heatmap colours show whether the given sample contains the given mutation or not (dark blue: present Delta-mutation; light blue: missing Omicron-mutation; dark red: present Omicron-mutation; light red: missing Delta-mutation). Dashed vertical lines mark the recombination breakpoint range(s) for each lineage. (The same genomic regions are indicated with red shaded areas in Figure 4 of the main manuscript.) [\[png\]](SuppFigures/SuppFig5.png) [\[pdf\]](SuppFigures/SuppFig5.pdf)
- **Supplementary Figure 6.** Distribution of sequencing platforms and instruments within all good-quality samples
included in the study, for co-infection samples and for samples selected for downstream read-level analysis. [\[png\]](SuppFigures/SuppFig6.png) [\[pdf\]](SuppFigures/SuppFig6.pdf)
- **Supplementary Figure 7.** Schematic diagram of the workflow used to produce the data
analysed in the study. Only those steps of the [VEO variant calling pipeline](https://github.com/enasequence/covid-sequence-analysis-workflow) and features of the 
[COVID-19 Data Portal](https://www.covid19dataportal.org/) are shown that are relevant to the current
analysis. More details on both can be found in [Rahman et al. (2023)](https://www.biorxiv.org/content/biorxiv/early/2023/04/26/2023.04.19.537514.full.pdf). For the CoVEO database, only those tables and fields are displayed that were queried during data processing. Queries, codes, data files and vizualizations are uploaded to the csabaiBio/SARSCoV2-coinf github repository. Postgres, PostgreSQL and the Slonik Logo are trademarks or registered trademarks of the PostgreSQL Community Association of Canada and used with their permission. [\[png\]](SuppFigures/SuppFig7.png) [\[pdf\]](SuppFigures/SuppFig7.pdf)


- **Supplementary Data 1.** Co-infection prevalence in different [ENA](https://www.ebi.ac.uk/ena/) studies. Studies are listed in decreasing order based on the total number of their good-quality samples. Studies highlighted in grey had co-infection prevalence larger than 20%. [\[xlsx\]](SuppTables/SuppTable1.xlsx) [\[csv\]](SuppTables/SuppTable1.csv)
- **Supplementary Data 2.** List of unique variant-defining mutations used in the study. Samples presenting a ratio of at least 0.5 of unique defining mutations for at least two different variants were retained for further analysis. Prevalences indicate the percentage of [GISAID](https://gisaid.org/) samples assigned to the specific variant that had the given mutation. [\[xlsx\]](SuppTables/SuppTable2.xlsx) [\[csv\]](SuppTables/SuppTable2.csv)
- **Supplementary Data 3.** Number of unique variant-defining mutations used in the study for each investigated variant. [\[xlsx\]](SuppTables/SuppTable3.xlsx) [\[csv\]](SuppTables/SuppTable3.csv)
- **Supplementary Data 4.** Mutually exclusive defining mutations of specific variant combinations, defined as mutations present in at least 80% of GISAID samples assigned to the given variant, while simultaneously present in less than 10% of the samples assigned to any other variant(s) of the variant combination. (Variant combinations for which no more than 10 putative co-infection samples were detected based on unique defining mutations alone (Supplementary Data 2 and 3) are not listed.) [\[xlsx\]](SuppTables/SuppTable4.xlsx) [\[csv\]](SuppTables/SuppTable4.csv)


- **Supplementary Methods 1 - analysis pipeline.** PostgreSQL queries for co-infection detection using the CoVEO database. [\[html\]](pipelines/SuppFile1_coinf_pipeline.html)
  - **Contents:** In this notebook, we query the CoVEO PostgreSQL database to identify SARS-CoV-2 co-infection samples. To this end, we select samples that carry a convincing ratio of unique defining mutations of multiple variant strains. We further refine the set of samples by considering all mutually exclusive defining mutations of their variant combination, finally setting a threshold of 80% for the ratio of mutually exclusive defining mutations that have to be present in all composing variants for a sample to be deemed a co-infection case.
  - **Data files needed as input:**
      - list of mutations with lineage-specific prevalences in the GISAID database
        - [datatable](https://github.com/rvalieris/LCS/blob/master/data/pre-generated-marker-tables/pango-designation-markers-v1.9.tsv.gz) provided by [rvalieris/LCS](https://github.com/rvalieris/LCS)
        - original paper describing the data: *Valieris, R. et al. A mixture model for determining SARS-Cov-2 variant composition in pooled samples. Bioinformatics (2022) [doi:10.1093/bioinformatics/btac047.](https://academic.oup.com/bioinformatics/article/38/7/1809/6519145?login=false)*
  - **Data files generated as output:**
      - Supplementary Data 1-4.
      - Additional data files 1-4.     
- **Supplementary Methods 2 - analysis pipeline.** Allele frequency-based identification of putative co-infection samples containing trace amounts of recombinant genomes. [\[html\]](pipelines/SuppFile2_AF_pipeline.html)
  - **Contents:** In this notebook, we investigate the alternate allele frequency distributions measured in co-infection samples at the genomic positions of mutually exclusive variant-defining mutations. Our analysis reveals a systematic bias in standardized allele frequency values in samples of specific variant combinations. To detect putative recombinants based on alternate allele frequency shifts along the genome, we employ an initial hard-filtering step on co-infection samples and finally refine our results by introducing a pipeline which is aimed to correct for the above described bias in alternate allele frequency distributions in specific genomic positions. Finally, a list of putative intra-host recombinant samples is selected.
  - **Data files needed as input:** Additional data files 3 and 4
- **Supplementary Methods 3 - analysis pipeline.** Traces of read-level recombination in co-infection samples. [\[html\]](pipelines/SuppFile3_read_pipeline.html)
  - **Contents:** In this notebook, we analyse a subset of previously identified co-infection samples for the presence of short reads that overlap variant-defining mutations of both parental strains of the sample and carry both of these mutations simultaneously. We investigate how the genomic distribution of canonical lineage-specific mutations inherently affects the distribution of overlapping reads and thus the detectability of recombination breakpoints. We further examine reads carrying traces of recombination for recombination hotspots, traces of subgenomic RNA, comparability to AF-based analysis results and possible chimeric origin. As an introduction, we discuss the technical and theoretical challenges of intra-host recombinant detection.
  - **Data files needed as input:** Additional data files 3 and 5

## Additional data files

- **Additional data file 1.** List of *unique* defining mutations in samples where at least 50% of *unique* defining mutations of at least two variants were present. [\[tar.gz\]](data/datafile1.tar.gz)
  -   fields:
      - `runid`: integer identifying the sample
      - `pos`: genomic position of the mutation
      - `ref`: reference allele at the genomic position
      - `alt`: alternate allele at the genomic position
      - `dp`: sequencing depths at the genomic position
      - `af`: ratio of reads supporting the alternate allele (alternate allele frequency)
      - `variant`: the mutation is a unique defining mutation of `variant`
      - `variants`: list of variants for which at least 50% of unique defining mutations are present in the sample
  - *Note:* The file only contains the *unique* defining mutations of those variants for each sample that are listed in the `variants` column. Defining mutations with no evidence in the sequencing data of a sample are not included.

- **Additional data file 2.** List of *mutually exclusive* defining mutations in samples where at least 50% of *mutually exclusive* defining mutations of all variants of the sample's variant combination are present. [\[tar.gz\]](data/datafile2.tar.gz)
  -   fields:
      - `runid`: integer identifying the sample
      - `pos`: genomic position of the mutation
      - `ref`: reference allele at the genomic position
      - `alt`: alternate allele at the genomic position
      - `dp`: sequencing depths at the genomic position
      - `af`: ratio of reads supporting the alternate allele (alternate allele frequency)
      - `variant`: the mutation is a *mutually exclusive* defining mutation of `variant`
      - `num_defmuts`: number of *mutually exclusive* defining mutations of `variant` present in the sample
      - `num_total_markers`: total number of *mutually exclusive* defining mutations of `variant` (in the given variant combination indicated in the `variants` column)
      - `variants`: variant combination of the sample
  - *Note:* The file only contains the *mutually exclusive* defining mutations of those variants for each sample that are listed in the `variants` column. Defining mutations with no evidence in the sequencing data of a sample are not included.

- **Additional data file 3.** List of *mutually exclusive* defining mutations in samples where at least 80% of *mutually exclusive* defining mutations of all variants of the sample's variant combination are present. [\[tar.gz\]](data/datafile3.tar.gz)
  -   fields: same as for Additional data file 2. (above)

- **Additional data file 4.** [ENA accession IDs](https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html) and detailed metadata for co-infection samples. [\[tar.gz\]](data/datafile4.tar.gz)
  -   fields:
      - `runid`: integer identifying the sample (same as in the above data files)
      - `sample_accession`: ENA sample accession
      - `experiment_accession`: ENA experiment accession
      - `study_accession`: ENA study accession
      - `variants`: variant combination of the sample (sorted in alphabetic order)
      - `collection_date`: date of sample collection
      - `collection_date_valid`: boolean indicating whether the collection date was correctly provided by the uploader
      - `first_created`: date of data upload
      - `country_name`: name of the originating country
      - `instrument_platform`: sequencing platform
      - `instrument_model`: model of sequencing instrument
      - `host`: virus-host
      - `description`: string provided by the uploader describing the sample/experiment
      - `library_strategy`: library strategy used during sequencing
      - `library_selection`: technique for library selection
      - `primer_type`: name of the primer set used for amplification
      - `base_count`: total number of bases produced during sequencing
      - `estimated_n_content`: the ratio of genomic positions for which sequencing depth did not reach 10

- **Additional data file 5.** 118 co-infection samples selected for read-level analysis. [\[tar.gz\]](data/datafile5.tar.gz)
  -   fields: `runid`, `sample_accession`, `experiment_accession`, `study_accession` (same as for Additional data file 4. (above))
  -   Sample selection: The original set of previously detected 7,700 co-infection samples was first limited to those 7,290 that contained traces of exactly two variants. (I.e. samples identified as the mixtures of three or more variant strains were discarded.) Then the resulting set of samples was further downsampled to a set of 100 samples for the read-level analysis to decrease computation time and simultaneously preserve the prevalence of specific variant combinations. The 13 co-infection samples identified as putative intra-host recombinants based on alternate allele frequency (AF) shifts along their genome (see Supplementary File 1) were added to this list, along with 5 artificial mixture samples of study PRJNA827817, resulting in altogether 118 samples for read-level explorations.

