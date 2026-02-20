AI can now build trading algorithms like Goldman Sachs' algorithmic trading desk (for free).
https://x.com/heynavtoor/status/2024475005485273538/photo/1

Here are 15 insane Claude prompts that replace $500K/year quant strats (Save for later)
1. The Goldman Sachs Quant Strategy Architect
"You are a managing director on Goldman Sachs' algorithmic trading desk who designs systematic trading strategies managing $10B+ in institutional capital across global equity markets.
I need a complete quantitative trading strategy designed from scratch.
Architect:
- Strategy thesis: the specific market inefficiency or pattern this strategy exploits
- Universe selection: which instruments to trade and why (stocks, ETFs, futures, options)
- Signal generation logic: the exact mathematical rules that produce buy and sell signals
- Entry rules: precise conditions that must all be true before opening a position
- Exit rules: profit targets, stop losses, time-based exits, and signal reversal exits
- Position sizing model: how much capital to allocate per trade based on conviction and risk
- Risk parameters: maximum drawdown, position limits, sector exposure caps, and correlation limits
- Backtesting framework: how to properly test this strategy against historical data
- Benchmark selection: what to measure performance against and why
- Edge decay monitoring: how to detect when the strategy stops working
Format as a Goldman Sachs-style quantitative strategy memo with mathematical formulas, pseudocode logic, and risk parameter tables.
My trading focus: [DESCRIBE YOUR CAPITAL, PREFERRED MARKETS, TIME HORIZON, RISK TOLERANCE, AND ANY STRATEGIES YOU'VE EXPLORED]"

2. The Renaissance Technologies Backtesting Engine

"You are a senior quantitative researcher at Renaissance Technologies who builds rigorous backtesting systems that separate real alpha from overfitted noise across decades of market data.
I need a complete backtesting framework that gives me honest, reliable results.
Build:
- Data requirements: which historical data feeds I need, minimum time periods, and data quality checks
- Backtesting engine architecture: event-driven or vectorized with pros and cons for my strategy type
- Transaction cost modeling: commissions, slippage, bid-ask spread, and market impact estimates
- Lookahead bias prevention: safeguards that ensure no future data leaks into past decisions
- Survivorship bias handling: accounting for delisted stocks and failed companies in historical data
- Walk-forward optimization: train on past data, test on unseen data in rolling windows
- Out-of-sample testing protocol: how to split data so results aren't just curve-fitting
- Monte Carlo simulation: randomize trade sequences to understand the range of possible outcomes
- Statistical significance tests: is the backtest return real or could it happen by random chance
- Complete Python backtesting code ready to run with sample data and visualization

Format as a quantitative research document with full Python code, statistical validation methodology, and result interpretation guidelines.

My strategy: [DESCRIBE YOUR TRADING STRATEGY, PREFERRED MARKET, TIME FRAME, AND AVAILABLE HISTORICAL DATA]"


3. The Two Sigma Risk Management System

"You are a senior portfolio risk manager at Two Sigma who builds risk management frameworks protecting $60B+ in assets from catastrophic losses during black swan events and market crashes.

I need a complete risk management system for my trading operations.

Build:

- Position sizing algorithm: Kelly Criterion or fractional Kelly with exact implementation
- Stop-loss framework: fixed, trailing, volatility-adjusted, and time-based stops with rules for each
- Maximum drawdown controls: hard limits that automatically reduce position size or halt trading
- Correlation monitoring: detect when supposedly uncorrelated positions start moving together
- Value at Risk (VaR) calculation: estimate maximum daily loss at 95% and 99% confidence levels
- Stress testing scenarios: simulate portfolio behavior during 2008 crash, COVID crash, and flash crashes
- Leverage limits: maximum margin utilization rules with automatic deleveraging triggers
- Sector and factor exposure caps: prevent hidden concentration risk across positions
- Liquidity risk assessment: ensure every position can be exited within acceptable timeframe and cost
- Daily risk dashboard: every metric I should check every morning before markets open

Format as a Two Sigma-style risk management specification with formulas, Python implementation code, and a daily risk monitoring checklist.

My portfolio: [DESCRIBE YOUR TRADING CAPITAL, STRATEGY TYPES, POSITION COUNT, LEVERAGE USAGE, AND BIGGEST RISK CONCERN]"

4. The Citadel Alpha Signal Research Lab

"You are a senior quantitative researcher at Citadel who discovers and validates new alpha signals by analyzing alternative data, market microstructure, and statistical patterns across thousands of securities.

I need a systematic process for discovering profitable trading signals.

Research:

- Signal idea generation framework: 20 categories of potential alpha signals to investigate
- Data source inventory: price data, fundamental data, sentiment data, and alternative data sources
- Feature engineering pipeline: transform raw data into testable trading signals step by step
- Signal strength testing: information coefficient, hit rate, and risk-adjusted return for each signal
- Decay analysis: how quickly each signal loses its predictive power after formation
- Correlation check: ensure new signals aren't just repackaging existing known factors
- Signal combination methodology: how to blend multiple weak signals into one strong composite
- Regime detection: identify which signals work in trending vs mean-reverting vs volatile markets
- Turnover analysis: how often the signal forces trades and whether the alpha survives transaction costs
- Signal monitoring dashboard: track live signal performance against backtested expectations

Format as a Citadel-style quantitative research report with signal definitions, statistical test results, and Python code for signal generation.

My focus: [DESCRIBE YOUR MARKET, AVAILABLE DATA SOURCES, TRADING FREQUENCY, AND TYPES OF SIGNALS YOU'RE INTERESTED IN]"

5. The Jane Street Market Making Engine

"You are a senior quantitative trader at Jane Street who designs market-making algorithms that profit from bid-ask spreads while managing inventory risk across thousands of trades per day.

I need a complete market-making strategy framework.

Design:

- Spread calculation model: how to set bid and ask prices based on volatility, volume, and inventory
- Inventory management: rules for staying neutral and avoiding large directional bets
- Quote adjustment logic: how to shift prices when inventory builds up on one side
- Adverse selection detection: identify when informed traders are picking off your quotes
- Speed and latency requirements: how fast order placement and cancellation need to be
- Hedging strategy: when and how to offset accumulated directional risk
- Market microstructure analysis: understanding order book dynamics, tick sizes, and queue priority
- PnL decomposition: separate profit from spread capture vs directional moves vs hedging costs
- Risk limits: maximum inventory, maximum loss per day, and automatic shutdown triggers
- Performance metrics: spread captured, inventory turnover, Sharpe ratio, and fill rate targets

Format as a Jane Street-style trading system specification with mathematical models, pseudocode, and risk parameter tables.

My interest: [DESCRIBE THE MARKET YOU WANT TO MAKE IN, YOUR CAPITAL, TECHNOLOGY AVAILABLE, AND EXPERIENCE LEVEL WITH MARKET MAKING]"



6. The AQR Factor Model Builder

"You are a senior researcher at AQR Capital Management who builds multi-factor models used to construct portfolios that systematically harvest risk premiums across global markets.

I need a complete factor model for portfolio construction.

Build:

- Factor selection: which factors to include (value, momentum, quality, size, low volatility) with evidence
- Factor definition: exact calculation formula for each factor using available financial data
- Factor portfolio construction: how to build long-short portfolios for each individual factor
- Factor exposure measurement: how to calculate my current portfolio's exposure to each factor
- Factor correlation matrix: how factors move relative to each other and diversification benefits
- Multi-factor combination: how to weight and blend factors into a single composite score
- Rebalancing methodology: when to rebalance factor portfolios and how to minimize turnover
- Factor timing analysis: can we increase exposure to factors when conditions favor them
- Performance attribution: decompose returns into factor contributions and stock-specific alpha
- Complete Python implementation with data loading, factor calculation, and portfolio construction

Format as an AQR-style factor research paper with mathematical definitions, empirical results framework, and production-ready code.

My investment universe: [DESCRIBE YOUR MARKET (US STOCKS, GLOBAL, ETFs), CAPITAL SIZE, REBALANCING FREQUENCY, AND FACTOR PREFERENCES]"


7. The D.E. Shaw Statistical Arbitrage System

"You are a senior portfolio manager at D.E. Shaw who builds statistical arbitrage systems that exploit pricing relationships between related securities using advanced statistical methods.

I need a complete pairs trading and statistical arbitrage framework.

Build:

- Pair selection methodology: how to find stocks that move together using correlation and cointegration
- Cointegration testing: Engle-Granger and Johansen tests to verify the pair relationship is real
- Spread calculation: how to measure the price difference between paired securities correctly
- Z-score signal generation: when the spread deviates enough from normal to trigger a trade
- Entry and exit thresholds: exact z-score levels for opening, adding to, and closing positions
- Hedge ratio calculation: how many shares of each stock to trade to stay market-neutral
- Mean reversion speed analysis: how quickly the spread typically returns to normal
- Regime change detection: identify when a pair relationship breaks down permanently
- Portfolio of pairs: how to run 20+ pairs simultaneously with capital allocation rules
- Complete Python code with pair screening, signal generation, and backtesting

Format as a D.E. Shaw-style quantitative research document with statistical test outputs, strategy rules, and full implementation code.

My market: [DESCRIBE YOUR PREFERRED SECTOR OR MARKET, AVAILABLE DATA, TRADING CAPITAL, AND EXPERIENCE WITH PAIRS TRADING]"

