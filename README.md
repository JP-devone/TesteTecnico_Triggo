
# 🛒 Olist E-commerce: Análise de Dados e Visualizações Interativas

Este projeto tem como objetivo realizar uma análise exploratória e a construção de dashboards interativos utilizando o conjunto de dados da **Olist** — um e-commerce brasileiro que opera em marketplace.

A análise foi desenvolvida no **Google Colab**, com foco em identificar padrões de comportamento de clientes, desempenho logístico e eficiência de vendedores, além de construir visualizações relevantes para a tomada de decisão.

---

## 📁 Organização do Projeto

O projeto foi dividido em cinco grandes seções no notebook:

### 🔹 1. Importação e Testes do Dataset
Carregamento das tabelas disponíveis no dataset da Olist, validações iniciais e testes com os dados brutos.

### 🔹 2. Preparação dos Dados
Limpeza, normalização e engenharia de variáveis, como tempo de entrega, aprovação, indicadores de atraso e fusão de tabelas relevantes.

### 🔹 3. Análise Exploratória de Dados (EDA)
Visualizações com **Plotly Express** e análises com **pandas** para entender o comportamento dos clientes, volume de vendas, sazonalidade, entre outros.

### 🔹 4. Solução de Problemas de Negócio
Respostas visuais e analíticas para perguntas como:
- Qual a relação entre tempo de entrega e avaliação do cliente?
- Quais os estados com maior concentração de pedidos?
- Quais os vendedores com melhor desempenho?

### 🔹 5. Visualização e Dashboards
Criação de dashboards e gráficos interativos com **Plotly** para explorar:
- Mapa de calor de pedidos por estado
- Relação entre tempo de entrega e nota de avaliação
- Ranking de vendedores por volume, nota média e tempo médio de entrega

---

## ▶️ Como Executar o Projeto

### 1. Clone este repositório:

```bash
git clone https://github.com/JP-devone/TesteTecnico_Triggo.git
```

### 2. Acesse a pasta clonada:

```bash
cd TesteTecnico_Triggo
```

### 3. Abra o arquivo `TesteTécnicoTriggo` no [Google Colab](https://colab.research.google.com/)

### 4. Baixe o dataset da Olist no Kaggle:  
🔗 [Link para o dataset no Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?resource=download&select=olist_customers_dataset.csv)

### 5. Faça o upload de todos os arquivos `.csv` do dataset para o Colab.

#### 🔼 Opção 1: Upload direto do computador

Rode o seguinte código no Colab:

```python
from google.colab import files

# Vai abrir uma janela para você selecionar os arquivos CSV do seu computador
uploaded = files.upload()
```

Depois, você pode carregar os dados com:

```python
import pandas as pd

customers = pd.read_csv('olist_customers_dataset.csv')
orders = pd.read_csv('olist_orders_dataset.csv')
# E assim por diante...
```

---

#### ☁️ Opção 2: Upload via Google Drive

1. Coloque todos os arquivos `.csv` do dataset em uma pasta no seu Google Drive.
2. Rode o código abaixo no Colab:

```python
from google.colab import drive
drive.mount('/content/drive')
```

3. Acesse os arquivos com o caminho adequado:

```python
caminho = '/content/drive/MyDrive/olist-dataset/'

customers = pd.read_csv(caminho + 'olist_customers_dataset.csv')
orders = pd.read_csv(caminho + 'olist_orders_dataset.csv')
# E os demais arquivos...
```

---

### ✅ Depois do upload

Após carregar os arquivos, continue executando o notebook seção por seção — iniciando pela parte de **Importação e Testes do Dataset**.

---

## 🏆 Principais Resultados

- **Entrega influencia a nota:** pedidos entregues dentro do prazo tendem a receber avaliações mais altas.
- **Concentração de pedidos:** estados como SP, RJ e MG lideram em volume de vendas.
- **Performance dos vendedores:** foi possível identificar os vendedores com maior volume, melhor avaliação e menor tempo de entrega, apoiando a gestão da plataforma.
- **Dashboards interativos:** visualizações criadas com Plotly facilitam a análise dinâmica dos dados.

---

## 📌 Tecnologias Utilizadas

- Python (pandas, numpy)
- Plotly Express
- Google Colab
- Jupyter Notebook
- Dataset Olist

---

## 📬 Contato

Caso tenha dúvidas ou sugestões, fique à vontade para abrir uma issue ou entrar em contato por:  
📧 joaopedrobvictor@hotmail.com
