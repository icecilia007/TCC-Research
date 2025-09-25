# ERG Classification by Using ML Methods Based on Short-Time Fourier Transform

Albasu, Faisal B.; Kulyabin, Mikhail; Zhdanov, Aleksei; Dolganov, Anton; Borisov, Vasilii; Ronkin, Mikhail. "ERG Classification by Using ML Methods Based on Short-Time Fourier Transform," in 2024 IEEE Ural-Siberian Conference on Biomedical Engineering, Radioelectronics and Information Technology (USBEREIT), Yekaterinburg, Russia, 2024, pp. 318-321. doi: [10.1109/USBEREIT61901.2024.10583978](https://doi.org/10.1109/USBEREIT61901.2024.10583978)

## 1. Fichamento de Conteúdo

A reescrita da seção do fichamento, adicionando as informações detalhadas sobre o banco de dados e o método de análise em formato de texto corrido, é apresentada abaixo:

***

### 1. Fichamento de Conteúdo (Texto Corrido Revisado)

O artigo apresenta uma metodologia para classificação de sinais de *electroretinography* (ERG) utilizando *machine learning* (ML) baseado em *short-time Fourier transform* (STFT). O problema central é aprimorar a capacidade de classificar automaticamente os sinais ERG como saudáveis ou não saudáveis, superando as limitações da análise manual e das abordagens tradicionais de domínio do tempo ou frequência.
O estudo utiliza STFT, um método do domínio tempo-frequência, para extrair características dos sinais ERG. O banco de dados utilizado para esta investigação é um o *OculusGraphy: Ophthalmic Electrophysiological Signals Database*, um banco de dados que contém informações sobre ERG. Este banco de dados é composto por cinco tipos de sinais ERG, incluindo a resposta ERG Máxima 2.0, resposta ERG Fotópica 2.0, resposta ERG Escotópica 2.0, Potenciais Oscilatórios e resposta *Flicker* ERG Fotópica 2.0. Os sinais foram registrados seguindo o padrão *International Society for Clinical Electrophysiology of Vision* (ISCEV).
Para esta análise, foi utilizada apenas a resposta ERG máxima 2.0. O *dataset* continha 414 sinais ERG totais, sendo 340 classificados como não saudáveis e 74 como saudáveis.
A STFT converte os sinais no domínio tempo-frequência e os representa através de um espectrograma 2D. Este espectrograma é obtido utilizando uma função de janela (que possui um determinado comprimento e forma) que desliza sobre o sinal e realiza a Transformada de Fourier Rápida (FFT) em cada segmento. A extração de características (*features*) é realizada a partir deste espectrograma e inclui as intensidades mínima, máxima, mediana e média, as quais representam, respectivamente, as regiões de baixa, alta, média e amplitude média do sinal.
Essas características otimizadas são aplicadas para treinar modelos de Árvore de Decisão para a classificação binária (saudável *versus* não saudável). A pesquisa compara diferentes funções de janela (*window functions*), tamanhos de janela e sobreposições (*overlaps*) para determinar a combinação ótima na extração de características. Os resultados mostraram que a função janela *Bartlett* com tamanho 32 e sobreposição 4 produziu as características mais otimizadas, atingindo acurácia de 83%, F1-*score* de 0.91 e precisão de 0.81. A metodologia demonstra potencial considerável como biomarcador para diagnóstico de condições retinianas, contribuindo para desenvolvimento de ferramentas mais eficazes de avaliação da saúde funcional da retina.

## 2. Fichamento Bibliográfico

* *Electroretinography* (*ERG*) (Eletroretinografia) é método não invasivo de avaliação do status funcional da retina usando estimulação luminosa, com sinais de duração típica de até 250ms e faixa de frequência de 0 a 1kHz. Tipos de resposta ERG incluem *scotopic* 2.0 (baixa luminosidade, fotorreceptores bastonetes), *maximum* 2.0 (alta intensidade, cones) e *photopic* 2.0 (intensidade média, cones), cada um com características específicas de amplitude e latência (página 318 - 319).
* *Short-time Fourier transform* (*STFT*) (Transformada de Fourier de Tempo Curto) converte sinais para domínio tempo-frequência usando função janela deslizante sobre o sinal, produzindo espectrograma 2D com eixos de tempo, frequência e amplitude codificada por cores (páginas 318-319).
* Extração de características *(Feature Extraction)*  refere-se ao processo de identificar e quantificar informações importantes de um sinal ou conjunto de dados para que possam ser utilizadas por um modelo de aprendizado de máquina. Neste estudo, as características (ou *"features"*) foram extraídas dos espectrogramas e incluíram as intensidades mínima, máxima, mediana e média, que representam as regiões de baixa, alta, média e amplitude média do sinal, respectivamente (página 319).
* *Dataset* desbalanceado representa um dos principais desafios do estudo, consistindo em 414 sinais totais com 340 não-saudáveis e 74 saudáveis, o que impacta significativamente a performance dos modelos, fazendo com que eles não performem particularmente bem nas amostras minoritárias (sinais saudáveis) (páginas 319 e 320).
* *Trade-off* de resolução tempo-frequência é uma limitação inerente da STFT onde janelas mais estreitas tendem a produzir melhores resoluções temporais enquanto janelas mais largas produzem resoluções de frequência mais altas, exigindo um compromisso entre a resolução de cada domínio (páginas 320 e 321).

## 3. Fichamento de Citações

* _"ERG signals have significant potential for detecting and diagnosing a wide range of early retinal-related diseases such as diabetic retinopathies, cone and rod dystrophies, and age-related macular degenerative disorders."_
* _"Time-frequency domain analysis emerges as a comprehensive approach that allows for simultaneous examination of signals in both time and frequency domains."_
* _"This method has demonstrated its efficacy in generating valuable features for ERG classification, as evidenced by existing research findings."_
* _"In particular, the Bartlett window function with a size of 32 and an overlap of 4 was found to produce the most optimal features for the model"_
* _"This work has the potential to contribute to the development of more effective tools to assess the functional health of the retina, enhancing the diagnosis and treatment of various retinal diseases."_
* _"Initial results from this investigation have indicated that this methodology has considerable potential, but also presents several challenges, such as imbalanced datasets and the resolution trade-off."_
* _"Ultimately, this work has the potential to contribute to the development of more effective tools for assessing the functional health of the retina, enhancing the diagnosis and treatment of various retinal diseases."_
* _"The model used for the classification of signals based on the extracted features uses a decision tree algorithm implemented using the scikit-learn library to determine whether a signal is healthy or unhealthy."_
