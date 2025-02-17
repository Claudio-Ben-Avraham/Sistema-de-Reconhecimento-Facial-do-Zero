# Sistema de Reconhecimento Facial do Zero

## Objetivo

O objetivo deste projeto é criar um sistema de reconhecimento facial utilizando as bibliotecas e frameworks estudados nas aulas. A proposta envolve o uso do framework **TensorFlow**, juntamente com outras bibliotecas que o projetista julgue necessárias, para construir um sistema que seja capaz de detectar e reconhecer múltiplas faces em uma imagem ou vídeo.

## Visão Geral

Neste projeto, desenvolveremos um sistema de **detecção e reconhecimento de faces**. O processo será dividido em duas partes principais:

1. **Detecção de Faces:** Utilizaremos uma rede treinada para detectar as faces presentes nas imagens.
2. **Reconhecimento de Faces:** Após a detecção, uma rede de classificação será usada para identificar ou classificar as faces detectadas.

O sistema será capaz de identificar mais de uma face ao mesmo tempo, conforme ilustrado na **Figura 1** abaixo, que representa o resultado esperado.

## Figura 1: Exemplo de Resultado Esperado

![Exemplo de Reconhecimento Facial](link_da_imagem_aqui)

O sistema deve ser capaz de processar imagens ou vídeos e identificar as faces presentes, destacando-as com caixas delimitadoras e associando-as a um identificador único para cada rosto.

## Requisitos

- **TensorFlow**: Para implementar e treinar as redes neurais.
- **OpenCV**: Para manipulação e processamento de imagens ou vídeos.
- **NumPy**: Para manipulação de arrays e cálculos.
- **Matplotlib**: Para exibição de imagens e gráficos.
- Outras bibliotecas podem ser utilizadas conforme a necessidade do projeto.

## Etapas do Projeto

### 1. Detecção de Faces

Utilizar uma rede neural treinada para identificar as faces nas imagens. Alguns métodos possíveis incluem:

- **Haar Cascades**: Método mais simples e rápido.
- **YOLO (You Only Look Once)**: Rede neural mais avançada e precisa para detecção de objetos, incluindo faces.
- **MTCNN (Multi-task Cascaded Convolutional Networks)**: Popular para detecção de faces.

### 2. Reconhecimento de Faces

Após a detecção, a face detectada será passada por uma rede de **classificação** para identificá-la ou associá-la a uma pessoa conhecida. Algumas abordagens comuns incluem:

- **FaceNet**: Usado para gerar embeddings faciais que podem ser comparados para reconhecimento.
- **VGGFace**: Rede neural treinada para reconhecimento facial.
- **ResNet50**: Outra arquitetura que pode ser adaptada para reconhecimento facial.

### 3. Processamento em Tempo Real (Opcional)

Se o sistema for aplicado a vídeos ou câmeras em tempo real, a detecção e reconhecimento de faces deverão ser feitas em tempo real, processando cada frame da captura de vídeo.

## Como Usar

1. **Instalar as Dependências:**

```bash
pip install tensorflow opencv-python numpy matplotlib

    Executar o Script:

Execute o script de reconhecimento facial com um vídeo ou imagem como entrada.

python reconhecimento_facial.py --input caminho/para/imagem_ou_video

    Resultado Esperado:

O programa processará a imagem ou vídeo, detectará as faces e as reconhecerá, exibindo o resultado com caixas delimitadoras e identificadores de rosto.
