# Neural machine translation of clinical text: an empirical investigation into multilingual pre-trained language models and transfer-learning

Han L, Gladkoff S, Erofeev G, Sorokina I, Galiano B, Nenadic G. Neural machine translation of clinical text: an empirical investigation into multilingual pre-trained language models and transfer-learning. Front Digit Health. 2024 Feb 26;6:1211564. doi: [10.3389/fdgth.2024.1211564. PMID: 38468693; PMCID: PMC10926203.](https://pubmed.ncbi.nlm.nih.gov/38468693/)

## 1. Fichamento de Conteúdo

Este trabalho investiga a aplicação de modelos de *Neural Machine Translation* (NMT) no domínio clínico com o objetivo de facilitar a transferência de conhecimento no setor da saúde e combater a disparidade digital em diferentes idiomas. O artigo compara o desempenho de três *Multilingual Pre-Trained Language Models* (MPLMs) baseados em arquitetura *transformer*, focando na tradução entre Inglês e Espanhol. Os modelos testados incluem o Marian (s-MPLM, pequeno porte), o *No Language Left Behind* (NLLB) (xL-MPLM, porte massivo) e o WMT21fb (xL-MPLM, porte massivo). A metodologia envolveu o *fine-tuning* dos modelos utilizando um *corpus* médico bilíngue,MeSpEn, de aproximadamente 250 mil pares de segmentos clínicos, para adaptar os modelos clínicos. Um ponto crucial na metodologia foi o *transfer learning* aplicado ao WMT21fb, que, por não ter o Espanhol em seu pré-treinamento, foi adaptado com o *fine-tuning* em apenas uma *epoch*, configurando um teste de transferência de conhecimento para um novo par linguístico. A avaliação foi realizada em três sub-tarefas (casos clínicos, terminologia e conceitos ontológicos) e incluiu tanto métricas automáticas (*BLEU, COMET, etc.*) quanto uma crucial avaliação humana baseada em especialistas utilizando a métrica *Human-Centric Expert-Based Post-Editing Quality Evaluation*(HOPE). Os resultados mostraram que o modelo s-MPLM Clinical-Marian superou consistentemente os modelos massivos Clinical-NLLB e Clinical-WMT21fb na avaliação humana de casos clínicos. Este achado principal sugere que, no domínio clínico, a qualidade da limpeza e o *fine-tuning* dos dados são mais importantes do que o tamanho do modelo. Ademais, o *transfer learning* com o WMT21fb provou-se eficaz, demonstrando a capacidade dos modelos massivos em acomodar um novo espaço linguístico não visto na fase de pré-treinamento, mediante *fine-tuning* suficiente.

## 2. Fichamento Bibliográfico

*   *Multilingual Pre-Trained Language Models* (MPLMs): São modelos desenvolvidos para múltiplos idiomas usando grandes volumes de dados antes de serem adaptados (*fine-tuned*) para tarefas específicas (páginas 3, 4, 11).

* *Epoch*: é uma métrica fundamental no treinamento de modelos de Machine Learning (ML), representando o número de vezes que o algoritmo de treinamento percorre o *dataset* de treinamento completo. (página 6)

*   *Transfer Learning*: É uma metodologia que permite aplicar o conhecimento adquirido por um modelo pré-treinado em um conjunto de linguagens (ou domínio) a um novo conjunto de linguagens (ou domínio) através do ajuste fino (*fine-tuning*).(páginas 1, 4, 12).

*   Métrica *Human-centric Expert-based Post-editing quality Evaluation*(HOPE): É uma métrica de avaliação de qualidade focada no esforço de pós-edição e centrada no humano, que utiliza especialistas para identificar 8 tipos de erros predefinidos, cada um com diferentes níveis de penalidade. (páginas 16, 17).

## 3. Fichamento de Citações

*   "Clinical texts and documents contain a wealth of information and knowledge in the field of healthcare, and their processing, using state-of-the-art language technology, has become very important for building intelligent systems capable of supporting healthcare and providing greater social good.".

*   "Furthermore, our expert-based human evaluations demonstrate that the small-sized pre-trained language model (PLM) wins in the clinical domain fine-tuning over the other two extra-large language models by a large margin. This finding has never been previously reported in the field.".

*   "The first finding can shed some light on the idea that in clinical domain-specific MT, it is better to do more data cleaning and fine-tuning rather than build extra large LMs.".

*   "To the best of our knowledge, our work is the first to compare small-size and extra-large MPLMs in the clinical domain of NMT.".

*   "The automated metrics deliver an illusion of measurement – they are a good tool for iterative stochastic gradient descent during training, but they do not measure quality (only some sort of similarity), are not compatible when any of the underlying factors change, provide results on a non-uniform scale even on their interval of validity, and in general are not sufficiently reliable, and may be misleading.".

*   "On the contrary, human measurement is the golden universal standard that provides the least common denominator between these scenarios.".
