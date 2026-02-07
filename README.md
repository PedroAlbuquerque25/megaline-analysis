# Megaline Telecom: Data-Driven Revenue Analysis 📞📊

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Conda](https://img.shields.io/badge/Environment-Conda-green.svg)](https://docs.conda.io/)
[![Market](https://img.shields.io/badge/Market-Canada/US-red.svg)](#)

## 🇺🇸 Project Overview (English)
As a Data Analyst for **Megaline**, a major telecom operator, I analyzed the profitability of two prepaid plans: **Surf** and **Ultimate**. The objective was to identify consumption patterns among 500 users and determine which plan generates more revenue to optimize the company's marketing budget.

### 🚀 Key Findings & Business Insights
* **Revenue Drivers:** Users on the **Surf** plan frequently exceed their data limits, generating significant additional revenue through overage fees, making it highly profitable despite the lower base fee.
* **Usage Patterns:** Data consumption is the primary differentiator. Most Surf users pay for extra Gigabytes, suggesting a need for a mid-tier plan.
* **Statistical Validation:** Conducted **Independent Samples T-tests** (Welch's t-test) to confirm that the revenue difference between plans is statistically significant ($p < 0.05$).
* **Regional Neutrality:** The analysis proved that user behavior and revenue in the **NY-NJ area** are not significantly different from other regions.

### 🛠️ Technical Implementation
* **ETL & Data Cleaning:** Processed five relational datasets, handled missing values, and corrected data types (datetime conversion).
* **Complex Business Logic:** Implemented specific billing rules:
    * Individual calls rounded up to the nearest minute.
    * Total monthly data usage rounded up to the next Gigabyte.
* **Statistical Analysis:** Used `scipy.stats` for hypothesis testing and `seaborn` for distribution analysis (Histograms and Boxplots).

---

## 🇧🇷 Resumo do Projeto (Português)
Análise de rentabilidade dos planos **Surf** e **Ultimate** da operadora **Megaline**. O projeto utiliza análise exploratória de dados e testes estatísticos para definir onde a empresa deve focar seus investimentos publicitários.

### 🔍 Destaques Técnicos
* **Lógica de Negócio:** Arredondamento de chamadas e dados conforme regras da empresa.
* **Testes de Hipóteses:** Validação estatística de que a receita entre os planos é significativamente diferente.
* **Visualização:** Gráficos comparativos de consumo mensal por plano.

---

## 📂 Project Structure
```text
├── datasets/             # Megaline CSV files (Calls, Internet, Messages, Plans, Users)
├── notebooks/            # Jupyter Notebook with complete analysis
├── README.md             # Project documentation
└── requirements.txt      # Project dependencies