# healthier

Target Discovery for Anti-aging Interventions

------------------------------------------------

## 00-objective

Discover targets with the greatest potential to significantly delay, interrupt or reverse human biological aging phenotypes, using (i) multi-omics, multi-tissues and multi-species data, (ii) longitudinal analysis of chronological, biological and functional aging and (iii) comparisons with experiments data (rejuvenation, e.g. partial reprogramming, iPSC; known anti-aging interventions).

------------------------------------------------

## 01-raw_data

Multi-omics: genomics, transcriptomics, epigenomics/methylomics, proteomics, lipidomics, metabolomics, etc
Multi-tissues
Multi-species (to learn from evolutionary pathways): humans, primates, mice, axolotls, C. elegans, zebrafish
Developmental/longitudinal phases: fertilization, zygote, cleavage, morula, blastula (blastocyst), gastrulation, neurula, embryo (embryonic period: up to 8 weeks), fetus (fetal period: from the 9th week until birth), newborn (neonatal), infant (baby), childhood, pre-adolescence, adolescence, youth, young adult, middle age, elderly (third age), senescence
Aging: chronological, biological (e.g. epigenetic), functional (tissue decline)
Rejuvenation experiments: epigenetic reprogramming ((c)iPSC, OSK, epigenetic partial reprogramming), fasting, marrow transplant, exercise, metformin, plasma, etc
Another anti-aging interventions

See Datasets.xlsx

------------------------------------------------

## 02-downloading_parsing_and_unifying_data

See healthier_v1.ipynb

------------------------------------------------

## 03-preprocessing_and_data_analysis

Scanpy / AnnData para dados de célula única;
MOFA+ para integrar multi-ômicas;
Monocle3 para trajetórias de diferenciação celular;
Deep Learning frameworks (ex: PyTorch, TensorFlow) para modelagem;
Bioinfokit, GSEApy, Lifelines para estatísticas e análise funcional;
Jupyter Notebook / Colab para organização e execução;

integração_multi_ômica
- considerar efeito cumulativo de coisas que podem ser menos expressas no velho mas que já se acumularam no organismo ao longo dos anos
- melhorias e adaptações (ex. Fibrose seria pra proteger)
- mecanismos compensatórios (faz algo ruim pra tentar amenizar algo pior por exemplo) 
- considerar que existem hallmarks coringa, ou seja, que fingiríamos desconhecer, para modelar o processo de envelhecimento, eles poderiam receber por exemplo pesos
- Doenças relacionadas à idade como output negativo (ex: Alzheimer, câncer, sarcopenia, doenças cardiovasculares, fibrose, etc)
- considerar a chance de doenças por idade como output ruim (exemplo cancer aumenta exponencialmente, demência aumenta e no final diminui um pouco)
death rate by age como output ruim
envelhecimento x rejuvenescimento
idade relativa à expectativa de vida

MODELING:

DNNs
Network neighbors
Causal inference
Causal graphs
Over/UnderExpression
Knockouts
Interactome
Relevance/Impact
Ordinary differential equation model
Constraint-based model
Petri net
Boolean model
Logical model
análise de expressão diferencial e redes coexpressas
Trajectory inference / pseudotime
model biological systems, simulate complex processes, and study network dynamics
Output primário: regressão epigenética
Considerar: Efeito cumulativo, Mecanismos compensatórios/adaptativos (ex: aumento de colágeno e TGF-β como resposta a dano crônico, metilação que silencia danos anteriores), Hallmarks “coringa” com pesos, Mortes (taxas de morte por faixa etária) e doenças (taxa de incidência) como outputs negativos (não o envelhecimento)

feature importance (ex: SHAP, LIME)
Construção de redes (WGCNA)
Expressão diferencial (limma, DESeq2)
Inferência de idade biológica ou pseudotempo (Monocle, methylation clocks)

_PYTHON (pandas, scanpy, anndata, scikit-learn, pytorch)
scanpy, anndata (análise de transcriptoma e single-cell)
statsmodels, scikit-learn, pandas, seaborn, matplotlib
networkx ou pyvis para redes de genes
Python (Scanpy, ScVelo, pySCENIC, pandas, sklearn)
Weighted Gene Co-expression Network Analysis (WGCNA)
modelos bayesianos hierárquicos
regressão, causal inference ou redes bayesianas
Bayesian networks, Structural Equation Modeling (SEM), SHAP values
PCA 
trajectory inference ou latent time models

_R (Seurat, limma, edgeR) 
WGCNA para redes coexpressas
R + Bioconductor (limma, DESeq2, edgeR, WGCNA)
limma: linear models for microarray data (analyzing microarray and RNA-seq data)
Análise de pseudotempo

------------------------------------------------

## 04-visualization_evaluation_feedback

interativas, dashboard, plots, redes, relatórios, share on bioRxiv

-----------------------------------------------

## 05-target_discovery

alvos prioritários

-----------------------------------------------

## 07-test_validation_development

Buscar validação funcional ou ligantes disponíveis (OpenTargets, DrugBank)
drug_targets_OpenTargets
resultados_experimentos
papers_key
resultados_chave

-----------------------------------------------

## 07-share_publish

