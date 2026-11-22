# 📊 Lab 04 — EDA e Estatística Descritiva

Projeto desenvolvido na disciplina de **Ciência de Dados**, com foco em Análise Exploratória de Dados (EDA) e Estatística Descritiva aplicadas ao dataset **Tips** (gorjetas).

---

## 📁 Estrutura do Projeto

```
CD/
└── 8784_0.ipynb   # Notebook principal com todas as questões resolvidas
```

---

## 🎯 Objetivos

Aplicar os principais conceitos de EDA para extrair insights de um conjunto de dados real, cobrindo:

- Carga e inspeção de dados
- Medidas de Tendência Central
- Medidas de Dispersão
- Visualização e detecção de outliers
- Análise de correlação bivariada

---

## � Questões Resolvidas

### Q1 — Preparação do Ambiente e Carga de Dados
- Carregamento do dataset `tips` via Seaborn
- Exibição das primeiras linhas com `.head()`
- Inspeção de tipos e valores nulos com `.info()`

### Q2 — Medidas de Tendência Central
- Cálculo de **Média**, **Mediana** e **Moda** da coluna `total_bill`
- Interpretação automática da assimetria da distribuição

### Q3 — Medidas de Dispersão
- Cálculo de **Variância** e **Desvio Padrão**
- Resumo estatístico completo com `.describe()`
- Cálculo manual do **IQR** (Intervalo Interquartil)

### Q4 — Visualização e Identificação de Outliers
- **Boxplot** com linhas de referência para média e mediana
- **Histograma com KDE** para análise da forma da distribuição
- Identificação de outliers pela regra de **1,5 × IQR** → 9 outliers encontrados

### Q5 — Análise de Correlação Bivariada
- **Correlação de Pearson** entre `total_bill` e `tip`: **r = 0,6757**
- Gráfico de dispersão com **reta de regressão** e faixa de confiança de 95%

---

## 📌 Principais Resultados

| Métrica | Valor |
|---|---|
| Média (`total_bill`) | $ 19,79 |
| Mediana (`total_bill`) | $ 17,80 |
| Desvio Padrão | $ 8,90 |
| Outliers detectados | 9 registros (acima de $ 40,30) |
| Correlação Pearson (bill × tip) | r = 0,6757 (forte positiva) |

---

## 🛠️ Tecnologias Utilizadas

| Biblioteca | Uso |
|---|---|
| `pandas` | Manipulação e análise de dados |
| `numpy` | Operações numéricas |
| `matplotlib` | Criação de gráficos |
| `seaborn` | Visualizações estatísticas |
| `jupyter` | Ambiente de execução interativa |

---

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/wjr007/lab04-eda-estatistica.git
   cd lab04-eda-estatistica
   ```

2. Instale as dependências:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Execute o notebook:
   ```bash
   jupyter notebook 8784_0.ipynb
   ```

---

## � Dataset

**Tips** — Registros de gorjetas em um restaurante americano, disponível nativamente no Seaborn.

| Coluna | Descrição |
|---|---|
| `total_bill` | Valor total da conta (USD) |
| `tip` | Valor da gorjeta (USD) |
| `sex` | Sexo do pagador |
| `smoker` | Fumante ou não |
| `day` | Dia da semana |
| `time` | Período (almoço/jantar) |
| `size` | Tamanho do grupo |
