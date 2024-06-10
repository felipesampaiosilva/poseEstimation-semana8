# Pose Estimation para Bovinos

Este repositório contém a implementação do pose estimation para bovinos, utilizando o dataset ANIMAL-POSE. A seguir, estão detalhadas as etapas realizadas no processo, os resultados obtidos e as conclusões pessoais.

## 1. Análise Exploratória do Dataset

O dataset ANIMAL-POSE foi obtido a partir do site oficial [Animal-Pose Dataset](https://sites.google.com/view/animal-pose/). Este dataset inclui imagens de diversos animais, com anotações para pose estimation.

### Quantidade de Imagens

Após análise do dataset, foram identificadas X imagens de bovinos, distribuídas da seguinte forma:

- **Total de Imagens**: Y imagens
- **Imagens de Bovinos**: X imagens

### Análise Gráfica

Foram gerados gráficos para visualizar a distribuição das imagens no dataset:

- **Distribuição das Imagens por Tipo de Animal**:

![Distribuição de Imagens por Tipo de Animal](distribuição.png)

### Descrição Textual

A análise exploratória revelou que o dataset é diversificado, contendo imagens de vários tipos de animais com diferentes poses. A maioria das imagens de bovinos apresenta anotações completas para a aplicação de pose estimation, o que facilita a aplicação de técnicas de visão computacional.

## 2. Filtragem e Processamento de Imagens de Bovinos

### Filtragem de Imagens

Foi realizada a filtragem do dataset para selecionar somente as imagens de bovinos. As imagens foram identificadas com base no prefixo dos nomes dos arquivos ou através das anotações específicas para bovinos.

### Etapas de Processamento

O processamento das imagens de bovinos envolveu as seguintes etapas:

1. **Carregamento da Imagem**: As imagens foram carregadas a partir dos caminhos fornecidos no dataset.
2. **Conversão para Escala de Cinza**: As imagens foram convertidas para escala de cinza para simplificar o processamento.
3. **Equalização do Histograma**: Aplicamos a equalização do histograma para melhorar o contraste da imagem.
4. **Detecção de Bordas**: Utilizamos o filtro Sobel para detectar as bordas das imagens.

#### Figura Ilustrativa

Abaixo está uma figura que ilustra o processo de processamento de imagem:

![Processamento de Imagem](processamento-bovinos.png)

#### Exemplo Detalhado Passo a Passo

1. **Carregamento da Imagem**: Uma imagem com sufixo `co` foi carregada para o sistema.
2. **Conversão para Escala de Cinza**: A imagem foi convertida para escala de cinza.
3. **Equalização do Histograma**: A equalização do histograma foi aplicada para melhorar o contraste.
4. **Detecção de Bordas**: As bordas da imagem foram detectadas utilizando o filtro Sobel.

## 3. Resultados do Processamento

### Gráficos e Tabelas

Os resultados do processamento foram resumidos em gráficos e tabelas que demonstram a eficácia das técnicas aplicadas:

![Distribuição de Imagens por Tipo de Animal](distribuição.png)


### Descrição Textual

Os resultados indicam que as técnicas de processamento aplicadas foram eficazes na detecção de poses de bovinos. A equalização do histograma melhorou significativamente a qualidade das imagens, permitindo uma detecção de bordas mais precisa.

## 4. Conclusões Pessoais

### Aprendizados

Durante este projeto, foi possível aprender sobre a importância da análise exploratória de dados e como a filtragem adequada pode facilitar o processamento subsequente. A aplicação de técnicas de processamento de imagem como equalização de histograma e detecção de bordas demonstrou ser eficaz para o problema de pose estimation.



