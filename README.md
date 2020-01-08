# Pine Script

A library of trading indicators, strategies and code snippets for Pine Script programming language.

---
## Strategies
* [Template Simple Strategy](/Strategies/Template%20Simple%20Strategy.pine)
> An simple long/short strategy template file.

* [Template Simple Strategy](/Strategies/Template%20Advance%20Strategy.pine)
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

---
## Indicators

---
## Snippets

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
