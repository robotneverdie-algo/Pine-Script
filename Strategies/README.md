# Strategies

A collection of trading strategies.

---
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
> Notes:
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

* [Requested 002 Strategy](/Strategies/Requested%20002%20Strategy.pine)
> Requested strategy by discord user IamLegion#6493. [1]
> * Trend Following - 2 Higher Timeframe Moving Average. [2]
> * Trend Confirmation - 2 Lower Timeframe Moving Average. [2]
> * Entry/Exit - Entry: 2 Moving Average, Connors RSI, Stochastic %K & %D and Bollinger BandWidth Exit: MACD and RSI
> * Stop-Loss and Profit-Taking - Fix Percentage, ATR Percentage  
>
> References/Notes:  
> [1] Strategy mainly use for backtesting setting for ProfitTrailer bot.  
> [2] Use for turning on the bot.  
