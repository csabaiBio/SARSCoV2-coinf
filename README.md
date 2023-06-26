# Systematic detection of co-infection and subclonal recombinants in more than 2 million global SARS-CoV-2 samples 

**Orsolya Anna Pipek, Anna Medgyes-Horváth, József Stéger, Krisztián Papp, Dávid Visontai, VEO Technical Working Group, István Csabai**

>Systematic monitoring of SARS-CoV-2 co-infection cases and assessing the risk of recombinant emergence are crucial for forecasting the milestones of viral evolution and their potential clinical impact. Here we present a comprehensive analysis of more than 2 million SARS-CoV-2 samples of the COVID-19 Data Portal to identify co-infections and traces of subclonal recombination. Co-infection was reliably present in 0.33% of the investigated cases. Two independent procedures were implemented to detect evidence of subclonal recombination. We show that sensitivity is predominantly determined by the density of defining mutations along the genome, thus we used an expanded list of disjunct defining mutations of specific variant combinations to increase statistical power. We call attention to multiple challenges rendering recombinant detection difficult and estimate artifactual chimeric sequences to be present at a minimum rate of 10%, thus facilitating the mitigation of false positives studies exploring the recombination potential of SARS-CoV-2 in clinical samples.


This repository contains additional data files, supplementary figures and analysis pipelines for the above manuscript.

## Supplementary files

- **Supplementary Figure 1.** The number of samples with reasonable coverage of the SARS-CoV-2 genome (see the Methods of the above paper for details) assigned to different variants in the [CoVEO](https://www.covid19dataportal.org/coveo) database. [\[png\]]() [\[pdf\]]()
- **Supplementary Figure 2.** Temporal distribution of co-infection samples for variant combinations with more than 50 samples. (The same figures for the top 4 most abundant combinations are shown in Figure 1C of the main manuscript.) Prevalence curves indicate the number of [GISAID](https://gisaid.org/) samples assigned to the respective variants (binned weekly). Blue vertical lines on the bottom panels mark the collection date of co-infection samples of the given variants. Whenever the collection date was not available, the date of data upload was used as a proxy, marked with red vertical lines. [\[png\]]() [\[pdf\]]()
- !!!!!!!!!!! **Supplementary Figure 3.** GISAID blabla. [\[png\]]() [\[pdf\]]()


- **Supplementary Table 1.** Co-infection prevalence in different [ENA](https://www.ebi.ac.uk/ena/) studies. Studies are listed in decreasing order based on the total number of their good-quality samples. Studies highlighted in grey had co-infection prevalence larger than 20%. [\[xlsx\]]()
- **Supplementary Table 2.** List of unique variant-defining mutations used in the study. Samples presenting a ratio of at least 0.5 of unique defining mutations for at least two different variants were retained for further analysis. Prevalences indicate the percentage of [GISAID](https://gisaid.org/) samples assigned to the specific variant that had the given mutation. [\[xlsx\]]()
- **Supplementary Table 3.** Number of unique variant-defining mutations used in the study for each investigated variant. [\[xlsx\]]()
- !!!!!!!!!!! **Supplementary Table 4.** List of disjunct variant-defining mutations considered for each variant combination. [\[xlsx\]]()

- !!!!!!!!!!! **Supplementary File 1 - analysis pipeline.** Detailed pipeline of subclonal recombination detection from allele frequency distributions at disjunct defining mutations, along with corrections for allele frequency bias and interpretation of analysis results. [\[html\]]()
- !!!!!!!!!!! **Supplementary File 2 - analysis pipeline.** Detailed pipeline of detecting short reads overlapping defining mutations of multiple variants and carrying signs of recombination, along with the identification of chimeric sequences and subgenomic RNA. [\[html\]]()

## !!!!!!!!!!! Additional data files

- list with at least 0.5 of unique muts in at least two variants
- list with at least 0.5 of disjunct muts in of all variants of the var comb
- final list of coinf sample muts
- coinf sample meta
- samples selected for read-level analysis
