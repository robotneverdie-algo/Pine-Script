# Pine Script

A library of trading indicators, strategies and code snippets for Pine Script programming language.

---
## Strategies
* [Template Simple Strategy](/Strategies/Template%20Simple%20Strategy.pine)
> ###### An simple long/short strategy template file.

* [Template Advance Strategy](/Strategies/Template%20Advance%20Strategy.pine)
> ###### An advance long/short strategy template file.
> The template file layout an trend following trading system. [1] [2]
> * Trend Following - An indicator that identify trend's direction, most likely an moving average.
> * Trend Confirmation - Most trend following indicator are prone to whipsaw, so you what to confirm the movement with something like an momentum indicator.
> * Entry/Exit - Now that you have an trend directional bias you may want to find an optimal entry/exit strategy this is where overbought/oversold indicator come in handy.
> * Stop-Loss and Profit-Taking - We need to determine an method to take profit on a winning trade and an loss on an losing trade. [3]
> * Position Sizing - To control risk and maximize gains we must determine what size of a position we are willing to risk. [4]
>
> ###### References/Notes:  
> [1] https://www.babypips.com/learn/forex/design-your-trading-system  
> [2] https://www.investopedia.com/articles/forex/10/indicators-fx-traders-must-know.asp  
> [3] I provided an method using bollinger bands with an stop loss and three profit-taking price levels. Each time an tp level is hit you will reduce your position and move the stop-loss to the old price level.  
> [4] I use the formula: Position Size = Risk Amount / Distance to Stop Loss. https://medium.com/@cryptocreddy/comprehensive-guide-to-position-size-and-leverage-2e27764ce9e0

* [Example Advance Strategy](/Strategies/Example%20Advance%20Strategy.pine)
> ###### An example of an advance trend following strategy. [1]
> * Trend Following - Moving Average.
> * Trend Confirmation - Waddah Attar Explosion.
> * Entry/Exit - Fisher Transform.
>
> ###### References/Notes:  
> [1] If you wish to see re-entry results increase the Trades Count setting.

* [Requested 001 Strategy](/Strategies/Requested%20001%20Strategy.pine)
> ###### Requested strategy by discord user Mrhutqc#2962  
> A rewrite of Logical_Strat_Template_v0.2  
> \@author MrhutQC, Ozine  
> \@thanks DarkRico, FurryBoffin  
> * Trend Following - Higher Timeframe Moving Average.
> * Trend Confirmation - Waddah Attar Explosion.
> * Entry/Exit - Fisher Transform, Godmode Oscillator. https://www.tradingview.com/script/HL3vqXUM-Godmode-Oscillator-fresh-bread-generator-free-to-use/

* [Requested 002 Strategy](/Strategies/Requested%20002%20Strategy.pine)
> ###### Requested strategy by discord user IamLegion#6493. [1]
> * Trend Following - 2 Higher Timeframe Moving Average. [2]
> * Trend Confirmation - 2 Lower Timeframe Moving Average. [2]
> * Entry/Exit - Entry: 2 Moving Average, Connors RSI, Stochastic %K & %D and Bollinger BandWidth Exit: MACD and RSI
> * Stop-Loss and Profit-Taking - Fix Percentage, ATR Percentage  
>
> ###### References/Notes:  
> [1] Strategy mainly use for backtesting setting for ProfitTrailer bot.  
> [2] Use for turning on the bot.  

* [PSAR Strategy](/Strategies/PSAR%20Strategy.pine)
> ###### An trend strategy using Parabolic SAR.
> * Trend Following - A Moving Average.
> * Trend Confirmation - Parabolic SAR
> * Entry/Exit - None
> * Stop-Loss and Profit-Taking - ATR
> * Position Sizing - None

* [PSAR WT Strategy](/Strategies/PSAR%20WT%20Strategy.pine)
> ###### An trend strategy using Parabolic SAR and WaveTrend Oscillator.
> * Trend Following - Parabolic SAR.
> * Trend Confirmation - WaveTrend Oscillator.
> * Entry/Exit - IFish TCI Indicator
> * Stop-Loss and Profit-Taking - None
> * Position Sizing - None

* [Counter-Trend Strategy](/Strategies/Counter%20Trend%20Strategy.pine)
> ###### An counter-trend strategy finding tops/bottoms.  
> * Trend Following - Percentage Difference of Moving Average and Source, IFish TCI. [1]
> * Trend Confirmation - WaveTrend Oscillator
> * Entry/Exit - Sigma Accumulate
> * Stop-Loss and Profit-Taking - None
> * Position Sizing - None  
>
> ###### References/Notes:  
> [1] IFish TCI has static moving average (zlema) due to error: Script has too many local scopes.

---
## Indicators
### Momentum Indicators
##### These technical indicators may identify the speed of price movement
* [Fisher Transform Indicator](/Indicators/Momentum%20Indicators/Fisher%20Transform%20Indicator.pine)
> ###### Fisher Transform with an changeable EMA alpha https://www.mesasoftware.com/papers/UsingTheFisherTransform.pdf

* [Godmode Oscillator Indicator](/Indicators/Momentum%20Indicators/Godmode%20Oscillator%20Indicator.pine)
> ###### A rewrite of Godmode Oscillator https://www.tradingview.com/script/HL3vqXUM-Godmode-Oscillator-fresh-bread-generator-free-to-use/  
> \@author LazyBear, xSilas, Ni6HTH4wK

