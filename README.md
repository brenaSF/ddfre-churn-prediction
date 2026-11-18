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

| Modelo | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---|---|---|---|---|
| Random Forest | **0.8685** | **0.7642** | 0.4784 | 0.5884 | 0.7211 |
| XGBoost | 0.8630 | 0.7003 | **0.5293** | **0.6029** | **0.7369** |


> Random Forest : Mesmo com uma acurácia alta de 86,8%, o modelo tem um recall baixo de 47,8%, mostrando que pode errar ao não considerar clientes com churn. Além disso, o F1-score também é baixo, cerca de 58,8%. Neste caso, é necessário tirar as variáveis que mostraram um valor de qui-quadrado que não excluí a hipótese nula(H0) para a variável, ou seja, quando variáveis não tem nenhuma relação com churn.

> XBoost : O treinamento da base de dados com o modelo Xboost mostrou melhoria no recall e no F1-score para predição de churn de clientes; os valores de recall e F1 são, respectivamente, 52,9% e 60,3%. A acurácia e precisão caíram um pouco em relação ao modelo random forest, de 86,8% para 86,3% (acurácia) e 76,4% para 70,0% (precisão).
O modelo ficou mais sensível na classificação de possíveis clientes churn, o que pode gerar o alerta para os analistas.  No entanto, a acurácia e precisão sofreram neste processo, o que é bom para gerar maior engajamento de clientes, mas se mostram mais eficientes se o retorno financeiro dos clientes salvos supere o custo dos alarmes falsos.

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
