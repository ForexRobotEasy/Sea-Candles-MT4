# Sea Candles MT4

Sea Candles MT4 is a forex trading expert advisor developed by the Forex Robot Easy Team. It is a software that utilizes the CCI (Commodity Channel Index) oscillator to generate trading signals based on the CCI values and moving average (MA) thresholds.

## Global Variables and Constants

The code starts with defining a global variable and constant. The `CCI_RANGE` constant is set to 100, which will be used later in the code.

## CCI Oscillator Calculation

The `CalculateCCI` function calculates the CCI value for a given period. It calculates the sum of the difference between the closing price and the moving average over the specified period. Then, it calculates the mean deviation and uses it to calculate the CCI value. The CCI value is returned.

## Moving Average Calculation

The `CalculateMovingAverage` function calculates the simple moving average (SMA) for a given period. It uses the `iMA` function provided by the MQL5 platform to calculate the SMA. The SMA value is returned.

## Signal Generation

The `GenerateSignal` function generates trading signals based on the CCI and MA values. It takes the period, CCI threshold, and MA threshold as parameters. It calculates the CCI and MA values using the previously defined functions. If the CCI value is above the CCI threshold and the closing price is below the MA minus the MA threshold, a buy signal is generated. If the CCI value is below the negative CCI threshold and the closing price is above the MA plus the MA threshold, a sell signal is generated. The function returns true if a signal is generated, otherwise false.

## Classic Divergence Identification

The `IdentifyClassicDivergence` function identifies classic divergence based on the previous and current high values and CCI values. It calculates the previous and current high values and CCI values using the previously defined functions. If the current high value is higher than the previous high value and the current CCI value is lower than the previous CCI value, a classic divergence is identified. The function returns true if a classic divergence is identified, otherwise false.

## Overbought and Oversold States Detection

The `DetectOverboughtOversoldStates` function detects overbought and oversold states based on the CCI value and a specified threshold. It calculates the CCI value using the previously defined function. If the CCI value is above the threshold or below the negative threshold, an overbought or oversold state is detected. The function returns true if an overbought or oversold state is detected, otherwise false.

## Candlestick Visualization

The `VisualizeCandlesticks` function is responsible for visualizing candlesticks. The code to visualize candlesticks is not provided in the given code snippet.

## Notification System

The `SendNotification` function is responsible for sending notifications. The code to send notifications is not provided in the given code snippet.

## Expert Advisor

The `OnTick` function is the main function of the expert advisor. It is executed on each tick of the price. It generates trading signals, identifies classic divergence, and detects overbought or oversold states based on the defined criteria. If any of these conditions are met, it visualizes candlesticks and sends notifications.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 platform.

For detailed reviews and trading results of this product, you can visit [here](https://forexroboteasy.com/forex-robot-review/sea-candles-mt4-review-cci-oscillator-based-forex-software/).
