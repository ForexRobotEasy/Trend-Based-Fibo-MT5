# Trend Based Fibo MT5 ReadMe File

This code is a custom indicator for MetaTrader 5 (MT5) called Trend Based Fibo MT5. It is developed by the Forex Robot Easy Team and can be found on their website [forexroboteasy.com](https://forexroboteasy.com).

## Input Parameters

1. **fiboLevels** (default = 7): Number of Fibonacci levels to be calculated.
2. **timeframe** (default = PERIOD_CURRENT): Chart timeframe for the indicator.
3. **priceType** (default = PRICE_CLOSE): Price type used for calculating Fibonacci levels.

## Global Variables

- **fiboLevelsArray**: Array to store the calculated Fibonacci levels.

## Initialization Function

The `OnInit()` function is responsible for initializing the custom indicator. It calls the `CalculateFiboLevels()` function to calculate the Fibonacci levels.

## Deinitialization Function

The `OnDeinit()` function is called when the indicator is removed from the chart. It can be used for cleaning up any resources or variables used by the indicator.

## Iteration Function

The `OnCalculate()` function is called for each new tick or bar on the chart. It also calls the `CalculateFiboLevels()` function to recalculate the Fibonacci levels.

## Calculate Fibonacci Levels

The `CalculateFiboLevels()` function calculates the Fibonacci levels based on the specified input parameters. It first determines the start and end index based on the timeframe. Then, it iterates through the Fibonacci levels and calculates each level based on the high and low prices of the specified timeframe.

## Indicator Properties

The `GetIndicatorName()` function returns the name of the custom indicator as 'Trend Based Fibo MT5'.

The `GetIndicatorAuthor()` function returns the name of the developer as 'Forex Robot Easy Team'.

## Indicator Settings

The `GetIndicatorSettings()` function prints the indicator settings to the console, including the number of Fibonacci levels, the selected timeframe, and the price type.

---

**Product Description**

This code represents a custom indicator called Trend Based Fibo MT5. It is developed by the Forex Robot Easy Team and can be used in MetaTrader 5 (MT5) trading platform. 

The Trend Based Fibo MT5 indicator calculates Fibonacci levels based on the high and low prices of the specified timeframe. It allows traders to identify potential support and resistance levels in the market.

To use this indicator, simply add it to the chart in MT5 and configure the input parameters such as the number of Fibonacci levels, timeframe, and price type. The indicator will then automatically calculate and plot the Fibonacci levels on the chart.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that demonstrates how the indicator works. For detailed reviews and trading results of this product, visit the official developer's website at [forexroboteasy.com](https://forexroboteasy.com). For any further information or support regarding this indicator, please refer to the official developer using MQL5.
