# healthier

OBJETIVO:
Descobrir alvos com maior potencial para retardar, interromper ou reverter o envelhecimento biológico humano, com base em dados multi-ômicos e princípios sistêmicos da biologia do envelhecimento.

------------------------------------------------

DADOS:
Multi-ômicos: genoma, transcriptoma, epigenoma, metiloma, proteoma, lipidoma, metaboloma
Fases do desenvolvimento: fecundação, zigoto, blastocisto, epiblasto, gastrulação, embrião, bebê, criança, adolescente, jovem, adulto, velho
Envelhecimento: cronológico, biológico, epigenético, funcional (declínio tecidual)
Animais: humanos, primatas, camundongos, axolotes, C. elegans, peixes-zebra (comparar vias evolutivas)
Intervenções como proxy de rejuvenescimento: reprogramação epigenética ((c)iPSC, OSK, rejuvenescimento parcial), jejum, transplante de medula, exercício, metformina

Datasets: 
PhenoAge, GrimAge
MOFA+, MultiVI, TotalVI, Harmony, LIGER
Trajectory inference / pseudotime	Monocle3, Slingshot, Palantir, scVelo
SCENIC, RNA velocity, Dinâmica de metilação (EpiScanpy)
Estudos longitudinais (ex: Framingham, ROSMAP, GTEx, ENCODE, GSEs com timepoints)
RNA-seq, ATAC-seq (Assay for Transposase Accessible Chromatin sequencing), metilação (450k/EPIC), 
GTEx, Tabula Muris, HCA
DrugBank
GTEx: expressão gênica por tecido com idades humanas.
Allen Brain Atlas / BrainSpan: transcriptoma cerebral ao longo da vida.
Rejuvenation Roadmap / iPSC datasets: para efeitos da reprogramação.
idade biológica/epigenética (Monocle, ScVelo, methylation clocks)
DGIdb

------------------------------------------------

ETL:

------------------------------------------------

ANÁLISE/VISUALIZAÇÃO:

------------------------------------------------

MODELAGEM:

Output primário: regressão epigenética
Considerar: Efeito cumulativo, Mecanismos compensatórios/adaptativos (ex: aumento de colágeno e TGF-β como resposta a dano crônico, metilação que silencia danos anteriores), Hallmarks “coringa” com pesos, Mortes (taxas de morte por faixa etária) e doenças (taxa de incidência) como outputs negativos (não o envelhecimento)

feature importance (ex: SHAP, LIME)

_PYTHON (pandas, scanpy, anndata, scikit-learn, pytorch)
Weighted Gene Co-expression Network Analysis (WGCNA)
modelos bayesianos hierárquicos
regressão, causal inference ou redes bayesianas
Bayesian networks, Structural Equation Modeling (SEM), SHAP values
PCA 
trajectory inference ou latent time models

_R (Seurat, limma, edgeR, WGCNA)
limma: linear models for microarray data (analyzing microarray and RNA-seq data)
Análise de pseudotempo

Doenças relacionadas à idade como output negativo (ex: Alzheimer, câncer, sarcopenia, doenças cardiovasculares, fibrose, etc)

------------------------------------------------

AVALIAÇÃO/FEEDBACK:

-----------------------------------------------

DESENVOLVIMENTO:


---
- abordagem Multi-omics
- considerar estudos longitudinais
-considerar idade cronológica/biológica/epigenética
- considerar envelhecimento desde a fecundação, zigoto, embrionário
- considerar death rate by age como output ruim 
- considerar efeito cumulativo de coisas que podem ser menos expressas no velho mas que já se acumularam no organismo ao longo dos anos
- melhorias e adaptações (ex. Fibrose seria pra proteger)
- mecanismos compensatórios (faz algo ruim pra tentar amenizar algo pior por exemplo) 
- considerar que existem hallmarks coringa, ou seja, que fingiríamos desconhecer, para modelar o processo de envelhecimento, eles poderiam receber por exemplo pesos
- considerar a chance de doenças por idade como output ruim (exemplo cancer aumenta exponencialmente, demência aumenta e no final diminui um pouco)
- considerar resultados de experimentos (inclusive (c)iPSC)
- considerar também dados animais pois podem ter mecanismos evolutivos semelhantes aos humanos

