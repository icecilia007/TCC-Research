# Autism Spectrum Disorder detection using variable frequency complex demodulation of the electroretinogram

Posada-Quintero, Hugo F.; Manjur, Sultan Mohammad; Hossain, Md. Billal; Marmolejo-Ramos, Fernando; Lee, Irene O.; Skuse, David H.; Thompson, Dorothy A.; Constable, Paul A. "Autism spectrum disorder detection using variable frequency complex demodulation of the electroretinogram," in Research in Autism Spectrum Disorders, vol. 109, 2023, Article 102258. doi: [10.1016/j.rasd.2023.102258](https://doi.org/10.1016/j.rasd.2023.102258)

## 1. Fichamento de Conteúdo

O artigo propõe análise em domínio tempo-frequência de sinais de *electroretinogram* (*ERG*) para detecção de *Autism Spectrum Disorder* (*ASD*) com apoio de *machine learning* (*ML*). Utilizou ERG de 217 indivíduos (71 ASD, 146 controles), obtidos em flash de 113 e 446 Troland·segundo (*Td·s*) em cada olho, processados por *discrete wavelet transform* (*DWT*) e *variable frequency complex demodulation* (*VFCDM*). Extraiu 54 descritores DWT e 56 VFCDM, além de índices tempo-domínio (tempo e amplitude de ondas a e b). Treinou diversos classificadores com validação leave-subjects-out e balanceamento por *borderline SMOTE*. O melhor modelo, com features VFCDM do olho direito em 446 Td·s, foi Random Forest: AUC=0,90; sensibilidade=0,85; especificidade=0,78. Frequências altas (80–300 Hz) mostraram-se mais discriminantes, sustentando ERG em TFS como biomarcador objetivo para ASD.

## 2. Fichamento Bibliográfico

* *Autism Spectrum Disorder* (*ASD*) (Transtorno do Espectro Autista) envolve déficits sociais, de comunicação, comportamentos repetitivos e heterogeneidade fenotípica que atrasam diagnóstico (página 2).
* *Electroretinogram* (*ERG*) (Eletroretinograma) registra atividade de fotorreceptores (onda-a), células bipolares (onda-b) e potenciais originados em células amacrina (*oscillatory potentials* - OPs) e *Photopic Negative Response* (*PhNR*), fornecendo janela ao sistema nervoso central (página 2).
* *Variable frequency complex demodulation* (*VFCDM*) (Demodulação Complexa em Frequência Variável) é técnica de alta resolução tempo-frequência que decompõe sinais em bandas de ~42 Hz, preservando amplitude e fase, superando *DWT* em resolução (página 6).
* *Machine learning* (*ML*) (Aprendizado de Máquina) aplicou modelos como Random Forest, *Support Vector Machine* (*SVM*), XGBoost, entre outros, com validação subject-wise e balanceamento por *borderline SMOTE* (página 12).
* *Troland second* (*Td·s*) (Troland·segundo) mede iluminância retiniana corrigida pela área pupilar, garantindo constância de fótons independentes do diâmetro pupilar (página 3).
* Fatores discriminantes: flash de 446 Td·s no olho direito; bandas altas (80–300 Hz) de VFCDM; *Random Forest* alcançou AUC=0,90, sensibilidade=0,85, especificidade=0,78 (página 13).

## 3. Fichamento de Citações

* _"The early diagnosis of neurodevelopmental conditions such as autism spectrum disorder (ASD), is an unmet need."_
* _"One difficulty is the identification of a biological signal that relates to the ASD phenotype. The electroretinogram waveform has been identified as a possible signal."_
* _"We propose the use of a high resolution TFS technique, namely variable frequency complex demodulation (VFCDM), to decompose the ERG waveform and build machine learning models to categorize ASD."_
* _"ML models with VFCDM features outperformed models using the DWT, achieving an AUC of 0.90 (accuracy=0.81, sensitivity=0.85, specificity=0.78)."_
* _"We found that the higher frequency range (80–300 Hz) included more relevant information for classifying ASD compared to the lower frequencies."_
* _"We also found that the stronger flash strength of 446 Td·s in the right eye provided the best classification result."_
* _"TFS analysis of the ERG waveform is a potential tool to aid in the identification of the ASD phenotype."_