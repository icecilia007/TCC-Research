# Feature Extraction Methods for Electroretinogram Signal Analysis: A Review

Behbahani, Soroor; Ahmadieh, Hamid; Rajan, Sreeraman. "Feature Extraction Methods for Electroretinogram Signal Analysis: A Review," IEEE Access, vol. 9, pp. 116879-116897, 2021. doi: [10.1109/ACCESS.2021.3103848](https://doi.org/10.1109/ACCESS.2021.3103848)

## 1. Fichamento de Conteúdo

Este artigo apresenta uma revisão abrangente dos métodos de extração de características para análise de sinais de *electroretinogram* (*ERG*), sendo o primeiro trabalho de revisão sobre métodos de extração de características especificamente para sinais ERG humanos. A *electroretinography* é a resposta elétrica de diferentes células retinianas à luz e escuridão, incluindo fotorreceptores (bastonetes e cones), células bipolares, amacrínicas, ganglionares e células de Müller. O estudo categoriza os métodos em quatro domínios: análise no domínio do tempo (amplitudes e tempos implícitos tradicionais), domínio da frequência (*fast Fourier transform*, *power spectral density*, *linear prediction*), domínio tempo-frequência (*short-time Fourier transform*, *wavelet analysis*, *matching pursuit*) e métodos não-lineares e caóticos (*approximate entropy*, *Hurst exponent*, *largest Lyapunov exponent*, *Higuchi fractal dimension*). A revisão analisou 12 artigos sobre análise no domínio da frequência, mais de 25 trabalhos sobre domínio tempo-frequência e apenas 6 estudos sobre métodos não-lineares em ERG humano. Os resultados mostram que métodos de domínio da frequência e tempo-frequência superam consistentemente os parâmetros tradicionais do domínio do tempo, sendo a *wavelet analysis* particularmente eficaz para sinais ERG devido à sua capacidade de analisar sinais não-estacionários com diferentes resoluções tempo-frequência. O trabalho destaca que não existe um método universal para todos os tipos de doenças retinianas, sugerindo que combinações de métodos podem ser mais eficazes como biomarcadores para diagnóstico.

## 2. Fichamento Bibliográfico

* *Electroretinogram* (*ERG*) (Eletroretinograma) é sinal elétrico de curta duração (tipicamente 200 ms) que registra a resposta de células retinianas à estimulação luminosa, contendo componentes como ondas a, b, i-*wave*, *photopic negative response* e *oscillatory potentials* (p. 116879-116880).
* *Wavelet analysis* (*WA*) (Análise Wavelet) inclui *continuous wavelet transform* (*CWT*) e *discrete wavelet transform* (*DWT*), sendo superior ao *STFT* por fornecer melhor resolução em frequência para baixas frequências e melhor resolução temporal para altas frequências (pp. 116883-116887).
* Métodos não-lineares incluem *approximate entropy* (*ApEn*), *Hurst exponent* (*HE*), *largest Lyapunov exponent* (*LLE*) e *Higuchi fractal dimension* (*HFD*) para caracterizar comportamento caótico e complexidade de sinais ERG (pp. 116888-116890).
* *International Society for Clinical Electrophysiology of Vision* (*ISCEV*) estabeleceu protocolo padrão com seis tipos de resposta ERG baseados em diferentes estados de adaptação ao claro/escuro e intensidades de flash (p. 116880).
* Análise no domínio da frequência utiliza *fast Fourier transform* (*FFT*), *power spectral density* (*PSD*) e *linear prediction* (*LP*), sendo mais adequada para componentes de alta frequência como *oscillatory potentials* (80-160 Hz) (pp. 116881-116882).
* Extração de características tradicionais no domínio do tempo mede amplitudes e tempos implícitos das ondas a e b, mas é sensível a ruído e pode não capturar informações sutis de disfunções retinianas (p. 116880).

## 3. Fichamento de Citações

* _"Feature extraction methods often extract the intrinsic characteristics of these signals. Extracted features often be used to develop methods that can provide an accurate diagnosis of the underlying pathology."_
* _"ERG signal involves recording retinal cells' electrical activity after stimulation, which is widely used to detect different retinal layers' functions."_
* _"The ERG signal is a short signal that contains many components working at the same time. The short length of ERG and its complex nature and nonlinear dynamics make it challenging to select an appropriate analysis method."_
* _"Most papers showed the superiority of frequency-domain and time-frequency methods over the time-domain parameters used for ERG analysis."_
* _"Given the complex characteristics of ERG signals, the nonlinear and chaotic methods that illustrate the system's complexity are suitable for thoroughly analyzing and distinguishing between retinal layer performances."_
* _"Due to diversity in the retinal layers and differences in the cell's function, a single universal feature extraction approach may not be possible. In some cases, a combination of methods might be a better choice."_
* _"Nonlinear methods do not require windowing and therefore are devoid of such limitations. However, the computational requirements of nonlinear methods may be higher than the linear methods."_