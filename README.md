# Delta Hedging with Bands
Delta hedging of stock options with bands. In the sample results below you can see that a delta hedging threshold of 0.01 to 0.05 better than no threshold, especially for frequent rebalancing.

```
Option Parameters:
-----------------
Option Type:                   Straddle
Option Position:                -1.0000
Initial Stock Price (S0):      100.0000
Strike Price (K):              100.0000
Time to Maturity (T):            1.0000
Risk-free Rate (r):              0.0500
Implied Volatility (sigma):      0.2000
Realized Volatility:             0.1500
Transaction Cost:                0.0010
Number of Simulations:            10000
RNG seed:                            42

Delta Hedging Threshold: 0.0000
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          1         3.7758      8.8546      0.4264
          4         3.7540      4.9349      0.7607
         12         3.6114      3.1809      1.1354
         52         3.3932      1.8781      1.8067
        252         2.9258      1.2450      2.3500
       2520         1.0847      0.4771      2.2733
       5040        -0.0225      0.1758     -0.1279

Best Rebalancing Frequency (Max Mean/Std):        252

Delta Hedging Threshold: 0.0100
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          1         3.7758      8.8546      0.4264
          4         3.7541      4.9347      0.7608
         12         3.6116      3.1808      1.1355
         52         3.3960      1.8781      1.8082
        252         2.9502      1.2430      2.3735
       2520         1.5631      0.4914      3.1813
       5040         1.0036      0.2469      4.0644

Best Rebalancing Frequency (Max Mean/Std):       5040

Delta Hedging Threshold: 0.0200
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          1         3.7758      8.8546      0.4264
          4         3.7540      4.9350      0.7607
         12         3.6134      3.1805      1.1361
         52         3.4021      1.8814      1.8082
        252         3.0053      1.2504      2.4036
       2520         2.1025      0.6264      3.3565
       5040         1.8373      0.4609      3.9865

Best Rebalancing Frequency (Max Mean/Std):       5040

Delta Hedging Threshold: 0.0500
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          1         3.7758      8.8546      0.4264
          4         3.7549      4.9389      0.7603
         12         3.6190      3.1892      1.1348
         52         3.4393      1.9173      1.7938
        252         3.1881      1.3591      2.3457
       2520         2.8366      0.9719      2.9186
       5040         2.7630      0.9136      3.0241

Best Rebalancing Frequency (Max Mean/Std):       5040

Black-Scholes Price (Implied Volatility):     16.0241
Black-Scholes Price (Realized Volatility):    12.3063
BS Price Difference (Implied - Realized):      3.7179
Expected Profit (Ignoring T-Costs):            3.7179

Elapsed Time (s):   69.5800
```
