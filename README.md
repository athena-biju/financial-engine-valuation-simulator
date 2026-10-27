# MAAT Financial Engine — Forecasting and Valuation Simulations

**Exploratory financial modelling notebooks**, illustrating how a proposed fintech business might be evaluated under different growth, pricing and risk assumptions. This is a research/venture model, **not** a track record of investments made or an independent valuation of a listed company.

## What is in this repository?

- [`Financial Engine & Valuation Simulator.ipynb`](./Financial%20Engine%20%26%20Valuation%20Simulator.ipynb): 36-month illustrative client-growth, revenue, cash and burn projections; Monte Carlo scenarios (10,000 paths in the examples); Gordon Growth terminal-value sensitivity; and unit-economics measures such as LTV:CAC and payback.
- [`MAAT Financials 1.ipynb`](./MAAT%20Financials%201.ipynb): a companion modelling notebook retained as part of the exploratory project archive. Its complete execution was not independently revalidated for this documentation update.

## Investment-analysis questions

1. How much of a proposed valuation depends on the client-acquisition trajectory rather than current cash generation?
2. How do discount-rate and perpetual-growth assumptions change the terminal valuation?
3. Do proposed pricing, churn, acquisition costs and operating burn produce plausible unit economics?
4. What is the downside when growth assumptions are relaxed?

## How to inspect

Open the notebooks in GitHub for the written assumptions, code and stored outputs. To reproduce locally, use a Python/Jupyter environment with `numpy`, `pandas` and `matplotlib`, then review each notebook's variables before executing the cells. The notebooks have not been packaged or certified as a production application.

## Boundaries and interpretation

- **Illustrative inputs:** growth rates, margins, pricing and discount rates are model assumptions, not independently sourced market forecasts.
- **Valuation limitation:** a terminal-value model is very sensitive to the chosen discount and growth rates. Results should be interpreted as scenario exploration, not a recommendation to invest.
- **Prototype scope:** section headings discussing dashboards or exports are not evidence that a standalone deployed dashboard exists.
- **Provenance:** the project builds on MAAT venture modelling concepts; AI assistance was used for selected code and Markdown formatting, as disclosed in the original repository documentation.

**Relevant skills:** cash-flow modelling, valuation sensitivity, scenario analysis, Monte Carlo simulation, financial assumptions and unit economics.