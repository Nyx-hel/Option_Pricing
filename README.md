# Black_Scholes_Model

Financial Option Pricing Models
This repository contains Jupyter Notebooks demonstrating two fundamental models used in quantitative finance for option pricing: the Black-Scholes Model and the Heston Stochastic Volatility Model.

Files
Black_scholes.ipynb: Implements the Black-Scholes model for pricing European call and put options. It includes steps for fetching historical stock data, calculating annual volatility, and comparing theoretical option prices with actual market prices.

HESTON_STOCHASTIC_VOLATILITY_MODEL_CODE.ipynb: Contains code for the Heston Stochastic Volatility Model, which accounts for the stochastic nature of volatility in option pricing. This model is generally more complex than Black-Scholes but can offer a more realistic representation of market dynamics.

Black-Scholes Model (Black_scholes.ipynb)
Overview
The Black-Scholes model is a mathematical model for the dynamics of a financial market containing derivative investment instruments. From the model, one can deduce the Black-Scholes formula, which gives a theoretical estimate of the price of European-style options.

Key Features
Data Import: Fetches historical stock data using yfinance.

Volatility Calculation: Calculates annual volatility based on historical logarithmic returns.

Option Pricing: Implements the euro_vanilla function to compute theoretical call and put option prices.

Comparison: Compares the calculated theoretical call prices with actual market call prices for a given expiry.

Libraries Used
yfinance

pandas

numpy

matplotlib.pyplot

scipy.stats

Usage
Install Dependencies:

pip install yfinance pandas numpy scipy matplotlib

Open the Notebook:
Open Black_scholes.ipynb in a Jupyter environment (Jupyter Lab, Jupyter Notebook, or Google Colab).

Run Cells:
Execute the cells sequentially to see data import, volatility calculation, and option pricing. You can modify the symbol and T (time to expiry) parameters to experiment with different stocks and maturities.

Heston Stochastic Volatility Model (HESTON_STOCHASTIC_VOLATILITY_MODEL_CODE.ipynb)
Overview
The Heston model is a mathematical model that describes the evolution of the volatility of an underlying asset. Unlike the Black-Scholes model, which assumes constant volatility, the Heston model allows volatility to be stochastic, meaning it changes over time. This makes it more suitable for pricing options in markets where volatility exhibits clustering and mean reversion.

Key Features (Based on snippet analysis - full features may vary)
Data Import: Uses yfinance to fetch historical stock data.

Logarithmic Returns and Volatility: Calculates logarithmic returns and an initial volatility estimate.

Heston Call Price Calculation: Includes a heston_call_price function for calculating option prices under the Heston model. (Note: The full implementation of this function is not visible in the provided snippet, but its usage implies its presence.)

Parameter Optimization (Inferred): The presence of r_opt, k_opt, theta_opt, and sigma_opt suggests that the notebook likely includes a section for optimizing Heston model parameters to fit market data.

Libraries Used
yfinance

pandas

numpy

matplotlib.pyplot

sympy

scipy

scipy.stats

scipy.integrate

Usage
Install Dependencies:

pip install yfinance pandas numpy sympy scipy matplotlib

Open the Notebook:
Open HESTON_STOCHASTIC_VOLATILITY_MODEL_CODE.ipynb in a Jupyter environment.

Run Cells:
Execute the cells to observe how the Heston model is applied to real stock data. You may need to review the complete notebook for detailed instructions on parameter calibration and specific output interpretations.

Contributing
Feel free to fork this repository, open issues, or submit pull requests.

License
[Specify your license here, e.g., MIT, Apache 2.0, etc.]
