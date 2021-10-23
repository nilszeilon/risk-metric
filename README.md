### Risk metric for bitcoin 

* This risk metric can be used in tradingview by simply copying the code and pasting it in the strategy builder. Tried to publish on tradingview but seems like you first need to have an account for 3 months...

The risk-model takes an extension from a moving average as a fraction, close/MA and multiplies it by some growing factor to adjust for the growing market cap of the asset. This makes alot of sense to do before normalizing, since the fraction will have a harder time to reach the same level in an asset that has a market cap of 1T than the same asset with a market cap of 1B. 

##### Examples
![Risk metric with logarithmic growth](https://github.com/nilszeilon/risk-metric/blob/main/log_growth_example.png)

##### Thanks 

* A big thank you to Benjamin Cowen from Youtube, for inspiration to the risk metric. Worth noting that this is an approximation to his risk-metric, his risk-metric is private and may take alot more into account. 
* Thanks to quantadelic (tradingview) for the code to the logarithmic growth curves used in adjusting the risk. 


##### Usage and future work
* You may use this code in any way you like. 

* Add logarithmic growth compensation for other popular cryptocurrencies. 
* If you have any ideas to make the model perform even better feel free to fork this repository and contact me. 

