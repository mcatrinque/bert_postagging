# POS Tagging em Português com BERT

## Descrição do Projeto

Este projeto tem como objetivo implementar e avaliar um modelo de Part-of-Speech (POS) Tagging para a língua portuguesa utilizando o corpus Mac-Morpho e a arquitetura BERT. A tarefa de POS Tagging envolve a classificação da classe gramatical de cada palavra em um texto.

## Conjunto de Dados

O corpus Mac-Morpho, produzido pelo grupo NILC da ICMC USP, é utilizado para treinamento, validação e teste do modelo. Os dados estão disponíveis em [http://nilc.icmc.usp.br/macmorpho/macmorpho-v3.tgz](http://nilc.icmc.usp.br/macmorpho/macmorpho-v3.tgz).

## Implementação

### 1. Carregamento do Corpus

O conjunto de dados é lido a partir dos arquivos de treinamento, validação e teste utilizando a função `read_corpus`. Os dados são estruturados em um DataFrame do Pandas.

### 2. Carregamento do Tokenizer e Modelo BERT

O tokenizer e o modelo BERT pré-treinado específico para o português são carregados usando a biblioteca `transformers`. O modelo utilizado é "lisaterumi/postagger-portuguese".

### 3. Previsão de POS Tags

A função `predict_pos_tags_bert` é implementada para prever as POS tags utilizando o modelo BERT. As previsões são armazenadas para avaliação posterior.

### 4. Avaliação e Análise

A avaliação do modelo inclui cálculos de métricas como Acurácia, F1 Score, Precisão, Recall e Jaccard Score. A análise por classe gramatical fornece insights detalhados sobre o desempenho do modelo em diferentes categorias.

## Resultados e Conclusões

Os resultados destacam a eficácia do modelo BERT na tarefa de POS Tagging em português. A análise por classe gramatical permite identificar áreas de destaque e possíveis melhorias. As conclusões sugerem direções para ajustes finos e futuras explorações.

## Pré-requisitos e Instalação

- Certifique-se de ter o Python instalado (versão 3.6 ou superior).
- Instale as dependências usando `pip install -r requirements.txt`.

## Como Executar

Execute o notebook `bert_postagging.ipynb` em um ambiente Jupyter para reproduzir os resultados.
