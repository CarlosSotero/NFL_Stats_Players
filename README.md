# 🏈 Projeto: NFL com Dados — Análise e Clusterização de Jogadores (2012–2024)

## 📘 Sobre o Projeto
Este projeto tem como objetivo explorar e agrupar o desempenho histórico de jogadores **ofensivos e defensivos da NFL** entre as temporadas **2012 e 2024**, utilizando dados consolidados do Kaggle.

A base utilizada — [NFL Stats 1999–2022](https://www.kaggle.com/datasets/philiphyde1/nfl-stats-1999-2022) — contém estatísticas atualizadas até 2024, abrangendo jogadores, times, métricas avançadas e pontos de fantasy football.

---

## 🎯 Objetivos da Análise

- Explorar o desempenho histórico de jogadores ofensivos e defensivos;  
- Avaliar a evolução de métricas como:  
  - **QBs:** passer rating, jardas aéreas, touchdowns e interceptações;  
  - **RBs e WRs:** jardas corridas, recepções, touchdowns e eficiência;  
  - **Defesas:** tackles, sacks, interceptações e jogadas impactantes;  
- Criar **indicadores comparativos** entre jogadores e posições;  
- Aplicar **técnicas de clusterização (K-Means, PCA)** para identificar grupos de jogadores com estilos e desempenhos semelhantes;  
- Visualizar os clusters em gráficos 2D/3D e interpretar **perfis de performance**.

---

## 🤖 Etapas do Projeto

### 1. Coleta e Entendimento dos Dados
- Fonte: Kaggle (NFL Stats 2012–2024)  
- Dados ofensivos e defensivos consolidados em dataframes distintos.  
- Ampla variedade de métricas (yardas, touchdowns, interceptações, tackles, snaps, etc.)

### 2. Limpeza e Padronização
- Remoção de colunas irrelevantes e redundantes;  
- Substituição de valores nulos e inconsistentes (`college = 0 → "Desconhecido"`);  
- Conversão de colunas numéricas e categóricas para tipos adequados;  
- Filtragem de registros inconsistentes (ex: jogadores sem snaps defensivos).

### 3. Feature Engineering
Criação de novas variáveis derivadas para enriquecer as análises:
- **Ataque:** `total_yards`, `total_touchdown`, `yards_per_carry`, `yards_per_pass_attempt`, `catch_rate`  
- **Defesa:** `tackles_total`, `sack_rate`, `tackles_per_game`, `impact_plays`

### 4. Análise Exploratória (EDA)
- Visualização da evolução de touchdowns e yardas ao longo das temporadas;  
- Comparações entre posições (médias de tackles, sacks, interceptações e jogadas impactantes);  
- Identificação de outliers e padrões por posição.  

### 5. Clusterização
Fase atual do projeto:
- Aplicar **K-Means** para agrupar jogadores com base em múltiplas métricas de performance;  
- Reduzir dimensionalidade com **PCA** para visualização;  
- Analisar e nomear os clusters identificados (ex: *QBs móveis*, *WRs de posse*, *defensores playmakers*).

---

## 🔍 Tecnologias Utilizadas
- **Python 3.10+**
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn** (para K-Means, PCA e métricas de clusterização)
- **Jupyter / Google Colab**

---

## 🧩 Próximos Passos 
- Criar dashboards interativos com **Plotly** ou **Streamlit**  
- Publicar visualizações interpretativas sobre os grupos encontrados  

---

## ✍️ Autor
**Sotero**  
Cientista de Dados em formação | Apaixonado por futebol americano 🏈  
📧 Contato: [sotero.kka@gmail.com](mailto:sotero.kka@gmail.com)  
🌐 [LinkedIn](https://www.linkedin.com/in/carlos-sotero/)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)



