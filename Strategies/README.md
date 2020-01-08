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
