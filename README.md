# Bulk-RNA-seq
In this project i will perform the bulk analysis in 3 different tissue, brain, liver and lung, to extract differentially expressed genes. I will perform this analysis without excluding rRNA, mRNA, pseudogenes and non canonical chromosomes. The aim of this work is to understand if the methods seen during lesson are robust enough to be reliable in presence of additional sources of variation. I also want to prove that this workflow is able to find meaningful differentially expressed genes between the three samples

Each replicate was checked for this QC parameters:
- RIN > 6
- % of mapped reads > 85%
- % of rRNA reads → never higher then 10%

Below the step performed:
1. Data preprocessing: This phase includes reading the count files generated from sequencing, checking the data quality, and normalizing the counts for library size and technical correction factors.
2. Dispersion estimation: The EdgeR method estimates the dispersion of the data, which represents the biological and technical variation between samples. This estimation is important for calculating appropriate test statistics for differential analysis.
3. Identification of differentially expressed genes: Using appropriate statistical models, the EdgeR method calculates the statistical significance of differential expression for each gene. Test statistics such as expression ratio between two conditions, such as fold change, and p-value or adjusted p-value values are computed to assess significance.
4. P-value adjustment: The EdgeR method utilizes the Benjamini-Hochberg p-value adjustment method or other similar methods to correct the p-values for multiple comparisons in order to control the false positive rate.
5. Interpretation of results: Once the differentially expressed genes are identified, further functional analyses can be performed to understand the biological implications of the observed expression differences.
6. Enrichment analysis: to confirm the hypothesis about biological implication, molecular function and double check the original tissues.


