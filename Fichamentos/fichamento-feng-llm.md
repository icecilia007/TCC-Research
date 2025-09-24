# Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM

Feng, Yeli. "Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM," in 2024 IEEE Conference on Artificial Intelligence (CAI), Singapore, 2024, pp. 1281-1286. doi: [10.1109/CAI59869.2024.00227](https://doi.org/10.1109/CAI59869.2024.00227)

# Fichamento 6

### 1. Fichamento de Conteúdo

O artigo estuda a Similaridade Textual Semântica (STS) em ambientes clínicos multilíngues, abordando o problema de que a maioria das análises de ponta na área ainda dependem de arquiteturas *Large Language Models* (LLM) de gerações anteriores, como o *Bidirectional Encoder Representations from Transformers* (BERT). O objetivo é avaliar o potencial de modelos fundacionais mais recentes, como o T5, e propor uma solução eficiente e escalável. A metodologia consistiu em desenvolver o método *Multi-Layer Transformer Embeddings* (MLTE), que extrai e fusiona os *embeddings* de todas as camadas do codificador do transformador (utilizando *Sentence-T5-large* como *backbone*). As características de alta dimensão resultantes são comprimidas através de cinco métricas de distância e *kernel*, e o modelo é treinado em uma arquitetura *bi-encoder* ideal para *deployment* em larga escala. Para lidar com a multiplicidade de idiomas (inglês, chinês e japonês), foi adotada uma abordagem unificada, onde os textos não ingleses foram traduzidos para o inglês antes da análise. Os resultados demonstraram que o modelo *fine-tuned* com MLTE superou trabalhos relacionados em dois dos quatro *datasets* clínicos testados, como no *dataset* EBMSASS (correlação de Pearson de 0.8879), confirmando que a exploração das múltiplas camadas e o uso do T5 de domínio geral oferecem representação semântica superior aos modelos BERT clínicos especializados, especialmente sob a restrição de velocidade de um *bi-encoder*.

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
