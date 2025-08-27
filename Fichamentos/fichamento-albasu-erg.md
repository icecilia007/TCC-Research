# ERG Classification by Using ML Methods Based on Short-Time Fourier Transform

Albasu, Faisal B.; Kulyabin, Mikhail; Zhdanov, Aleksei; Dolganov, Anton; Borisov, Vasilii; Ronkin, Mikhail. "ERG Classification by Using ML Methods Based on Short-Time Fourier Transform," in 2024 IEEE Ural-Siberian Conference on Biomedical Engineering, Radioelectronics and Information Technology (USBEREIT), Yekaterinburg, Russia, 2024, ppágina 318-321. doi: [10.1109/USBEREIT61901.2024.10583978](https://doi.org/10.1109/USBEREIT61901.2024.10583978)

## 1. Fichamento de Conteúdo

O artigo apresenta uma metodologia para classificação de sinais de *electroretinography* (*ERG*) utilizando *machine learning* (*ML*) baseado em *short-time Fourier transform* (*STFT*). A *electroretinography* é um método não invasivo para avaliação funcional da retina através de estimulação luminosa, sendo útil para detecção precoce de doenças retinianas. O estudo utiliza transformada de Fourier de tempo curto para extrair características no domínio tempo-frequência de sinais ERG, aplicando essas características para treinar modelos de árvore de decisão para classificação de sinais saudáveis versus não saudáveis. A pesquisa compara diferentes funções de janela (*window functions*), tamanhos de janela e sobreposições (*overlaps*) para determinar a combinação ótima na extração de características. O *dataset* contém 414 sinais ERG de cinco tipos diferentes, sendo utilizada apenas a resposta ERG máxima 2.0, com 340 sinais não saudáveis e 74 saudáveis. Os resultados mostraram que a função janela *Bartlett* com tamanho 32 e sobreposição 4 produziu as características mais otimizadas, atingindo acurácia de 83%, F1-*score* de 0.91 e precisão de 0.81. A metodologia demonstra potencial considerável como biomarcador para diagnóstico de condições retinianas, contribuindo para desenvolvimento de ferramentas mais eficazes de avaliação da saúde funcional da retina.

## 2. Fichamento Bibliográfico

* *Electroretinography* (*ERG*) (Eletroretinografia) é método não invasivo de avaliação do status funcional da retina usando estimulação luminosa, com sinais de duração típica de até 250ms e faixa de frequência de 0 a 1kHz (página 318).
* *Short-time Fourier transform* (*STFT*) (Transformada de Fourier de Tempo Curto) converte sinais para domínio tempo-frequência usando função janela deslizante sobre o sinal, produzindo espectrograma 2D com eixos de tempo, frequência e amplitude codificada por cores (ppágina 318-319).
* *Machine learning* (*ML*) (Aprendizado de Máquina) utiliza algoritmo de árvore de decisão implementado com *scikit-learn* para classificação de sinais como saudáveis ou não saudáveis, escolhido pela natureza interpretável e capacidade com dados desbalanceados (página 319).
* Componentes ERG incluem amplitude das ondas a e b, latências, *oscillatory potentials* (OPs), *photopic negative response* e *flicker ERG response*, extraídos manualmente com assistência de clínico especializado para análise do status de saúde (página 318).
* Tipos de resposta ERG incluem *scotopic* 2.0 (baixa luminosidade, fotorreceptores bastonetes), *maximum* 2.0 (alta intensidade, cones) e *photopic* 2.0 (intensidade média, cones), cada um com características específicas de amplitude e latência (ppágina 318-319).
* Extração de características do espectrograma inclui intensidades mínima, máxima, mediana e média, representando respectivamente regiões de amplitude baixa, alta, média e média do sinal (página 319).

## 3. Fichamento de Citações

* _"ERG signals have significant potential for detecting and diagnosing a wide range of early retinal-related diseases such as diabetic retinopathies, cone and rod dystrophies, and age-related macular degenerative disorders."_
* _"Time-frequency domain analysis emerges as a comprehensive approach that allows for simultaneous examination of signals in both time and frequency domains."_
* _"This method has demonstrated its efficacy in generating valuable features for ERG classification, as evidenced by existing research findings."_
* _"The main objective of the study is to compare different window functions, sizes and overlaps in order to determine which combination yields the most optimal features for the classification of these signals."_
* _"This work has the potential to contribute to the development of more effective tools to assess the functional health of the retina, enhancing the diagnosis and treatment of various retinal diseases."_
* _"Initial results from this investigation have indicated that this methodology has considerable potential, but also presents several challenges, such as imbalanced datasets and the resolution trade-off."_
* _"Ultimately, this work has the potential to contribute to the development of more effective tools for assessing the functional health of the retina, enhancing the diagnosis and treatment of various retinal diseases."_