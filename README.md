# Pine Script

A library of trading indicators, strategies and code snippets for Pine Script programming language.

---
## Strategies
* [Template Simple Strategy](/Strategies/Template%20Simple%20Strategy.pine)
> An simple long/short strategy template file.

* [Template Advance Strategy](/Strategies/Template%20Advance%20Strategy.pine)
> An advance long/short strategy template file.
> The template file layout an trend following trading system. [1] [2]
> * Trend Following - An indicator that identify trend's direction, most likely an moving average.
> * Trend Confirmation - Most trend following indicator are prone to whipsaw, so you what to confirm the movement with something like an momentum indicator.
> * Entry/Exit - Now that you have an trend directional bias you may want to find an optimal entry/exit strategy this is where overbought/oversold indicator come in handy.
> * Stop-Loss and Profit-Taking - We need to determine an method to take profit on a winning trade and an loss on an losing trade. [3]
> * Position Sizing - To control risk and maximize gains we must determine what size of a position we are willing to risk. [4]
>
> References/Notes:  
> [1] https://www.babypips.com/learn/forex/design-your-trading-system  
> [2] https://www.investopedia.com/articles/forex/10/indicators-fx-traders-must-know.asp  
> [3] I provided an method using bollinger bands with an stop loss and three profit-taking price levels. Each time an tp level is hit you will reduce your position and move the stop-loss to the old price level.  
> [4] I use the formula: Position Size = Risk Amount / Distance to Stop Loss. https://medium.com/@cryptocreddy/comprehensive-guide-to-position-size-and-leverage-2e27764ce9e0

* [Example Advance Strategy](/Strategies/Example%20Advance%20Strategy.pine)
> An example of an advance trend following strategy. [1]
> * Trend Following - Moving Average.
> * Trend Confirmation - Waddah Attar Explosion.
> * Entry/Exit - Fisher Transform.
>
> References/Notes:  
> [1] If you wish to see re-entry results increase the Trades Count setting.

* [Moving Average Strategy](/Strategies/Moving%20Average%20Strategy.pine)
> Moving average cross strategies with three type:
> Price Cross - When price cross the slow ma
> Two Cross - When fast ma cross the slow ma
> Tri Cross - When fast ma cross mid, slow ma

* [Waddah Attar Explosion Strategy](/Strategies/Waddah%20Attar%20Explosion%20Strategy.pine)
> Waddah Attar Explosion with custom moving averages and exit strategies

* [Fisher Transform Strategy](/Strategies/Fisher%20Transform%20Strategy.pine)
> Fisher Transform with an changeable EMA alpha https://www.mesasoftware.com/papers/UsingTheFisherTransform.pdf

* [Godmode Oscillator Strategy](/Strategies/Godmode%20Oscillator%20Strategy.pine)
> A rewrite of Godmode Oscillator https://www.tradingview.com/script/HL3vqXUM-Godmode-Oscillator-fresh-bread-generator-free-to-use/  
> \@author LazyBear, xSilas, Ni6HTH4wK

* [Requested 001 Strategy](/Strategies/Requested%20001%20Strategy.pine)
> Requested strategy by discord user Mrhutqc#2962  
> A rewrite of Logical_Strat_Template_v0.2  
> \@author MrhutQC, Ozine  
> \@thanks DarkRico, FurryBoffin  
> * Trend Following - Higher Timeframe Moving Average.
> * Trend Confirmation - Waddah Attar Explosion.
> * Entry/Exit - Fisher Transform, Godmode Oscillator. https://www.tradingview.com/script/HL3vqXUM-Godmode-Oscillator-fresh-bread-generator-free-to-use/

---
## Indicators
* [Moving Average Indicator](/Indicators/Moving%20Average%20Strategy.pine)
> Moving average cross strategies with three type:
> Price Cross - When price cross the slow ma
> Two Cross - When fast ma cross the slow ma
> Tri Cross - When fast ma cross mid, slow ma

* [Waddah Attar Explosion Indicator](/Indicators/Waddah%20Attar%20Explosion%20Strategy.pine)
> Waddah Attar Explosion with custom moving averages and exit strategies

* [Risk Bands Indicator](/Indicators/Risk%20Bands%20Indicator.pine)
> An standalone indicator version of the stop-loss and profit-taking from Template Advance Strategy.

* [Fisher Transform Indicator](/Indicators/Fisher%20Transform%20Indicator.pine)
> Fisher Transform with an changeable EMA alpha https://www.mesasoftware.com/papers/UsingTheFisherTransform.pdf

* [Godmode Oscillator Indicator](/Indicators/Godmode%20Oscillator%20Indicator.pine)
> A rewrite of Godmode Oscillator https://www.tradingview.com/script/HL3vqXUM-Godmode-Oscillator-fresh-bread-generator-free-to-use/  
> \@author LazyBear, xSilas, Ni6HTH4wK

