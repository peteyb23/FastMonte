# FastMonte Research Journal

This journal records what I learn, why the project makes particular choices, and what the experiments actually show. Entries should be written plainly enough that I could explain them in an interview.

## Phase 0 — Project foundation

### The project in my own words

_Complete this after the Phase 0 comprehension check._

### Research question

How can variance-reduction methods make Monte Carlo option pricing more accurate and computationally efficient?

### Decisions

- Begin with European call options because they have a clear payoff rule and an analytical Black–Scholes benchmark.
- Compare standard Monte Carlo, antithetic variates, and control variates.
- Measure price estimates, error, standard error, confidence intervals, convergence, and runtime.
- Add source files only when their purpose has been taught.
- Keep all numerical claims evidence-based and reproducible.

### Scope boundaries

The initial project will not use live market data, recommend trades, price American or exotic options, optimize portfolios, or use machine learning.

### Results and discoveries

_No experimental results yet._

### Questions I still have

_Add questions here as they arise._

## Phase 1 — The financial problem

### My explanation

A European call option gives me the right, but not the obligation, to buy a stock at a fixed strike price on its expiration date. Its payoff is the greater of the final stock price minus the strike price or zero. It can be valuable before expiration because I can benefit if the stock rises while declining the transaction if exercising would hurt me. FastMonte will help determine what the call option is worth today so a buyer and seller can agree on the price paid for that future choice.

### What I learned

- A stock share represents a small ownership interest in a company.
- A European call option can be exercised only on its expiration date.
- Call payoff is `max(final stock price - strike price, 0)`.
- Payoff and profit differ because the option itself normally costs money upfront.
- Greater volatility and more time to expiration generally make a call option more valuable.
- Higher interest rates generally increase a call option's value because payment of the strike price is delayed.
- Pricing models depend on simplifying assumptions and do not perfectly reproduce real markets.

### Running example

- Stock price today: $100
- Strike price: $105
- Time to expiration: one year

### Current open question

How can we estimate a fair option price today when the stock's final price is unknown?
