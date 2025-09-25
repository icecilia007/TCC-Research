# Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM

Feng, Yeli. "Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM," in 2024 IEEE Conference on Artificial Intelligence (CAI), Singapore, 2024, pp. 1281-1286. doi: [10.1109/CAI59869.2024.00227](https://doi.org/10.1109/CAI59869.2024.00227)

# Fichamento 6

### 1. Fichamento de Conteúdo

O artigo estuda a *Similaridade Textual Semântica*(STS) em ambientes clínicos multilíngues, abordando o problema de que a maioria das análises de ponta na área ainda dependem de arquiteturas de *Large Language Models* (LLM) de gerações anteriores, como o *Bidirectional Encoder Representations from Transformers* (BERT). O objetivo central do trabalho de é preencher essa lacuna, investigando o potencial de modelos fundacionais mais recentes, como o T5, e propor uma solução eficiente e escalável.

O trabalho foi conduzido seguindo uma metodologia que se baseia na arquitetura *bi-encoder*. Embora os *cross-encoders* frequentemente superem os *bi-encoders* em precisão, a abordagem *bi-encoder* é mais adequada para aplicações em larga escala (*deployment* em tempo real) onde a escalabilidade e a velocidade de inferência são cruciais, pois as sentenças são processadas independentemente.

A metodologia utilizada consistiu no desenvolvimento do método *Multi-Layer Transformer Embeddings* (MLTE), uma abordagem de fusão de características inspirada no método *Embeddings from Language Models* (ELMo). O MLTE extrai e fusiona os *embeddings* de todas as camadas do codificador do transformador (explorando os *embeddings* de *Transformer* multicamadas como um *backbone* de característica semanticamente rica). O modelo base (*backbone*) escolhido para a avaliação do MLTE foi o *Sentence-T5-large*. As características de alta dimensão resultantes da fusão (F) são subsequentemente *comprimidas* (para uma dimensão L, 5) através de cinco métricas de distância e *kernel*, que se complementam mutuamente: similaridade de cosseno, distâncias Euclidiana e Manhattan, e *kernels* Polinomial e Sigmoide. O modelo final de predição aprende um regressor ou classificador a partir dessa característica comprimida.
Para lidar com a multiplicidade de idiomas clínicos (inglês, chinês e japonês), foi adotada uma abordagem unificada de linguagem. Nesta abordagem, os textos clínicos em línguas não inglesas são traduzidos para o inglês (usando a Interface de Programação de Aplicações do Google *Translate*) antes da análise, permitindo que um único modelo LLM especializado em inglês seja implantado para análise multilíngue, o que simplifica as operações de MLOps.

O modelo *Sentence-T5-large* foi ainda submetido a um *fine-tuning* na arquitetura *bi-encoder* para maximizar o poder de representação semântica dos *embeddings*. Os resultados demonstraram que o modelo ajustado (*fine-tuned*) com MLTE (*Sentence-T5-large-ft-MLTE*) superou trabalhos relacionados em dois dos quatro *datasets* clínicos testados (BIOSSES, EBMSASS, JACSTS, CHIP-STS), como no *dataset* EBMSASS (correlação de Pearson de 0,8879), confirmando que a exploração das múltiplas camadas e o uso do T5 de domínio geral oferecem representação semântica superior aos modelos BERT clínicos especializados, especialmente sob a restrição de velocidade de um *bi-encoder*.

### 2. Fichamento Bibliográfico

*   *Semantic Textual Similarity* (STS): Uma técnica essencial em *Natural Language Processing* (NLP) que prediz a relação de similaridade entre pares de textos curtos. É fundamental para aplicações como recuperação de informação e sistemas de pergunta-resposta em ambientes clínicos e biomédicos.
*   *Large Language Models* (LLM): Modelos de linguagem de grande escala que incluem arquiteturas como BERT, T5 e GPT. O avanço recente em LLMs elevou significativamente o desempenho da análise de STS.
*   *Multi-layer Transformer Embeddings* (MLTE): O método proposto no artigo, que extrai e funde *embeddings* de múltiplas camadas de blocos codificadores *Transformer* de um LLM. Essa fusão visa criar uma característica semântica mais rica para a análise de similaridade, inspirada pelo método *Embeddings from Language Models* (ELMo).
*   *Bi-encoder*: Uma arquitetura de modelagem na qual as sentenças de um par são processadas independentemente para gerar *embeddings* que são comparados subsequentemente (e.g., usando similaridade de cosseno). Embora geralmente inferior em acurácia ao *cross-encoder*, é computacionalmente mais eficiente e adequado para aplicações em tempo real e larga escala.
*   *Cross-encoder*: Uma arquitetura que concatena um par de sentenças em uma única entrada para o modelo, permitindo que o mecanismo de atenção capture o relacionamento detalhado entre o par. Embora alcance maior acurácia, é excessivamente mais lento no tempo de inferência e intensivo em custo computacional.
*   *Abordagem Multilíngue Unificada*: Estratégia utilizada para textos clínicos não ingleses (chinês e japonês), que são traduzidos automaticamente para o inglês. Isso permite o *deployment* de um único modelo especializado em inglês, simplificando as operações de Machine Learning Operations (MLOps) em ambientes multilíngues.
## 3. Fichamento de Citações

* _"Semantic Textual Similarity (STS) analysis predicts the relationship between pairs of short texts. It is considered the most essential technique for various applications such as information retrieval, text categorization, question-answering systems."_
* _"Research in STS analysis has progressed significantly, thanks to the recent technology breakthrough in Large Language Models (LLM)."_
* _"Although cross-encoders often outperform bi-encoders in prediction accuracy, they are computationally intensive. They can be excessively slower at inference time, especially for large-scale prior knowledge retrieval."_
* _"Therefore, bi-encoders are more suitable for real-world applications when scaling and speed matter."_
* _"This paper experimentally shows that the recent advance in machine translation makes it feasible to take a language-unified approach to the STS task for the multilingual clinical text."_
* _"The semantic representation power of embeddings from BERT models fine-tuned with biomedical or clinical corpora don't naturally exhibit a performance advantage over embedding produced by more recent T5 Transformer trained for the general domain."_
