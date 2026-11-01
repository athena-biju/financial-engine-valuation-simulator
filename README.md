# MAAT Financial Engine | Exploratory Valuation & Scenario Modelling

**Focus:** How sensitive is the valuation of an early-stage venture to growth, operating-cost, discount-rate and terminal-value assumptions?

**Research status:** Public Jupyter notebooks with illustrative inputs; **not** a historical investment track record, independently audited company valuation or tested production application.

## Research material

- [Financial Engine & Valuation Simulator](./Financial%20Engine%20%26%20Valuation%20Simulator.ipynb) — a 36-month client-growth and operating-cash projection, additional stochastic scenarios (10,000 paths in examples), and terminal-value sensitivities.
- [MAAT Financials 1](./MAAT%20Financials%201.ipynb) — a companion exploratory notebook retained in the project archive; it has not been fully revalidated for this README update.

## What the code illustrates

- Growth assumptions that change over phases of a venture's development.
- Revenue-like calculations, operating costs, cumulative cash position and cash runway.
- Monte Carlo simulations of terminal MRR and discount-rate/growth scenarios.
- Sensitivity of a terminal-value approach to the spread between discount rate and assumed perpetual growth.

## Accounting and valuation limitations (important)

1. In the deterministic notebook a column labelled `Revenue (€)` is calculated as **clients × price × gross margin**. This is closer to gross profit than gross revenue and should be relabelled or separated into distinct revenue, gross-profit and cash-flow lines.
2. Some terminal-value examples apply a Gordon-growth expression to monthly revenues or gross-profit proxies. **Gordon growth should ordinarily use the relevant sustainable cash flow or dividend measure, appropriately annualised**, and a defensible discount rate. The resulting values are mathematical sensitivity demonstrations, not validated fair values.
3. A constant highly positive **monthly** client-growth draw can compound into implausible terminal scale over 36 months; scenarios need market-capacity, churn and customer-acquisition constraints.
4. Selected terminal-value simulations condition on `r > g`. If sampling excludes invalid combinations, the resulting distribution is conditional on that filtering and may have long right tails near `r = g`.
5. The code uses illustrative assumptions rather than measured historical business results. A retained notebook heading referring to a dashboard or export layer is not proof of a deployed dashboard.

## Questions worth asking

- What proportion of valuation is explained by terminal assumptions rather than demonstrated unit economics?
- How do plausible market-size, churn, margin and acquisition-cost restrictions change the distribution?
- What downside scenarios can be underwritten without silently assuming uninterrupted compounding?
- What would an independent investor need to validate before assigning capital?

## Reproduce and extend

Inspect the code and its stated parameter values in Jupyter using `numpy`, `pandas` and `matplotlib`. No independent end-to-end execution certification is claimed.

**Analytical evidence:** Python modelling; scenario design; Monte Carlo mechanics; financial judgement about model sensitivity.  
**Provenance:** Exploratory MAAT venture work; AI assistance in selected code or formatting components as disclosed in original notebooks.

[Research index](https://github.com/athena-biju/rwi-portfolio-athena-biju/blob/main/research/README.md)
