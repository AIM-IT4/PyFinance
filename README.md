# PyFinance

PyFinance/
├── __init__.py
└── portfolio_optimization.py

To use this package in your own code, you would first need to install it using pip. Then, you could import it and use its functions and classes like this:

Example :

import portfolio_optimization

# Create a portfolio with hypothetical returns and covariances
returns = [0.1, 0.15, 0.2]
covariances = [[0.01, 0.002, 0.003],
               [0.002, 0.04, 0.005],
               [0.003, 0.005, 0.09]]
portfolio = portfolio_optimization.Portfolio(returns, covariances)

# Calculate the expected return and volatility of the portfolio
expected_return = portfolio.expected_return()
expected_volatility = portfolio.expected_volatility()

# Optimize the portfolio using the random search algorithm
optimized_portfolio = portfolio.optimize()

# Simulate the performance of the optimized portfolio over 10000 trials
performance = portfolio_optimization.simulate_portfolio_performance(optimized_portfolio, num_trials=10000)

