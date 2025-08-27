# Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM

Feng, Yeli. "Semantic Textual Similarity Analysis of Clinical Text in the Era of LLM," in 2024 IEEE Conference on Artificial Intelligence (CAI), Singapore, 2024, ppágina 1281-1286. doi: [10.1109/CAI59869.2024.00227](https://doi.org/10.1109/CAI59869.2024.00227)

## 1. Fichamento de Conteúdo

O artigo investiga o potencial dos large language models (LLMs) mais recentes para análise de similaridade textual semântica (semantic textual similarity - STS) em textos clínicos. O autor propõe o método MLTE (multi-layer transformer embeddings), uma abordagem de fusão de características que aproveita embeddings de múltiplas camadas de transformers para análise de similaridade semântica. A pesquisa compara modelos LLMs pré-treinados, incluindo BERT especializados em biomedicina versus modelos T5 de domínio geral, demonstrando que o Sentence-T5-large superou consistentemente modelos BERT especializados quando utilizados como bi-encoders. O método MLTE foi avaliado em quatro datasets clínicos multilíngues: BIOSSES (inglês), EBMSASS (inglês), JACSTS (japonês) e CHIP-STS (chinês). Os resultados mostraram que o método Sentence-T5-large-ft-MLTE alcançou correlação de Pearson de 0.9248 no BIOSSES, 0.8879 no EBMSASS, 0.8652 no JACSTS e F1-score macro de 0.8527 no CHIP-STS. O estudo também propõe uma abordagem unificada por idioma usando tradução automática, permitindo uso de modelo único em inglês para múltiplos idiomas, questionando a necessidade de LLMs clínicos especializados para cada idioma.

## 2. Fichamento Bibliográfico

* *Semantic textual similarity* (*STS*) (Similaridade Textual Semântica) é técnica essencial que prediz relacionamentos entre pares de textos curtos, sendo fundamental para recuperação de informação, categorização de texto e sistemas de pergunta-resposta em *NLP* clínico (página 1281).
* *Multi-layer transformer embeddings* (*MLTE*) (Embeddings de Transformer Multicamadas) extraem características de todas as camadas de blocos codificadores do *LLM*, fusionando-as em característica de entrada para análise semântica mais rica, inspirado no método *ELMo* (ppágina 1283-1284).
* *Large language models* (*LLMs*) (Modelos de Linguagem de Grande Escala) incluem *BERT*, *T5* e *GPT*, sendo que modelos *T5* de domínio geral demonstraram melhor desempenho que modelos *BERT* especializados em biomedicina quando usados como *bi-encoders* (ppágina 1284-1285).
* *Bi-encoder* versus *cross-encoder* representam diferentes paradigmas arquiteturais, onde *bi-encoders* processam sentenças independentemente sendo mais adequados para aplicações em tempo real, enquanto *cross-encoders* concatenam pares de sentenças mas são computacionalmente intensivos (página 1282).
* Abordagem unificada por idioma utiliza tradução automática para converter textos não ingleses para inglês, permitindo uso de modelo único especializado em inglês para *MLOps* multilíngue, simplificando deployment (ppágina 1283-1284).
* Métricas de avaliação incluem correlação de *Pearson* e *Spearman* para tarefas de regressão de similaridade, e acurácia com F1-*score* macro para classificação binária de similaridade/diferença (página 1284).

## 3. Fichamento de Citações

* _"Semantic Textual Similarity (STS) analysis predicts the relationship between pairs of short texts. It is considered the most essential technique for various applications such as information retrieval, text categorization, question-answering systems."_
* _"Research in STS analysis has progressed significantly, thanks to the recent technology breakthrough in Large Language Models (LLM)."_
* _"Although cross-encoders often outperform bi-encoders in prediction accuracy, they are computationally intensive. They can be excessively slower at inference time, especially for large-scale prior knowledge retrieval."_
* _"This paper proposes a new method that exploits LLM's multi-layer Transformer embeddings as semantic-rich feature backbone and pairwise distances and kernel metrics for feature compression."_
* _"This paper experimentally shows that the recent advance in machine translation makes it feasible to take a language-unified approach to the STS task for the multilingual clinical text."_
* _"The semantic representation power of embeddings from BERT models fine-tuned with biomedical or clinical corpora don't naturally exhibit a performance advantage over embedding produced by more recent T5 Transformer trained for the general domain."_
* _"Experimental outcomes showed that the proposed method is competitive and outperformed related works over two out of four datasets."_