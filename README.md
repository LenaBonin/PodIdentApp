# PodIdentApp
Repository of the PodIdent app https://kidneyapp.shinyapps.io/podIdent/

PodIdent app is an R shiny application made to visualize, explore and compare data from different studies about podocytes. <br>
## The user can :
1) Compare data, in this case one has 3 possibilities : 
  - Compare them using percentiles : in this case a barcode plot is displayed for each gene under study. There should be one vertical line per dataset in which the gene is found. However, all lines might not be visible without zooming in. The position across the x-axis indicates the percentile of the gene in the corresponding dataset, while the height of the bar is equal for all datapoints.
  - Compare them using normalized fold-change and visualize it using lollipop plot : in this case there is one plot per gene under study. 
  - Compare them using normalized fold-change and visualize it using a heatmap : the closer to 1 the more red, the closer to -1 the more blue are the tiles. 0 is shown is grey and missing values in white. In order for the heatmap to be displayed, at least two genes are necessary. 

2) Plot a gene set enrichment analysis : 
The user can select one or more keyword(s) he wants to study and one or more datasets. Then an enrichment plot for each keyword/dataset combination is displayed. This plot is computed using the fgsea package (Korotkevich G, Sukhov V, Sergushichev A (2019). “Fast gene set enrichment analysis.” bioRxiv. doi: 10.1101/060012, http://biorxiv.org/content/early/2016/06/20/060012.)

3) Download the datasets : 
The user can select one dataset to download as CSV. In addition the first 10 rows of the dataset are displayed in the application. It is also possible to download directly all datasets as CSV, in that case they are downloaded in a zip file. 

## Datasets
<strong> Single-Cell Transcriptome Profiling of the Kidney Glomerulus Identifies Key Cell Types and Reactions to Injury (Chung) : </strong> <br>
Single-cell transcriptome of the glomerulus in healthy and injured-model mice.
Single-cell RNA sequencing was performed on glomeruli from healthy mice and from four different disease models, nephrotoxic serum nephritis, diabetes, doxorubicin toxicity, and CD2AP deficiency. C57BL/6J and BTBR ob/ob (BTBR.Cg-Lepob/WiscJ) mice were used. Single-cell data were processed and further analyzed by Partek Flow software (version 8.0.19.0707).<br>
https://jasn.asnjournals.org/content/31/10/2341.long <br>
https://pubmed.ncbi.nlm.nih.gov/32651223/ <br>
<br>

<strong> A Single-Cell Transcriptome Atlas of the Mouse Glomerulus (Karaiskos) : </strong> <br>
Single-cell transcriptome of the glomerulus in WT mice.
Single-cell suspensions of glomeruli were collected from 8-week-old wild-type CD1 male mice. Highly parallel single-cell transcriptome profiling was generated by Drop-seq. Single-cell data were analyzed with Drop-seq tools v. 1.124, “dropbead” and Seurat. <br>
https://jasn.asnjournals.org/content/29/8/2060.long <br>
https://pubmed.ncbi.nlm.nih.gov/29794128/ <br>
<br>

<strong> Single-cell transcriptomics of the mouse kidney reveals potential cellular targets of kidney disease (Park) : </strong> <br>
Single-cell transcriptome of the kidney in healthy mice.
Droplet-based single-cell RNA sequencing was performed on whole kidney from seven healthy male C57BL/6 mice. Single-cell data were processed and analyzed by Seurat and edgeR. <br>
https://www.science.org/doi/10.1126/science.aar2131 <br>
https://pubmed.ncbi.nlm.nih.gov/29622724/ <br>
<br>

<strong> Molecular fingerprinting of the podocyte reveals novel gene and protein regulatory networks (Boerries transcriptome) : </strong> <br>
The transcriptome of mouse podocytes.
Transcriptomic profiling of podocytes and non-podocytes were generated by Affymetrix WT Mouse Gene ST 1.0. miRNA expression profiling was acquired through ArrayStar. Podocytes and non-podocytes were isolated by FACS sorting. Gt(ROSA)26Sortm4(ACTB-tdTomato,-EGFP)Luo/J × hNPHS2Cre mice were used. Statistical analysis of transcriptomic and miRNA data was performed with R. <br>
https://www.sciencedirect.com/science/article/pii/S0085253815558626?via%3Dihub <br>
https://pubmed.ncbi.nlm.nih.gov/23364521/ <br>
<br>

<strong> Genome-Wide Analysis of Wilms’ Tumor 1-Controlled Gene Expression in Podocytes Reveals Key Regulatory Mechanisms (Kann) : </strong> <br>
The transcriptome of mouse podocytes.
CHIP-seq data were acquired from pooled samples of 6 CD-1 wild-type mice using an anti-WT1 (Wilm’s tumor suppressor 1) antibody. GFP labeled podocytes from Nphs2-Cre and R26-mTmG hybrid mice were isolated by FACS and were subject to RNA sequencing. Data were mapped through Eland and Bowtie. <br>
https://jasn.asnjournals.org/content/26/9/2097.long <br>
https://pubmed.ncbi.nlm.nih.gov/25636411/<br>
<br>

