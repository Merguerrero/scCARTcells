# scCARTcells
Repository with the code for the CAR T cell multiomics project. You can find the manuscript **Integrative single-cell multi-omic analysis of clonal composition and transcriptional programs of CARneg and CD19 CARpos T cells reveals key drivers of immunotherapy response** as a preprint in [BioRxiv](https://www.biorxiv.org/content/10.1101/2024.01.23.576878v1).

In this project we analyse data from r/r B-ALL patients at the infusion product (IP) and the peak of *in vivo* expansion (peak). By FACS sorting we separated the transduced (CARpos) from the non transduced population (CARneg). Trough scRNAseq and scTCRseq we aimed to seak differences in the different timepoints and populations that could explain the clinical outcome of the patients. 

## In this repository you would find
**code for the analysis**
* 0_Doublets.qmd -> Doublet analysis 
* 0.1_KnnSmooth_CD4-8.qmd -> CD4 CD8 classification of the T cells
* 0.2_CD4CD8_DEF.qmd -> CD4 CD8 consensus classification of the T cells
* 2_AllPatients.qmd -> Exploration of the dataset, UMAPS, barplots, etc.
* 3.1_CompCluster_CAR+.qmd -> Compositional analysis with sccomp for CARpos cells
* 3.1_CompCluster_CAR-.qmd -> Compositional analysis with sccomp for CARneg cells
* 3.1_CompCluster_IP.qmd -> Compositional analysis with sccomp for IP cells
* 3.1_CompCluster_Peak.qmd -> Compositional analysis with sccomp for peak cells
* 3_DEG_Pseudobulk_CAR+.qmd -> Pseudobulk analysis for CARpos cells with DESeq2
* 3_DEG_Pseudobulk_CAR-.qmd -> Pseudobulk analysis for CARpos cells with DESeq2
* 3_DEG_Pseudobulk_IP.qmd -> Pseudobulk analysis for CARpos cells with DESeq2
* 3_DEG_Pseudobulk_PEAK.qmd -> Pseudobulk analysis for CARpos cells with DESeq2
* 4_ClusterMarkersVolcanoPiled.qmd -> Summary plot for 3_DEG_Pseudobulk analysis. (Fig S1A)
* 6_Signature_Act.qmd -> Signature exploration with Ucell
* 6_Signature_Exh_IP.qmd -> Signature exploration with Ucell
* 6_Signature_Ton.qmd -> Signature exploration with Ucell
* 7_gammadelta.qmd -> gammadelta T cell subpopulation analysis
  
**code for the figures**

| Figure | Panel | Code | Supplementary Figure | Panel | Code |
| :---:  | :---: | :--- | :---:  | :---: | :--- |
|1   | A     | [Biorender](https://www.biorender.com/)| 1   | A     |  `1_Other_Fig.qmd`  |
|1   | B     |  `1_Other_Fig.qmd`  | 1   | B     |  `2_AllPatients.qmd`  |
|1   | C     |  -  | 1   | C     |  `2_AllPatients.qmd`  |
|1   | D-I   | `2_AllPatients.qmd`  | 1   | D     |  `2_AllPatients.qmd`  |
|1   | J     | [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)| 1   | E     |  `2_AllPatients.qmd`  |
|    |       |    | 1   | F     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  |
|2   | A     |   `2_AllPatients.qmd` | 2   | A     |  `1_Other_Fig.qmd` |
|2   | B     |   `2_AllPatients.qmd` | 2   | B     |  `2_AllPatients.qmd`   |
|2   | C     |   `2_AllPatients.qmd & 3.1_CompCluster_IP.qmd` ` | 2   | C     |  `2_AllPatients.qmd`   |
|2   | D     |   `2_AllPatients.qmd` | 2   | D     |  `10_Validations.qmd`  |
|2   | E     |   `2_AllPatients.qmd` | 2   | E     |  `6_Signature_Act.qmd`  |
|2   | F     |  `3.1_CompCluster_IP.qmd`  | 2   | F     |  `6_Signature_Ton.qmd`  |
|2   | G     |  `10_Validations.qmd`  | 2   | G     |  `10_Validations.qmd`  |
|2   | H     |  `10_Validations.qmd` | 2   | H     |  `6_Signature_Exh_IP.qmd`  |
|2   | I     |  `10_Validations.qmd`  |    |      |   |
|2   | J     |  `6_Signature_Exh_IP.qmd`   |   |     |   |
|2   | K     |  `6_Signature_Exh_IP.qmd`  |   |     |   |
|2   | L     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |    |      |   |
|3   | A     |  `2_AllPatients.qmd`  | 3   | A     |  `2_AllPatients.qmd`  |
|3   | B     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | B     |  `3.1_CompCluster_CAR+.qmd & 3.1_CompCluster_CAR-.qmd`   |
|3   | C     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | C     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|3   | D     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | D     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|3   | E     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | E     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|3   | F     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | F     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|3   | G     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)  | 3   | G     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|   |      |    | 3   | H     |  [mereulab Repo](https://github.com/mereulab/CAR-T_Figures)   |
|4   | A     |  `7_gammadelta.qmd`  |    |      |   |
|4   | B     |  `7_gammadelta.qmd`  |    |      |   |
|4   | C     |  `7_gammadelta.qmd` |    |      |   |
|4   | D     |  `7_gammadelta.qmd`  |    |      |   |
|4   | E     |  `7_gammadelta.qmd`  |    |      |   |
|4   | F     |  `7_gammadelta.qmd`  |    |      |   |
|4   | G     |  `7_gammadelta.qmd`  |    |      |   |
|4   | H     |  `10_Validations.qmd`  |    |      |   |
|4   | I     |  `10_Validations.qmd`  |    |      |   |






