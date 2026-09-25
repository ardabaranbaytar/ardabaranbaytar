# Arda Baran Baytar 

I am a **Statistics graduate** with an associate degree in **Computer Programming**, starting my career in **data science and analytics**. I like taking a problem all the way from raw data to a working product: cleaning and exploring data, building and validating statistical and machine-learning models, and delivering the results as reports, dashboards, APIs and deployed applications.

My projects span finance, operations research and banking analytics, and they share one habit: testing results honestly — out-of-sample validation, realistic assumptions, and clearly reporting what did *not* work.

· [LinkedIn](https://www.linkedin.com/in/arda-baran-baytar-4b682a254/) · [Kaggle](https://www.kaggle.com/ardabaranbaytar) · [Medium](https://medium.com/@ardabaran119)

## Featured Projects

### [quant-lab](https://github.com/ardabaranbaytar/quant-lab) 

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

### [Banking ML: Cross-Platform Replication](https://github.com/ardabaranbaytar/banking-ml-cross-platform-replication) — *BSc thesis*

Reproduced and extended a graduate study on banking customer data across **Python, R, KNIME and Orange**: loan-repayment prediction, repayment-duration and credit-amount estimation, and customer segmentation with classification, regression and clustering methods.

`Python` `R` `KNIME` `Orange` `Machine Learning`

### [StochOpt-MDP](https://github.com/ardabaranbaytar/StochOpt-MDP) 

Optimal (s, S) inventory control formulated as a Markov Decision Process. The Bellman equation is solved by vectorized value iteration, and the resulting policy is benchmarked against base-stock and EOQ heuristics in a SimPy Monte Carlo simulation. Includes demand fitting (Poisson / Negative Binomial by AIC), a typed REST API, a React dashboard, and CSV/PDF reports.

`Python` `NumPy` `SciPy` `SimPy` `FastAPI` `React` `Docker`

### [alpha-quant](https://github.com/ardabaranbaytar/alpha-quant)

Statistical-arbitrage engine: Engle–Granger cointegration screening, a causal Kalman-filter hedge ratio, Ornstein–Uhlenbeck spread modeling and Z-score signals, routed through a portfolio risk gate into a deterministic paper-trading engine with a full audit trail. Prefix-invariance tests guarantee that future data can never change a past signal.

`Python` `statsmodels` `SQLAlchemy` `FastAPI` `MySQL`

### [JPMorgan Financial Performance Dashboard](https://github.com/ardabaranbaytar/jpmorgan-financial-performance-dashboard)

Power BI dashboard analyzing JPMorgan's financial performance and risk indicators using FDIC data.

## Technical Skills

* **Programming:** Python, SQL, R, TypeScript, Java
* **Statistics & Machine Learning:** pandas, NumPy, SciPy, statsmodels, scikit-learn, classification, regression, clustering, time-series analysis, Monte Carlo simulation
* **Domain Knowledge:** quantitative finance (backtesting, factor research, risk metrics), operations research (MDPs, simulation), banking analytics
* **Backend & Databases:** FastAPI, SQLAlchemy, MySQL, PostgreSQL
* **Frontend & Reporting:** React, Tailwind CSS, Power BI, Excel
* **Infrastructure:** Git, GitHub Actions, Docker, Linux (Ubuntu), systemd, Caddy

## Earlier Work

My first research repositories — [multi-strategy backtesting](https://github.com/ardabaranbaytar/multi-strategy-backtesting-framework), [momentum](https://github.com/ardabaranbaytar/momentum-strategy-backtest), [pairs trading](https://github.com/ardabaranbaytar/pairs-trading-backtest) and [equity factor research](https://github.com/ardabaranbaytar/equity-factor-research) — are archived. Their ideas were rebuilt and extended in **quant-lab**, including a fix for a look-ahead bias in the original pairs backtest (+86.8% with a full-sample hedge ratio → −11.0% with a rolling one).

---

*All trading projects are for research and education only. No real capital is deployed.*
