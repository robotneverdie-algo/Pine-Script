# Snippets

A collection of code snippets for Pine Script programming language.

---
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

* [Ticker](/Snippets/Ticker.pine)
>  Find if current ticker has quote currency. [1]
>
>  References/Notes:  
>  [1] Base currency must have three letters
