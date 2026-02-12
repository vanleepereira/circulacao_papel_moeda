# 📊 Análise da Circulação de Papel-Moeda no Brasil (2020–2025)

Este projeto analisa a evolução da circulação física de papel-moeda no Brasil entre 2020 e 2025, utilizando dados públicos do Banco Central do Brasil (SGS – Sistema Gerenciador de Séries Temporais).

O objetivo é explorar tendências recentes, especialmente no contexto da pandemia e da consolidação do Pix.

---

## 📌 Objetivos

- Limpar e tratar dados da série histórica do Banco Central
- Filtrar o período 2020–2025
- Calcular a média anual da circulação de cédulas
- Visualizar a tendência com gráficos em Matplotlib
- Explorar possíveis implicações econômicas

---

## 🗂️ Fonte dos Dados

Banco Central do Brasil  
Sistema SGS  
Série: 1786  

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Scikit-Learn (exploração inicial de previsão)

---

## 🔎 Etapas do Projeto

### 1️⃣ Leitura e Tratamento dos Dados

- Conversão da coluna de data (formato brasileiro DD/MM/YYYY)
- Conversão dos valores para formato numérico
- Remoção de valores ausentes

### 2️⃣ Filtragem do Período

Seleção dos dados entre 2020 e 2025:

```python
df_filtrado = df[df['data'].dt.year.between(2020, 2025)]




