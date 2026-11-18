# DDFRE – Churn Prediction

## 📌 Visão Geral

Projeto de ciência de dados que prevê o **churn (cancelamento) de clientes** no setor financeiro. Esta versão cobre a **análise exploratória (EDA)** e a **modelagem preditiva** com Random Forest e XGBoost.

> O DDFRE (Data-Driven Financial & Retention Engine) é um projeto maior. Esta é a primeira etapa, e a parte de engenharia de dados está no [roadmap](#-roadmap).

![Python](https://img.shields.io/badge/python-3.10+-blue)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

---

## 🎯 Objetivos

- Entender o perfil dos clientes e os fatores associados ao churn.
- Treinar e comparar modelos de classificação (Random Forest e XGBoost).
- Identificar as variáveis que mais influenciam o cancelamento.

---

## 🔍 O que foi feito

1. **EDA:** distribuição das variáveis, valores nulos, outliers, correlações e balanceamento da variável alvo.
2. **Pré-processamento:** tratamento de nulos, encoding de categóricas e separação treino/teste.
3. **Modelagem:** Random Forest e XGBoost.
4. **Avaliação:** accuracy, precision, recall, F1-score, ROC-AUC e matriz de confusão.
5. **Interpretação:** importância das variáveis (feature importance).

---

## 📊 Resultados

| Modelo | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---|---|---|---|---|
| Random Forest | – | – | – | – | – |
| XGBoost | – | – | – | – | – |


---

## 🛠️ Tecnologias

`Python` • `Pandas` • `NumPy` • `Matplotlib` • `Seaborn` • `Scikit-Learn` • `XGBoost` • `Jupyter Notebook`

---


## ▶️ Como executar

```bash
git clone https://github.com/brenaSF/ddfre-churn-prediction.git
cd ddfre-churn-prediction

```

---

## 🗺️ Roadmap

- [x] EDA
- [x] Modelos Random Forest e XGBoost
- [ ] Pipeline de engenharia de dados (Airflow + dbt, arquitetura Medallion)
- [ ] Anonimização de PII (LGPD)
- [ ] API com FastAPI + Docker
- [ ] Dashboard (Power BI / Streamlit)
- [ ] Agente GenAI (RAG)

---

## 👩‍💻 Autora

**Brena Freitas** – Cientista de Dados Júnior
[GitHub](https://github.com/brenaSF) • [LinkedIn](#)
