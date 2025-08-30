# Retinal Fundus Imaging as Biomarker for ADHD Using Machine Learning for Screening and Visual Attention Stratification

Choi H, Hong J, Kang HG, Park MH, Ha S, Lee J, Yoon S, Kim D, Park YR, Cheon KA. Retinal fundus imaging as biomarker for ADHD using machine learning for screening and visual attention stratification. NPJ Digit Med. 2025 Mar 17;8(1):164. doi: [10.1038/s41746-025-01547-9](https://doi.org/10.1038/s41746-025-01547-9). PMID: 40097590; PMCID: PMC11914053.

## 1. Fichamento de Conteúdo

O estudo examina a possibilidade de empregar imagens de fundo de olho como biomarcador não invasivo para triagem do transtorno de déficit de atenção e hiperatividade (TDAH) e para estratificar déficits de atenção executiva (FE) em crianças e adolescentes. Apoiado na relação neurobiológica entre retina e cérebro e no papel da dopamina em ambos, utiliza-se o pipeline AutoMorph para extrair automaticamente métricas neurovasculares — densidade de vasos, largura média e dimensão fractal. Em seguida, aplicaram-se quatro algoritmos de aprendizado de máquina (Random Forest, XGBoost, Extra Trees e regressão logística) para distinguir indivíduos com TDAH de controles típicos pareados por idade e sexo. A amostra incluiu 323 pares de participantes, totalizando 1 108 imagens após controle de qualidade. Para triagem de TDAH, os modelos apresentaram área sob a curva característica operacional do receptor (AUROC) entre 95,5% e 96,9%, com o XGBoost alcançando sensibilidade de 91,6% e especificidade de 92,0%. Para estratificação de subdomínios de FE, avaliada pelo Comprehensive Attention Test (CAT), observou-se AUROC superior a 80% nos domínios de atenção visual (VSA) e sustentada (SART), ao passo que o domínio auditivo (ASA) apresentou desempenho inferior. A análise de importância de variáveis por SHAP indicou densidade de vasos, largura média e dimensão fractal arterial como os principais preditores. Conclui-se que a análise de imagens de fundo de olho fornece biomarcadores objetivos e interpretáveis para apoiar a triagem de TDAH e a avaliação de déficits de atenção visual, complementando métodos clínicos convencionais.

## 2. Fichamento Bibliográfico

* *Retinal fundus imaging* é uma técnica que produz imagens bidimensionais da retina, amplamente utilizada em oftalmologia por ser rápida, não invasiva e de baixo custo (página 1).  
* *AutoMorph*: pipeline de deep learning para segmentação e quantificação de morfologia neurovascular, extraindo métricas como densidade de vasos, largura média e dimensão fractal (página 3).  
* *Random Forest (RF)* é um modelo de ensemble que combina múltiplas árvores de decisão para classificação; aplicado à distinção entre TDAH e controles típicos (página 4).  
* *XGBoost*: algoritmo de gradient boosting que ajusta sequencialmente modelos fracos para otimizar a previsão; obteve AUROC de 96,9 % no estudo (páginas 4–5).  
* *SHAP (Shapley Additive Explanations)* método de interpretação de modelos de ML que atribui valor de importância a cada característica com base na teoria dos jogos, permitindo visualizar o impacto de cada variável na predição (página 6).  
* *Comprehensive Attention Test (CAT)* teste computacional de performance contínua que avalia subdomínios de atenção (visual, auditiva, sustentada e Flanker), convertendo omissões, comissões e tempos de reação em attention quotients normalizados por idade e sexo (página 5).

## 3. Fichamento de Citações

* _"Retinal fundus photography offers noninvasive, rapid, reproducible, and cost-effective screening for structural changes"._  
* _"XGBoost model showed sensitivity of 91.6% (95% CI 89.7–93.7%) and specificity of 92.0% (95% CI 90.1–93.9%)"._  
* _"Visual selective attention and sustained attention response task domains consistently achieved AUROC values > 80% across multiple models"._  
* _"Higher vessel density, average vessel width, and arterial vessel density in Zone B were strongly associated with ADHD classification"._
* _"SHAP analysis revealed vessel density as the feature with greatest impact on model output, followed by arterial fractal dimension and average vein width"._
