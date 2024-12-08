# Contagem de Moedas com OpenCV e Keras em Python

Este repositório contém um exemplo de uso de um modelo Keras para detectar e classificar moedas em tempo real utilizando a captura de vídeo de uma webcam e o OpenCV. O modelo foi treinado para identificar moedas de 1 real, 25 centavos e 50 centavos. O código inclui o carregamento do modelo, o pré-processamento das imagens e a detecção de moedas nas imagens capturadas pela webcam.

### Descrição do Código

O código realiza as seguintes etapas:

1. **Carrega o modelo Keras pré-treinado**:
   Utiliza a função `load_model` do Keras para carregar o modelo treinado, que foi salvo no formato `.h5`.

2. **Captura de vídeo e pré-processamento**:
   A captura de vídeo é feita através da webcam utilizando o OpenCV. Cada frame capturado é pré-processado para detectar bordas e contornos, utilizando técnicas como desfoque e detecção de bordas com o algoritmo Canny.

3. **Detecção de moedas**:
   O código detecta os contornos das moedas na imagem, segmenta as regiões de interesse e as classifica usando o modelo Keras. As moedas são classificadas como "1 real", "25 cent" ou "50 cent" com base na previsão do modelo.

4. **Exibição do valor total**:
   O valor total das moedas detectadas é calculado e exibido em tempo real na janela de vídeo.

### Requisitos

- Python 3.10
- OpenCV
- NumPy
- Keras
- TensorFlow 2.9.1

