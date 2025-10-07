# 🏈 Projeto de Análise de Dados da NFL (1999–2024)

## 📘 Visão Geral
Este projeto tem como objetivo explorar e analisar dados históricos da **NFL (National Football League)** utilizando ferramentas de **Ciência de Dados**.  
A base de dados foi obtida no [Kaggle](https://www.kaggle.com/datasets/philiphyde1/nfl-stats-1999-2022) e complementada com informações mais recentes (2023–2024) via biblioteca `nfl_data_py`.

O foco inicial é preparar os dados para futuras análises preditivas e descritivas, com uma separação clara entre estatísticas **ofensivas** e **defensivas** dos jogadores.

---

## 📊 Estrutura dos Dados
O dataset contém informações detalhadas sobre os jogadores da NFL entre 1999 e 2024, incluindo:

- **Dados demográficos:** idade, altura, peso, faculdade, ano de draft etc.  
- **Métricas de performance:** jardas, touchdowns, interceptações, tackles, sacks, entre outros.  
- **Indicadores de fantasy football:** pontos padrão e PPR (Point Per Reception).  

Os arquivos principais utilizados foram:

- `yearly_player_stats_offense.csv` — Estatísticas ofensivas anuais por jogador.  
- `yearly_player_stats_defense.csv` — Estatísticas defensivas anuais por jogador.  

---

## 🧹 Etapa Atual: Limpeza e Padronização dos Dados
Até o momento, foram realizadas as seguintes etapas:

1. **Leitura e separação** dos datasets ofensivo e defensivo.  
2. **Seleção de colunas relevantes** para reduzir dimensionalidade e focar nas métricas principais.  
3. **Tratamento de valores ausentes**, substituindo `NaN` por `0` (colunas numéricas) ou `"Desconhecido"` (colunas categóricas).  
4. **Correção de codificações inválidas**, como valores `"0"` na coluna `college`, substituídos por `"Desconhecido"`.  
5. **Conversão de tipos de dados** para garantir consistência (ex: `draft_round`, `draft_pick`, `years_exp`, `age`).  
6. **Separação das bases** entre **ofensiva** e **defensiva** para análises futuras independentes.  

```python
# Exemplo: filtrando colunas existentes
offense_cols = [col for col in offensive_cols if col in df_offense.columns]
df_offense_reduzido = df_offense[offense_cols]
