# Systematic detection of co-infection and subclonal recombinants in more than 2 million global SARS-CoV-2 samples 

**Orsolya Anna Pipek, Anna Medgyes-Horváth, József Stéger, Krisztián Papp, Dávid Visontai, VEO Technical Working Group, István Csabai**

>Systematic monitoring of SARS-CoV-2 co-infection cases and assessing the risk of recombinant emergence are crucial for forecasting the milestones of viral evolution and their potential clinical impact. Here we present a comprehensive analysis of more than 2 million SARS-CoV-2 samples of the COVID-19 Data Portal to identify co-infections and traces of subclonal recombination. Co-infection was reliably present in 0.33% of the investigated cases. Two independent procedures were implemented to detect evidence of subclonal recombination. We show that sensitivity is predominantly determined by the density of defining mutations along the genome, thus we used an expanded list of disjunct defining mutations of specific variant combinations to increase statistical power. We call attention to multiple challenges rendering recombinant detection difficult and estimate artifactual chimeric sequences to be present at a minimum rate of 10%, thus facilitating the mitigation of false positives in studies exploring the recombination potential of SARS-CoV-2 in clinical samples.


This repository contains additional data files, supplementary figures and analysis pipelines for the above manuscript.

## Supplementary files

- **Supplementary Figure 1.** The number of samples with reasonable coverage of the SARS-CoV-2 genome (see the Methods of the above paper for details) assigned to different variants in the [CoVEO](https://www.covid19dataportal.org/coveo) database. [\[png\]](SuppFigures/SuppFig1.png) [\[pdf\]](SuppFigures/SuppFig1.pdf)
- **Supplementary Figure 2.** Temporal distribution of co-infection samples for variant combinations with more than 50 samples. (The same figures for the top 4 most abundant combinations are shown in Figure 1C of the main manuscript.) Prevalence curves indicate the number of [GISAID](https://gisaid.org/) samples assigned to the respective variants (binned weekly). Blue vertical lines on the bottom panels mark the collection date of co-infection samples of the given variants. Whenever the collection date was not available, the date of data upload was used as a proxy, marked with red vertical lines. [\[png\]](SuppFigures/SuppFig2.png) [\[pdf\]](SuppFigures/SuppFig2.pdf)
- **Supplementary Figure 3.** Disjunct defining mutations in [GISAID](https://gisaid.org/) samples assigned to the XD, XF and XS ’Deltacron’ (recombinant Delta and Omicron) lineages. Samples (rows) are listed by their GISAID ID, with their Pango lineage indicated in brackets. Defining mutations (columns) are coloured by their respective variant (blue for Delta and red for Omicron). Heatmap colours show whether the given sample contains the given mutation or not (dark blue: present Delta-mutation; light blue: missing Omicron-mutation; dark red: present Omicron-mutation; light red: missing Delta-mutation). Dashed vertical lines mark the recombination breakpoint range(s) for each lineage. (The same genomic regions are indicated with red shaded areas in Figure 4 of the main manuscript.) [\[png\]](SuppFigures/SuppFig3.png) [\[pdf\]](SuppFigures/SuppFig3.pdf)


- **Supplementary Table 1.** Co-infection prevalence in different [ENA](https://www.ebi.ac.uk/ena/) studies. Studies are listed in decreasing order based on the total number of their good-quality samples. Studies highlighted in grey had co-infection prevalence larger than 20%. [\[xlsx\]](SuppTables/SuppTable1.xlsx) [\[csv\]](SuppTables/SuppTable1.csv)
- **Supplementary Table 2.** List of unique variant-defining mutations used in the study. Samples presenting a ratio of at least 0.5 of unique defining mutations for at least two different variants were retained for further analysis. Prevalences indicate the percentage of [GISAID](https://gisaid.org/) samples assigned to the specific variant that had the given mutation. [\[xlsx\]](SuppTables/SuppTable2.xlsx) [\[csv\]](SuppTables/SuppTable2.csv)
- **Supplementary Table 3.** Number of unique variant-defining mutations used in the study for each investigated variant. [\[xlsx\]](SuppTables/SuppTable3.xlsx) [\[csv\]](SuppTables/SuppTable3.csv)
- **Supplementary Table 4.** Disjunct defining mutations of specific variant combinations, defined as mutations present in at least 80% of GISAID samples assigned to the given variant, while simultaneously present in less than 10% of the samples assigned to any other variant(s) of the variant combination. (Variant combinations for which no more than 10 putative co-infection samples were detected based on unique defining mutations alone (Supplementary Tables 2 and 3) are not listed.) [\[xlsx\]](SuppTables/SuppTable4.xlsx) [\[csv\]](SuppTables/SuppTable4.csv)

- [not yet uploaded] **Supplementary File 1 - analysis pipeline.** Detailed pipeline of subclonal recombination detection from allele frequency distributions at disjunct defining mutations, along with corrections for allele frequency bias and interpretation of analysis results. [\[html\]]()
- [not yet uploaded] **Supplementary File 2 - analysis pipeline.** Detailed pipeline of detecting short reads overlapping defining mutations of multiple variants and carrying signs of recombination, along with the identification of chimeric sequences and subgenomic RNA. [\[html\]]()

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

- **Additional data file 2.** List of *disjunct* defining mutations in samples where at least 50% of *disjunct* defining mutations of all variants of the sample's variant combination are present. [\[tar.gz\]](data/datafile2.tar.gz)
  -   fields:
      - `runid`: integer identifying the sample
      - `pos`: genomic position of the mutation
      - `ref`: reference allele at the genomic position
      - `alt`: alternate allele at the genomic position
      - `dp`: sequencing depths at the genomic position
      - `af`: ratio of reads supporting the alternate allele (alternate allele frequency)
      - `variant`: the mutation is a *disjunct* defining mutation of `variant`
      - `num_defmuts`: number of *disjunct* defining mutations of `variant` present in the sample
      - `num_total_markers`: total number of *disjunct* defining mutations of `variant` (in the given variant combination indicated in the `variants` column)
      - `variants`: variant combination of the sample
  - *Note:* The file only contains the *disjunct* defining mutations of those variants for each sample that are listed in the `variants` column. Defining mutations with no evidence in the sequencing data of a sample are not included.

- **Additional data file 3.** List of *disjunct* defining mutations in samples where at least 80% of *disjunct* defining mutations of all variants of the sample's variant combination are present. [\[tar.gz\]](data/datafile3.tar.gz)
  -   fields: same as for Additional data file 2. (above)

- [not yet uploaded] coinf sample meta
- [not yet uploaded] samples selected for read-level analysis