---
## Snippets
* [Moving Average](/Snippets/Moving%20Average.pine)
> An collection of moving averages used in the code base. [1]
> * alma - Arnaud Legoux Moving Average
> * cvwma - Coefficient of Variation Weighted Moving Average https://www.tradingview.com/script/0dBtJvhu-Stratus-DW/
> * dema - Double Exponential Moving Average
> * donchian - Donchian Middle Channel
> * ema - Exponential Moving Average
> * frama - Fractal Adaptive Moving Average http://www.mesasoftware.com/papers/FRAMA.pdf
> * hull - Hull Moving Average
> * jma - Jurik Moving Average https://www.tradingview.com/script/nZuBWW9j-Jurik-Moving-Average/
> * kama - Kaufman Adaptive Moving Average
> * lsma - Least Square Moving Average
> * mcginley - McGinley Dynamic
> * modframa - Modified Fractal Adaptive Moving Average http://etfhq.com/blog/2010/09/30/fractal-adaptive-moving-average-frama/#Mod
> * rma - Running Moving Average https://en.wikipedia.org/wiki/Moving_average#Modified_moving_average
> * sma - Simple Moving Average
> * smma - Smoothed Moving Average
> * supersmoother - SuperSmoother Filter http://www.mesasoftware.com/papers/PredictiveIndicatorsForEffectiveTrading%20Strategies.pdf
> * tema - Triple Exponential Moving Average
> * vama - Volatility Adjusted Moving Average https://www.tradingview.com/script/ZHGCH1jf-Volatility-Adjusted-Moving-Average-JD/
> * vidya - Variable Index Dynamic Average https://www.tradingview.com/script/hdrf0fXV-Variable-Index-Dynamic-Average-VIDYA/
> * vwma - Volume-Weighted Moving Average
> * wma - Weighted Moving Average
> * zlema - Zero Lag Exponential Moving Average http://www.mesasoftware.com/papers/ZeroLag.pdf  
>
> References/Notes:  
> [1] TradingView will slow down when their is a long chain of if/else statement, so have to split MA function.

* [Channel Bands](/Snippets/Channel%20Bands.pine)
> An collection of channel bands used in the code base.
> * bollinger - Bollinger Bands
> * keltner - Keltner Channels
> * atr - Average True Range
> * donchian - Bollinger Bands
> * chandelier - Chandelier Exit

* [Momentum](/Snippets/Momentum.pine)
> Description:
> An collection of momentum indicator used in the code base.
> * adx - Average Directional Movement Index
> * adxr - Average Directional Movement Index Rating
> * apo - Absolute Price Oscillator
> * aroonosc - Aroon Oscillator
> * asi - Accumulative Swing Index https://library.tradingtechnologies.com/trade/chrt-ti-accumulative-swing-index.html
> * bop - Balance Of Power
> * cci - Commodity Channel Index
> * cmo - Chande Momentum Oscillator
> * crsi - Connors RSI https://www.tradingmarkets.com/media/2012/ConnorsRSI-Pullbacks-Guidebook.pdf [1]
> * dx - Directional Movement Index
> * imi - Intraday Momentum Index
> * mfi - Money Flow Index
> * ppo - Percentage Price Oscillator
> * roc - Rate of change
> * rsi - Relative Strength Index
> * stoch - Stochastic K https://www.freestockcharts.com/help/Content/Indicators/Stochastics.htm [2]
> * stochrsi - Stochastic Relative Strength Index [2]
> * ultosc - Ultimate Oscillator
> * willr - Williams %R
>
> References/Notes:  
> [1] Use PercentRank instead of ROC describe in ConnorsRSI Guidebook.  
> [2] Return K not %K: %K = sma(K, pk_len) %D = sma(%K, pd_len)

---
## Copying
You may copy and/or modified this project source code on the condition that you released under the same license and keep copyright notice when distributing this project source code.
TradingView template default header are license under Mozilla Public License 2.0
> // This source code is subject to the terms of the Mozilla Public License 2.0 at https://mozilla.org/MPL/2.0/  
> // © YOUR NAME

---
## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md) file.

---
## Donation
If you like any of the project code consider donating.  
BTC: 32LxoJWQvUJbZsJY2ZBqopoCCELigfzFy3  
ETH: 0x9a0661d3FE5110a40685bdF9F329eF1f159F2482  
XTZ: tz1PBFLc4PeQnkjneXKjS8o7rWNK5zNaLjGa  
BNB: bnb1mtxsz94u4xvj5z5ste6t2n9y50fg0w4vy7u0v4  

---
## License
This project is licensed under the [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/).

---
## Disclaimer
### No Investment Advice Provided
USE THE SOFTWARE AT YOUR OWN RISK. YOU ARE RESPONSIBLE FOR YOUR OWN MONEY. ALL TRADING INVOLVES HIGH RISK AND YOU CAN LOSE A SUBSTANTIAL AMOUNT OF MONEY, NO MATTER WHAT METHOD YOU USE. THE AUTHOR HAS NO RESPONSIBILITY FOR YOUR TRADING RESULTS. YOU SHOULD ALWAYS UNDERSTAND THAT PAST PERFORMANCE IS NOT NECESSARILY INDICATIVE OF FUTURE RESULTS.
