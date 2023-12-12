# Gold Digger EA MT4

[![Forex Robot Easy](https://forexroboteasy.com/wp-content/uploads/2019/05/forex-robot-easy-logo.png)](https://forexroboteasy.com/forex-robot-review/gold-digger-ea-mt4-review-profitable-night-trade-forex-software/)

Gold Digger EA MT4 is an Expert Advisor developed by the Forex Robot Easy Team. It is designed for highly profitable gold scalping during night-time Forex trading sessions. This EA uses a fixed Stop Loss and Take Profit strategy to ensure risk management and maximize profits.

## Features

- Fixed Stop Loss and Take Profit values in points
- Hidden Take Profit value for better risk management
- Adjustable trading lot size

## How it Works

The Gold Digger EA MT4 operates during night-time Forex trading between 22:00 and 06:00. It uses the `OnTick()` function to check if it is night-time. If it is, the EA calculates the desired profit level based on the current Ask price and the Hidden Take Profit value. If the Bid price reaches or exceeds the profit level, all open trades are closed using the `CloseAllTrades()` function. If the profit level is not reached, a new trade is opened using the `OpenTrade()` function.

The `IsNightTime()` function checks if the current hour falls within the night-time range. If it does, the function returns true; otherwise, it returns false.

The `CloseAllTrades()` function iterates through all open orders and closes them using the `OrderClose()` function. It uses the Bid price as the closing price and applies a predefined slippage value.

The `OpenTrade()` function calculates the stop loss and take profit levels based on the current Bid price, the Stop Loss and Take Profit values, and the Point value. It then opens a buy trade using the `OrderSend()` function.

## Product Description

Gold Digger EA MT4 is a highly profitable Expert Advisor designed for night-time Forex trading sessions. It scalps the gold market using a fixed Stop Loss and Take Profit strategy, ensuring risk management and maximizing profits. With adjustable trading lot size, traders can customize their risk-reward ratio according to their preferred trading style.

Please note that Forex Robot Easy is not the official developer of this product. We provide this sample code as an example of how the Gold Digger EA MT4 can work as described in the product. To find the official developer and access detailed reviews and trading results of this product, please visit [Forex Robot Easy - Gold Digger EA MT4 Review](https://forexroboteasy.com/forex-robot-review/gold-digger-ea-mt4-review-profitable-night-trade-forex-software/). For further information and support, please refer to MQL5, the official platform for expert advisor development.
