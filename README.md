# 🏈 Projeto: Análise de Dados da NFL (2012–2024)

## 📘 Sobre o Projeto
Este projeto visa explorar o desempenho histórico de jogadores **ofensivos e defensivos da NFL** entre as temporadas **2012 e 2024**, utilizando dados consolidados do Kaggle.

A base utilizada — [NFL Stats 1999–2022](https://www.kaggle.com/datasets/philiphyde1/nfl-stats-1999-2022) — contém estatísticas atualizadas até 2024, abrangendo jogadores, times, métricas avançadas e pontos de fantasy football.

---

## 🎯 Objetivo da Análise

- Explorar o desempenho histórico de jogadores ofensivos e defensivos;
- Avaliar a evolução de métricas como:
  - **QBs:** passer rating, completions, touchdowns e interceptações;
  - **RBs e WRs:** jardas corridas, recepções, touchdowns e eficiência;
  - **Defesas:** tackles, sacks, interceptações e pontos defensivos;
- Criar indicadores comparativos entre jogadores e posições;
- Desenvolver análises e visualizações para identificar padrões e tendências ao longo das temporadas;
- Futuramente, criar **modelos de predição de performance e pontuação fantasy**.

---

## 🧹 Limpeza e Padronização

Etapas aplicadas:
1. Remoção de colunas irrelevantes e redundantes;  
2. Substituição de valores nulos por `"Desconhecido"` em campos categóricos;  
3. Correção de inconsistências (`college = 0` → `"Desconhecido"`);  
4. Conversão de colunas numéricas para tipo `int`;  
5. Salvamento dos datasets limpos para análises posteriores.

---

## ✍️ Autor
**Sotero**  
Cientista de Dados em formação | Apaixonado por futebol americano 🏈  
📧 Contato: sotero.kka@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/carlos-sotero/)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)



