# Option-Greeks

Step 1
Import the following libraries
1) Datetime
2) Pandas
3) Numpy
4) Scipy.stats
5) Pandas datareader
6) Matplotlib.pyplot - It will help you plot the data.
7) Py_vollib - It will help to perform Blackscholes calculation and directly calculate the option greeks.

Step 2 - Calculate the Volatility of the Instrument
Here Datetime Library will be used to select the data timeframe.
To get the data for the instrument we will use pdr.get_data
Then we will define the volatility
volatility = log_returns.rolling(window=TRADING_DAYS).std()*np.sqrt(252)

Step 3 - Black Scholes Model

We will define the BSM Variables
r = interest rate
S= stock price
K = strike price
T = Time
Sigma = Volatility ( We will used the above calculated volatility here).
We will calculate the Call option and Put option price.

Step 4 - Calculating Option greeks.

(Note - the numbers take in the calculation Black Scholes variable are arbitrary, except the Volatility).
