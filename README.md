# Delta-Hedging-with-Bands
Delta hedging of stock options with bands. In the sample results below you can see that a delta hedging threshold of 0.02 works better than no threshold, especially for frequent rebalancing.

```
Option Parameters:
-----------------
Option Type:                   Straddle
Option Position:                -1.0000
Initial Stock Price (S0):      100.0000
Strike Price (K):              100.0000
Time to Maturity (T):            1.0000
Risk-free Rate (r):              0.0000
Implied Volatility (sigma):      0.2500
Realized Volatility:             0.2000
Transaction Cost:                0.0010
Number of Simulations:             1000


Delta Hedging Threshold: 0.0000
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          0         4.8334     11.5606      0.4181
          1         4.1223     12.1250      0.3400
          4         3.8164      6.7718      0.5636
         12         3.8656      4.0093      0.9641
         52         3.5995      2.3531      1.5297
        252         2.9273      1.4085      2.0783
        504         2.5333      1.1138      2.2745
        756         2.3199      1.0033      2.3123
       1008         2.0613      0.8798      2.3429
       2520         1.0437      0.4943      2.1113
       5040        -0.1386      0.2025     -0.6845
      10080        -1.8110      0.5943     -3.0475
      20160        -4.0764      1.3679     -2.9801

Best Rebalancing Frequency (Max Mean/Std):       1008

Delta Hedging Threshold: 0.0100
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          0         3.4148     12.9935      0.2628
          1         3.5671     12.2978      0.2901
          4         3.8259      6.3985      0.5979
         12         3.5769      4.1172      0.8688
         52         3.3284      2.2250      1.4959
        252         2.9975      1.3646      2.1966
        504         2.6339      1.1163      2.3595
        756         2.4335      0.9926      2.4517
       1008         2.1854      0.8707      2.5100
       2520         1.4857      0.4975      2.9864
       5040         0.8361      0.2738      3.0541
      10080         0.1897      0.4232      0.4481
      20160        -0.4179      0.8044     -0.5195

Best Rebalancing Frequency (Max Mean/Std):       5040

Delta Hedging Threshold: 0.0200
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          0         3.9789     12.3405      0.3224
          1         4.1756     12.3567      0.3379
          4         3.8055      6.6388      0.5732
         12         3.7568      4.1630      0.9024
         52         3.5376      2.2414      1.5783
        252         3.0615      1.4120      2.1682
        504         2.7595      1.1344      2.4327
        756         2.6013      1.0376      2.5071
       1008         2.4567      0.9681      2.5377
       2520         2.0170      0.6634      3.0402
       5040         1.7244      0.4734      3.6428
      10080         1.4366      0.3948      3.6386
      20160         1.1612      0.4622      2.5123

Best Rebalancing Frequency (Max Mean/Std):       5040

Delta Hedging Threshold: 0.0500
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          0         3.8235     12.3627      0.3093
          1         3.5175     12.0672      0.2915
          4         3.3276      6.6905      0.4974
         12         3.7414      3.8813      0.9640
         52         3.5384      2.3149      1.5286
        252         3.2057      1.5308      2.0942
        504         3.0447      1.3030      2.3367
        756         2.9602      1.1846      2.4989
       1008         2.9680      1.1769      2.5219
       2520         2.8473      1.0273      2.7717
       5040         2.7801      0.9586      2.9001
      10080         2.6412      0.9541      2.7683
      20160         2.6031      0.8614      3.0218

Best Rebalancing Frequency (Max Mean/Std):      20160

Delta Hedging Threshold: 0.1000
Delta Hedging Simulation Results
--------------------------------
Rebalancing    Mean Profit    Std Dev    Mean/Std
-----------    -----------    -------    --------
          0         4.1356     11.6412      0.3553
          1         3.1222     12.7470      0.2449
          4         4.0509      6.6061      0.6132
         12         3.7617      4.5053      0.8350
         52         3.5902      2.6657      1.3468
        252         3.3240      1.8404      1.8061
        504         3.3450      1.6840      1.9863
        756         3.2360      1.6493      1.9620
       1008         3.2808      1.6226      2.0219
       2520         3.2347      1.5093      2.1432
       5040         3.2665      1.4621      2.2342
      10080         3.1940      1.5026      2.1257
      20160         3.1630      1.4129      2.2387

Best Rebalancing Frequency (Max Mean/Std):      20160

Black-Scholes Price (Implied Volatility):     19.8953
Black-Scholes Price (Realized Volatility):    15.9311
BS Price Difference (Implied - Realized):      3.9642
Expected Profit (Ignoring T-Costs):            3.9642

Elapsed Time (s):   33.2110
```
