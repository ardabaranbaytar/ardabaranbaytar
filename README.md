# Arda Baran Baytar 👋

I am a **Statistics graduate** with an associate degree in **Computer Programming**, working toward a career in **quantitative research**. I build research tools end to end — from statistical tests and backtests to APIs, dashboards and deployed services — and I care most about results that survive honest validation: point-in-time data, out-of-sample tests and realistic costs.

🌐 [ardabaranbaytar.com](https://ardabaranbaytar.com) · 💼 [LinkedIn](https://www.linkedin.com/in/arda-baran-baytar-4b682a254/) · 📊 [Kaggle](https://www.kaggle.com/ardabaranbaytar) · ✍️ [Medium](https://medium.com/@ardabaran119)

## Featured Projects

### [quant-lab](https://github.com/ardabaranbaytar/quant-lab) · [live demo](https://quant.ardabaranbaytar.com)

Portfolio-level backtesting, factor research and a statistical-arbitrage paper-trading bot in one codebase, from research notebook to deployed app.

* Weight-based backtest engine: long/short and multi-asset, trades at the close and earns the next day's return, costs on actual turnover
* Point-in-time S&P 500 universe with delisting-aware accounting
* Walk-forward validation, purged yearly walk-forward for ML, placebo tests and a locked hold-out
* Pair-break monitor: seven causal detectors, each calibrated to a 1% daily false-alarm rate
* Daily paper-trading bot (SQL persistence, FastAPI, React dashboard), scheduled on a Linux server

**Survivorship bias, measured.** The same monthly momentum strategy (2010–2024):

| Universe | CAGR | Sharpe |
|---|---:|---:|
| Today's S&P 500 constituents (typical tutorial setup) | 25.1% | 1.09 |
| Point-in-time S&P 500 membership | 10.1% | 0.55 |
| SPY buy & hold | 13.6% | 0.83 |

The project also documents negative results: classic pairs trading and Avellaneda–Lee residual stat-arb do not survive costs out of sample on free daily large-cap data, and an ML entry filter showed no predictive power.

`Python` `pandas` `statsmodels` `FastAPI` `MySQL` `React` `TypeScript` `GitHub Actions`

### [StochOpt-MDP](https://github.com/ardabaranbaytar/StochOpt-MDP) · [live demo](https://stochopt.ardabaranbaytar.com)

Optimal (s, S) inventory control formulated as a Markov Decision Process. The Bellman equation is solved by vectorized value iteration, and the resulting policy is benchmarked against base-stock and EOQ heuristics in a SimPy Monte Carlo simulation. Includes demand fitting (Poisson / Negative Binomial by AIC), a typed REST API, a React dashboard, and CSV/PDF reports.

`Python` `NumPy` `SciPy` `SimPy` `FastAPI` `React` `Docker`

### [alpha-quant](https://github.com/ardabaranbaytar/alpha-quant)

Statistical-arbitrage engine: Engle–Granger cointegration screening, a causal Kalman-filter hedge ratio, Ornstein–Uhlenbeck spread modeling and Z-score signals, routed through a portfolio risk gate into a deterministic paper-trading engine with a full audit trail. Prefix-invariance tests guarantee that future data can never change a past signal.

`Python` `statsmodels` `SQLAlchemy` `FastAPI` `MySQL`

### [Banking ML: Cross-Platform Replication](https://github.com/ardabaranbaytar/banking-ml-cross-platform-replication) — *BSc thesis*

Reproduced and extended a graduate study on banking customer data across **Python, R, KNIME and Orange**: loan-repayment prediction, repayment-duration and credit-amount estimation, and customer segmentation with classification, regression and clustering methods.

### [JPMorgan Financial Performance Dashboard](https://github.com/ardabaranbaytar/jpmorgan-financial-performance-dashboard)

Power BI dashboard analyzing JPMorgan's financial performance and risk indicators using FDIC data.

## Technical Skills

* **Programming:** Python, SQL, R, TypeScript, Java
* **Statistics & Data:** pandas, NumPy, SciPy, statsmodels, scikit-learn, time-series analysis, Monte Carlo simulation
* **Quantitative Finance:** backtesting, cointegration & pairs trading, factor research, walk-forward validation, risk metrics
* **Backend & Databases:** FastAPI, SQLAlchemy, MySQL, PostgreSQL
* **Frontend & Reporting:** React, Tailwind CSS, Power BI, Excel
* **Infrastructure:** Git, GitHub Actions, Docker, Linux (Ubuntu), systemd, Caddy

## Earlier Work

My first research repositories — [multi-strategy backtesting](https://github.com/ardabaranbaytar/multi-strategy-backtesting-framework), [momentum](https://github.com/ardabaranbaytar/momentum-strategy-backtest), [pairs trading](https://github.com/ardabaranbaytar/pairs-trading-backtest) and [equity factor research](https://github.com/ardabaranbaytar/equity-factor-research) — are archived. Their ideas were rebuilt and extended in **quant-lab**, including a fix for a look-ahead bias in the original pairs backtest (+86.8% with a full-sample hedge ratio → −11.0% with a rolling one).

---

*All trading projects are for research and education only. No real capital is deployed.*
