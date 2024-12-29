# Projeto de Transfer Learning em Python - Detecção Cachorro e Gato em Imagens

Este projeto utiliza um modelo de aprendizado de máquina para classificar imagens e detectar a probabilidade de um animal ser um **cachorro** ou um **gato**. Ele utiliza o TensorFlow para processar a imagem e realizar a previsão, além de exibir as informações visualmente na imagem com caixas delimitadoras e porcentagens.

## Funcionalidade

- O código carrega uma imagem, realiza a previsão utilizando um modelo de rede neural previamente treinado, e exibe a imagem com as caixas delimitadoras para **cachorro** e **gato**.
- As caixas são coloridas de **azul** para cachorros e **vermelho** para gatos.
- O código também exibe a porcentagem de confiança da classificação de cachorro e gato para cada imagem.

## Como Funciona

1. **Carregamento da Imagem**: O código começa carregando uma imagem do caminho especificado (`image_path`).
2. **Pré-processamento da Imagem**: A imagem é redimensionada para `160x160` e normalizada para valores no intervalo de `[0, 1]`.
3. **Predição**: O modelo realiza uma previsão para identificar a probabilidade de ser cachorro ou gato.
4. **Desenho das Caixas**: Duas caixas são desenhadas sobre a imagem:
    - **Caixa Azul** para **Cachorro**.
    - **Caixa Vermelha** para **Gato**.
5. **Exibição da Imagem**: A imagem é exibida com as caixas delimitadoras e as porcentagens de confiança.

## Como Usar

1. **Instale as Dependências**:
   Para rodar este código, você precisará ter as seguintes bibliotecas instaladas:

   - `TensorFlow`
   - `OpenCV`
   - `NumPy`
   - `Matplotlib`

   Você pode instalar essas dependências usando `pip`:

   ```bash
   pip install tensorflow opencv-python numpy matplotlib
