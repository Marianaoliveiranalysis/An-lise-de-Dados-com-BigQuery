# Análise-de-Dados-com-BigQuery
# 🚲 Análise de Dados do Sistema de Bicicletas Compartilhadas de Austin, Texas

Este projeto utiliza **Google Cloud BigQuery** e dados públicos do dataset  
[`bigquery-public-data.austin_bikeshare`](https://console.cloud.google.com/marketplace/product/city-of-austin/bikeshare)  
para explorar e analisar padrões de uso do sistema de bicicletas compartilhadas da cidade de **Austin, Texas**.

A análise foi desenvolvida no **Google Colab**, com integração ao **BigQuery** via `pandas-gbq`.

---

## 📌 Objetivo
O objetivo deste projeto é entender melhor o uso das bicicletas compartilhadas em Austin, fornecendo **insights de negócio** que possam ajudar na otimização da operação, como:
- Identificação das estações mais movimentadas.
- Perfil dos principais usuários.
- Tempo médio das viagens.
- Tipos de bicicletas mais utilizados.

---

## ⚙️ Etapas do Projeto

### 1️⃣ Configuração do ambiente no Google Colab
```python
!pip install pandas-gbq --quiet

import pandas as pd
from pandas_gbq import read_gbq

2️⃣ Importação dos dados com SQL

A consulta foi realizada diretamente no BigQuery utilizando a função read_gbq() para carregar os dados do dataset público.

3️⃣ Exploração e tratamento dos dados

df.describe() → estatísticas descritivas

df.info() → estrutura dos dados

df['coluna_interessante'].value_counts() → contagem de valores relevantes

4️⃣ Definição de perguntas de negócio

Para cada questão foram aplicados:

Filtros e agrupamentos (groupby, agg).

Visualizações (matplotlib, seaborn).

5️⃣ Conclusão

Resumo com os principais insights da análise.

📊 Principais Descobertas e Insights

🚉 Estações de partida mais populares

21st/Speedway @ PCL → 108.559 viagens

21st & Speedway @ PCL → 71.145 viagens

Dean Keeton/Speedway → 6.506 viagens

👉 Estratégia: aumentar a disponibilidade de bicicletas nessas áreas.

👥 Principais tipos de usuários

Student Membership → 430.347

Local365 → 389.728

U.T. Student Membership → 28.910

👉 Insight: grande adesão por estudantes e residentes locais.

⏱️ Tempo médio das viagens: ~28,7 minutos.

🚲 Tipo de bicicleta mais utilizada: clássica.

🚀 Como Executar

Acesse o Google Colab
.

Crie um novo notebook.

Instale e importe as bibliotecas necessárias.

Conecte ao BigQuery com pandas-gbq.

Rode as consultas SQL e aplique os passos da análise.

📝 Conclusão

O estudo mostra que:

A demanda se concentra em estações próximas a universidades.

O perfil de maior adesão é de estudantes e residentes locais.

Bicicletas clássicas são preferidas.

O tempo médio de uso gira em torno de meia hora, sugerindo uso para deslocamentos curtos.

Esses insights podem orientar estratégias de alocação de bicicletas, planos de assinatura direcionados e melhorias na infraestrutura para atender melhor à demanda.

👤 Autor: Mariana Rodrigues de Oliveira
📅 Ano: 2025
