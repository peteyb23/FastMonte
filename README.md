# FastMonte

An interactive quantitative-finance lab that compares Monte Carlo methods for pricing European call options.

## Research question

How can variance-reduction methods make Monte Carlo option pricing more accurate and computationally efficient?

## What the finished project will do

A user will choose a hypothetical stock price, option contract, time remaining, volatility, interest rate, simulation count, and simulation method. FastMonte will then:

- estimate the option's value using Monte Carlo simulation;
- calculate the Black–Scholes benchmark price;
- report error, uncertainty, and runtime;
- visualize simulated stock prices and option payoffs;
- show how estimates converge as the simulation count grows; and
- compare standard Monte Carlo, antithetic variates, and control variates.

FastMonte is both a learning project and a reproducible experiment. Any numerical finding reported here will come from saved experiments, not assumptions.

## Scope

### Included

- European call options
- Geometric Brownian motion under Black–Scholes assumptions
- Standard Monte Carlo simulation
- Antithetic variates
- Control variates
- Black–Scholes analytical benchmark
- Accuracy, uncertainty, convergence, and runtime comparisons
- Interactive Streamlit application
- Automated tests and reproducible experiments

### Not included in the initial project

- Live market data or brokerage connections
- American, exotic, or multi-asset options
- Trading recommendations or strategies
- Portfolio optimization
- Machine learning
- A full stochastic-calculus derivation
- Production trading infrastructure

These are possible future extensions only after the core research question is answered.

## Planned project structure

```text
FastMonte/
├── app.py                  # Streamlit interface (Phase 9)
├── src/
│   ├── black_scholes.py    # Analytical benchmark (Phase 5)
│   ├── monte_carlo.py      # Simulation methods (Phases 3, 7, 8)
│   └── experiments.py      # Reproducible benchmarks (Phase 6)
├── tests/                  # Automated tests (added with the code tested)
├── notebooks/              # Exploratory research, only when useful
├── README.md
├── requirements.txt        # Dependencies, added when first needed
└── research_journal.md     # Learning notes, decisions, and results
```

Files will be introduced during the phase in which their purpose is learned.

## Project checklist

- [x] Phase 0: Define the finished project, lock scope, and establish the repository
- [x] Phase 1: Learn the financial problem and explain it in my own words
- [ ] Phase 2: Learn probability and Monte Carlo through a small simulation
- [ ] Phase 3: Build the simplest standard Monte Carlo option pricer
- [ ] Phase 4: Understand and implement the stock-price model
- [ ] Phase 5: Build and test the Black–Scholes benchmark
- [ ] Phase 6: Design and run the standard Monte Carlo experiment
- [ ] Phase 7: Implement and evaluate antithetic variates
- [ ] Phase 8: Implement and evaluate control variates
- [ ] Phase 9: Build the interactive Streamlit application
- [ ] Phase 10: Test, validate, and clean the project
- [ ] Phase 11: Write the quantitative research report
- [ ] Phase 12: Polish GitHub, deploy, and prepare portfolio explanations

## Current status

Phases 0 and 1 are complete. The financial problem and call-option payoff are understood; no pricing or simulation code has been written yet.
