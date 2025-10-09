# 🏈 Projeto: Análise de Dados da NFL (2012–2024)

## 📘 Sobre o Projeto
Este projeto tem como objetivo explorar o desempenho histórico de jogadores **ofensivos e defensivos da NFL** entre as temporadas **2012 e 2024**, utilizando dados consolidados do Kaggle.

A base utilizada — [NFL Stats 1999–2022](https://www.kaggle.com/datasets/philiphyde1/nfl-stats-1999-2022) — contém estatísticas atualizadas até **2024**, abrangendo **jogadores, times, métricas avançadas** e **pontos de fantasy football**.

Os dados foram obtidos via **KaggleHub** e combinados com informações mais recentes do pacote `nfl_data_py`, garantindo consistência e cobertura completa das últimas temporadas (2023–2024).

---

## 🎯 Objetivos

- Explorar o desempenho histórico de jogadores ofensivos e defensivos;  
- Avaliar a evolução de métricas como:
  - **QBs:** passer rating, completions, touchdowns e interceptações;  
  - **RBs e WRs:** jardas corridas, recepções, touchdowns e eficiência;  
  - **Defesas:** tackles, sacks, interceptações e pontos defensivos;  
- Criar **indicadores comparativos** entre jogadores e posições;  
- Desenvolver **análises e visualizações** para identificar padrões e tendências ao longo das temporadas;  
- Futuramente, criar **modelos de predição de performance e pontuação fantasy**.

---

## 🧹 Limpeza e Padronização

Etapas aplicadas:

1. Remoção de colunas irrelevantes e redundantes;  
2. Substituição de valores nulos por `"Desconhecido"` em campos categóricos;  
3. Correção de inconsistências (`college = 0` → `"Desconhecido"`);  
4. Conversão de colunas numéricas para tipo `int`;  
5. Exclusão de registros sem posição ou nome de jogador;  
6. Salvamento dos datasets limpos para etapas analíticas posteriores.

---

## 🧠 Feature Engineering

Criação de novas métricas para enriquecer as análises:

### 🟦 Ofensivo
- **total_yards:** jardas aéreas + jardas terrestres  
- **total_touchdowns:** touchdowns de passe + de corrida  
- **yards_per_pass_attempt:** jardas médias por tentativa de passe  
- **yards_per_carry:** jardas médias por tentativa de corrida  
- **yards_per_reception:** jardas médias por recepção  
- **catch_rate:** taxa de recepções por target  

### 🟥 Defensivo
- **tackles_total:** tackles solo + assistidos  
- **sack_rate:** taxa de sacks por snap  
- **int_rate:** taxa de interceptações por snap  
- **ff_rate:** taxa de fumbles forçados por snap  
- **tackles_per_game:** tackles por jogo  
- **impact_plays:** jogadas de impacto (sack + INT + fumble + safety + TD)  

Essas variáveis foram criadas para permitir **análises comparativas** entre posições e avaliar **eficiência individual** dos atletas.

---

## 📊 Análise Exploratória (EDA)

### ✅ **Ataque – Concluído**
Foram realizadas análises sobre o desempenho de jogadores ofensivos, explorando:
- Tendências históricas de jardas, touchdowns e eficiência por posição;   
- Identificação de outliers e jogadores de alta performance;  
- Correlação entre volume de jogo e eficiência (yards per attempt, catch rate etc.);  
- Visualizações comparativas entre posições e temporadas.

---

### 🏗️ **Defesa – Em andamento**
Etapas planejadas:
- Análise de distribuição de tackles, sacks e interceptações por posição;  
- Avaliação da evolução das defesas ao longo das temporadas;  
- Identificação de jogadores consistentes e “playmakers”;  
- Visualizações de impacto defensivo por temporada e posição.

---

## 📈 Próximos Passos

- Finalizar **EDA da defesa**;  
- Realizar **análises comparativas entre ataque e defesa**;  
- Calcular correlações com métricas de pontuação fantasy;  
- Desenvolver **modelos preditivos de performance**;  
- Criar um **dashboard interativo** com Streamlit ou Plotly.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python  
- **Bibliotecas:** pandas, numpy, nfl_data_py, matplotlib
- **Fonte de dados:** Kaggle
- **Ambiente:** Google Colab  

---

## ✍️ Autor
**Sotero**  
Cientista de Dados em formação | Apaixonado por futebol americano 🏈  
📧 Contato: sotero.kka@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/carlos-sotero/)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)



