# Analysis and Processing of Human Electroretinogram

Alaql, Abdulrahman Mohammad. "Analysis and Processing of Human Electroretinogram," Master’s Thesis, Department of Electrical Engineering, University of South Florida, 2016.

## 1. Fichamento de Conteúdo

Este trabalho apresenta uma investigação detalhada de técnicas de *digital signal processing* (*DSP*) aplicadas ao *electroretinogram* (*ERG*) humano, com foco no sinal fotópico. Após coleta em 2000 Hz, o ERG médio foi analisado em domínio do tempo (ondas a e b) e frequência (espectro de potência). Aplicou-se *short time Fourier transform* (*STFT*), *continuous wavelet transform* (*CWT*) e *discrete wavelet transform* (*DWT*) para revelar características tempo-frequência e decompor o sinal. O *DWT* permitiu extrair, sequencialmente, componentes de ondas a, b, *oscillatory potentials*, onda i e *photopic negative response*, reconstruindo o ERG com alta fidelidade. Os métodos demonstram o potencial do ERG como biomarcador para diagnóstico de condições retinianas.

## 2. Fichamento Bibliográfico

* *Electroretinogram* (*ERG*) (Eletroretinograma) é a medida da resposta elétrica da retina a flashes de luz, usada para diagnóstico de disfunções retinianas (página 10).
* *Discrete wavelet transform* (*DWT*) (Transformada Discreta de Wavelet) decompõe o ERG em sub-bandas de frequência, extraindo componentes específicos como *oscillatory potentials* e *photopic negative response* (página 40).
* *Continuous wavelet transform* (*CWT*) (Transformada Contínua de Wavelet) mapeia o ERG no domínio tempo-escala, permitindo visualizar evolução de frequências de ondas a, b, i e *photopic negative response* (página 37).
* *Short time Fourier transform* (*STFT*) (Transformada de Fourier de Tempo Curto) segmenta o ERG em janelas, oferecendo resolução tempo-frequência limitada para análise preliminar (página 35).
* Modelagem de ERG por equações de Castro fornece forma paramétrica para ondas a e b, auxiliando extração sequencial de componentes (página 41).
* Extração de componentes retinianos via DWT seguiu ordem: ondas a e b, *oscillatory potentials*, onda i, *photopic negative response*, contribuindo para a compreensão e análise de biomarcadores funcionais da retina (página 42–48).

## 3. Fichamento de Citações

* _"Electroretinagram (ERG) is the recording of electrical activity of retinal cells elicited by light stimulation, which has been widely used to help diagnose different types of retinal dysfunctions."_
* _"The ERG response signal is a short non-stationary signal that contains overlapping components. Different Digital Signal Processing techniques are investigated ... such as STFT, CWT and DWT."_
* _"The plot of the reconstructed signal and the original ERG signal shows small differences which exist mostly in peaks. The shape of the reconstructed signal matches the original one with some noticeable changes in amplitude that have a small margin of difference."_
* _"Continuous Wavelet Transform (CWT) ... offers a very detailed time-scale representation which can be approximated to a time-frequency plot ..."_
* _"Short Time Fourier Transform does not offer a specific and detailed time-frequency representation of the signal and the resolution of the plot is relatively low."_
* _"The ERG model almost matches the original signal in the early ERG response, an imperfection in the model is noticed in the implicit time of a-wave as well as the peak amplitude."_
* _"DSP techniques which are utilized ... STFT, CWT and DWT ... a comprehensive analysis showed that some techniques are more suitable than others."_