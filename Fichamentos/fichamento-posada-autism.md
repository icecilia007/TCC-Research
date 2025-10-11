# Autism Spectrum Disorder detection using variable frequency complex demodulation of the electroretinogram

Posada-Quintero, Hugo F.; Manjur, Sultan Mohammad; Hossain, Md. Billal; Marmolejo-Ramos, Fernando; Lee, Irene O.; Skuse, David H.; Thompson, Dorothy A.; Constable, Paul A. "Autism spectrum disorder detection using variable frequency complex demodulation of the electroretinogram," in Research in Autism Spectrum Disorders, vol. 109, 2023, Article 102258. doi: [10.1016/j.rTEA.2023.102258](https://doi.org/10.1016/j.rasd.2023.102258)

## 1. Fichamento de Conteúdo

O artigo propõe a validação do eletrorretinograma (ERG) como um biomarcador objetivo para o Transtorno do Espectro Autista (TEA), abordando a carência de um sinal biológico de fácil obtenção para diagnóstico precoce. O estudo empregou o ERG, considerado uma janela indireta para o sistema nervoso central, coletado de 217 indivíduos (71 TEA e 146 controles) recrutados em Londres e Adelaide. Os dados foram obtidos com o dispositivo RETeval, utilizando *flashes* em duas intensidades 113 e 446 *Troland Seconds* (Td·s). A principal inovação metodológica reside na aplicação de análise no *time-frequency spectrum* (TFS), comparando a *discrete wavelet transform* (DWT) com a técnica de alta resolução demodulação complexa de frequência variável (VFCDM). Após extrair 56 *features* do VFCDM e usar balanceamento *Borderlines Synthetic Minority Over-Sampling Technique(SMOTE)* e validação *subject-independent*, o classificador *Random Forest* alcançou o melhor desempenho, com *area under the receiver operating characteristics curve* (AUC) de 0,90, sensibilidade de 0,85 e especificidade de 0,78, na configuração de 446 Td·s no olho direito. A interpretação fisiológica dos resultados revela que as *features* mais importantes para a classificação foram encontradas na faixa de altas frequências (80–300 Hz). Esta faixa corresponde aos potenciais oscilatórios (OPs) da retina, indicando que o TEA afeta a função das células amácrinas e sugere um possível déficit na via de sinalização dopaminérgica, consolidando o VFCDM como uma ferramenta promissora para a detecção do fenótipo de TEA.

## 2. Fichamento Bibliográfico

* Transtorno do Espectro Autista (TEA) envolve déficits sociais, de comunicação, comportamentos repetitivos e heterogeneidade fenotípica que atrasam diagnóstico (página 2).
* *Electroretinogram* (*ERG*) (Eletroretinograma) registra atividade de fotorreceptores (onda-a), células bipolares (onda-b) e potenciais originados em células amacrina (*oscillatory potentials* - OPs) e *Photopic Negative Response* (*PhNR*), fornecendo janela ao sistema nervoso central (página 2).
* *Variable frequency complex demodulation* (*VFCDM*) (Demodulação Complexa em Frequência Variável) é técnica de alta resolução tempo-frequência que decompõe sinais em bandas de ~42 Hz, preservando amplitude e fase, superando *DWT* em resolução (página 6).
* *Troland second* (*Td·s*) (Troland·segundo) mede iluminância retiniana corrigida pela área pupilar, garantindo constância de fótons independentes do diâmetro pupilar (página 3).

## 3. Fichamento de Citações

* _"The early diagnosis of neurodevelopmental conditions such as autism spectrum disorder (TEA), is an unmet need."_
* _"One difficulty is the identification of a biological signal that relates to the TEA phenotype. The electroretinogram waveform has been identified as a possible signal."_
* _"ML models with VFCDM features outperformed models using the DWT, achieving an AUC of 0.90 (accuracy=0.81, sensitivity=0.85, specificity=0.78)."_
* _"We found that the higher frequency range (80–300 Hz) included more relevant information for classifying TEA compared to the lower frequencies."_
* _"We also found that the stronger flash strength of 446 Td·s in the right eye provided the best classification result."_
* _"TFS analysis of the ERG waveform is a potential tool to aid in the identification of the TEA phenotype."_