* [Trend Confirmation Index Indicator](/Indicators/Momentum%20Indicators/Trend%20Confirmation%20Index%20Indicator.pine)
> ###### TCI indicator presumed if the position of an close within a candlestick provides information on whether the uptrend is gaining or losing power.  
> A rewrite of Trend Confirmation Index http://www.fxcodebase.com/code/viewtopic.php?f=38&t=61051  
> \@author Mario Jemic

* [WaveTrend Oscillator Indicator](/Indicators/Momentum%20Indicators/WaveTrend%20Oscillator%20Indicator.pine)
> ###### A rewrite of WaveTrend Oscillator. https://www.tradingview.com/script/2KE8wTuF-Indicator-WaveTrend-Oscillator-WT/  
> \@author LazyBear

### Trend Indicators
##### These technical indicators measure the direction and strength
* [Moving Average Indicator](/Indicators/Trend%20Indicators/Moving%20Average%20Indicator.pine)
> ###### Moving average cross strategies with three type:
> Price Cross - When price cross the slow ma
> Two Cross - When fast ma cross the slow ma
> Tri Cross - When fast ma cross mid, slow ma

* [Waddah Attar Explosion Indicator](/Indicators/Trend%20Indicators/Waddah%20Attar%20Explosion%20Strategy.pine)
> ###### Waddah Attar Explosion with custom moving averages and exit strategies

* [MACD Line with Channel Bands Indicator](/Indicators/Trend%20Indicators/MACD%20Line%20with%20Channel%20Bands%20Indicator.pine)
> ###### A rewrite of Bollinger Bands on Macd https://www.tradingview.com/script/SG9NNwvz-Bollinger-Bands-on-Macd/
> © Dreadblitz

* [Momentum with Channel Bands Indicator](/Indicators/Trend%20Indicators/Momentum%20with%20Channel%20Bands%20Indicator.pine)
> ###### Momentum indicators with channel bands.
> Momentum out of channel bands, price is trending and if momentum in channel bands possible pause or reversal of the current trend.

### Volatility Indicators
##### These technical indicators measure the rate of price movement
* [Risk Bands Indicator](/Indicators/Volatility%20Indicators/Risk%20Bands%20Indicator.pine)
> ###### An standalone indicator version of the stop-loss and profit-taking from Template Advance Strategy.

### Volume Indicators
##### These technical indicators measure the strength of a trend based on volume

### Experimental Indicators
##### These technical indicators are experimental, usually combination of indicators.
* [IFish TCI Indicator](/Indicators/Experimental%20Indicators/IFish%20TCI%20Indicator.pine)
> ###### An inverse fisher transformation of TCI indicator http://www.fxcodebase.com/code/viewtopic.php?f=38&t=61051

* [Long/Short Ratio Levels Indicator](/Indicators/Experimental%20Indicators/Long%20Short%20Ratio%20Levels%20Indicator.pine)
> ###### Support/resistance levels based on spike in BTC long/short ratio, assuming green/red candles increase/decrease the long ratio, also dramatic increase/decrease in long ratio provide support/resistance levels.

* [Momentum Levels Indicator](/Indicators/Experimental%20Indicators/Momentum%20Levels%20Indicator.pine)
> ######  Support/Resistance levels with momentum indicators and channel bands.
> Momentum out of channel bands, price is trending and if momentum in channel bands possible pause or reversal of the current trend.
> These pause or reversal act as support/resistance levels.
>  
> ###### Color Schemes:
>  * Line: Trend Pause - Shape (circle) / Support (green) / Resistance (red)
>  * Line: Trend Reversal - Shape (circle) / Support/Resistance (yellow)

* [Sigma Accumulate Indicator](/Indicators/Experimental%20Indicators/Sigma%20Accumulate%20Indicator.pine)
> ###### Sigma (stdev) with money flow index and using bollinger bands to extrapolated the extremes in volatility and volume.
> ###### Color Schemes:
> * Column: Sigma Accumulate - Shape (columns) / Rising (blue) / Falling (purple) / Normal (gray)

---
## Snippets
* [Moving Average](/Snippets/Moving%20Average.pine)
> ###### An collection of moving averages used in the code base. [1]
> * alma - Arnaud Legoux Moving Average
> * cvwma - Coefficient of Variation Weighted Moving Average https://www.tradingview.com/script/0dBtJvhu-Stratus-DW/
> * dema - Double Exponential Moving Average
> * donchian - Donchian Middle Channel
> * ecema - Error Corrected EMA http://www.mesasoftware.com/papers/ZeroLag.pdf
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
> * zlema - Zero Lag Exponential Moving Average https://www.fmlabs.com/reference/default.htm?url=ZeroLagExpMA.htm
>
> ###### References/Notes:  
> [1] TradingView will slow down when their is a long chain of if/else statement, so have to split MA function.

* [Channel Bands](/Snippets/Channel%20Bands.pine)
> ###### An collection of channel bands used in the code base.
> * bollinger - Bollinger Bands
> * keltner - Keltner Channels
> * atr - Average True Range
> * donchian - Bollinger Bands
> * chandelier - Chandelier Exit

* [Momentum](/Snippets/Momentum.pine)
> ###### An collection of momentum indicator used in the code base.
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
> ###### References/Notes:  
> [1] Use PercentRank instead of ROC describe in ConnorsRSI Guidebook.  
> [2] Return K not %K: %K = sma(K, pk_len) %D = sma(%K, pd_len)

* [Ticker](/Snippets/Ticker.pine)
>  ###### Find if current ticker has quote currency.

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