<strong> A Multi-layered Quantitative In Vivo Expression Atlas of the Podocyte Unravels Kidney Disease Candidate Genes (Rinschen and Goeddel) : </strong> <br>
The proteome and transcriptome of podocytes and non-podocyte cells in native mouse glomeruli.
Podocytes and non-podocyte fractions were isolated from glomeruli by FACS sorting. Pod.Cre x mT/mG mice were used. Podocyte and non-podocyte fractions were subjected to label-free quantitative proteomics analysis. Quantification was done via MaxQuant. <br>
https://www.sciencedirect.com/science/article/pii/S2211124718306181?via%3Dihub <br>
https://pubmed.ncbi.nlm.nih.gov/29791858/ <br>
<br>

<strong> Molecular fingerprinting of the podocyte reveals novel gene and protein regulatory networks (Boerries proteome) : </strong> <br>
The proteome of mouse podocytes.
Podocytes and non-podocytes were isolated by FACS sorting. Gt(ROSA)26Sortm4(ACTB-tdTomato,-EGFP)Luo/J × hNPHS2Cre mice were used. Podocytes and non-podocytes were subjected to SILAC and label-free proteomic quantification. Proteomic data were processed by MaxQuant. <br>
https://www.sciencedirect.com/science/article/pii/S0085253815558626?via%3Dihub <br>
https://pubmed.ncbi.nlm.nih.gov/23364521/ <br>
<br>

<strong> Tripartite Separation of Glomerular Cell Types and Proteomes from Reporter-Free Mice (CMS) : </strong> <br>
The proteome of podocytes, mesangial cells and glomerular endothelial cells in mice of three strains.
Murine mesangial, endothelial cells and podocytes were isolated by timMEP. C57BL/6, BALB/c and mT/mD mice were used. Proteomic data were searched by MaxQuant and quantified by LFQ algorithm. <br>
https://jasn.asnjournals.org/content/32/9/2175 <br>
https://pubmed.ncbi.nlm.nih.gov/34074698/ <br>
<br>


## Percentiles
For each gene in each dataset, we compute its percentile of absolute quantification. That is to say, percentile correspond to the percentage of genes in the same dataset that have an absolute quantification smaller or equal to the absolute quantification of the gene under study.

## Normalized fold-changes
In order to be able to compare all datasets together we decided to use the relative quantification variable. However, these variables differed a lot between the datasets in their amplitude. Thus, we decided to normalize them in order to get a number between -1 and 1, where -1 means completely under expressed and 1 over expressed in that dataset. <br>
To this aim, we used the fact that for a normal distribution, 99.7 % of the data lie between mean - 3 sd (lower bound) and mean + 3 sd (upper bound). For each gene, if its absolute quantification was less than the lower bound, then its normalized fold-change was set to -1, if it was greater than the upper bound, its normalized fold-change was set to 1. Otherwise, the normalized fold-change was computed as:<br>
-1+ 2*(q<sub>r</sub> - Lb)/(Ub – Lb) <br>
With: q <sub>r</sub>: relative quantity of the gene product, Lb: lower boundary, Ub: upper boundary <br>
Histograms of the normalized relative quantifications can be found in the file [Histogram_rq.pdf](Histograms_rq.pdf)<br>
<br>
In addition, before performing the normalization, we actually had to compute the log2 fold-change of single-cell datasets from the data. Indeed, for each genes, only the expressions by cell types were available. Thus, we computed the log2 of fold-change as : <br>
log2(p/(e+m) for Chung and Karaiskos single-cell, and as : log2(p/e) for Park dataset <br> With p: sum of the expression of all podocyte cells, e: sum of the expression of all endothelial cells and m: sum of the expression of all messangial cells <br>
If either p or the sum e+m were equal to 0, then the gene was remove from the dataset as it was not possible to compute its log2 fold-change. <br>

<strong> Nb : </strong> There is no relative quantification for Genome-Wide Analysis of Wilms’ Tumor 1-Controlled Gene Expression in Podocytes Reveals Key Regulatory Mechanisms (Kann) dataset. So it cannot be compared in normalized fold-change form in the app.

## Enrichment plot
In the here provided gene set enrichment analysis (GSEA, the user can define a gene set of interest by selecting an UniProtKB Keyword ( https://www.uniprot.org/keywords/ ) and investigate an eventual enrichment in a selected dataset.<br>
<br>
For this, all genes of the dataset are ranked according to the absolute quantification of their mRNA or protein product (x-axis, high – left, low – right). A rolling-sum is increased or decreased for each gene associated or not associated to the gene set (green line). The highest value reached (upper red line) is called the enrichment score (ES) and gives note about the over-all regulation of the selected gene set. In addition, black lines indicate the exact position of found genes in the ranked list. <br>
<br>
Regulated gene sets have a higher ES, as the associated genes appear close to each other in the ranked list. In addition, the position of the peak along the x-axis indicates the average expression level of the gene set. The distribution of the individual genes across the rank list of changed expression levels may offer a deeper understanding of similarly expressed clusters within the gene set, but can be disadvantageous for large gene sets(Subramanian et al., 2005). <br>

<strong> Nb : </strong> In the original publication by Subramanian et al., 2005), this analysis was used to study the correlation of gene ontology term enrichments to clinical phenotypes. For this, the strength of the increase or decrease of the rolling-sum depended on the correlation of the specific gene to the phenotype. <br>
Here, the enrichment of UniProtKB keywords is shown and an evaluation of the relevance of each individual gene for the keyword would not be possible. Thus, the rolling-sum is changed by the same value per gene and the enrichment shows the number of genes associated to the keyword.  
