# Clock GMT Live MT4

This code provides a custom indicator for MetaTrader 4 (MT4) that displays the GMT time offset of the broker, the local time of the trader, and the ping of the broker. The indicator updates this information in real-time and can be used to optimize forex trading based on real-time broker information.

## How It Works

The code consists of several functions and event handlers:

1. **GetGMTOffset()**: This function retrieves the GMT time offset from the broker using the `TimeGMTOffset()` function and displays it in a user-friendly format using the `Print()` function.

2. **GetLocalTime()**: This function retrieves the local time of the trader using the `TimeLocal()` function and displays it in a user-friendly format using the `Print()` function.

3. **GetBrokerPing()**: This function retrieves the ping of the broker using the `TerminalInfoInteger()` function with the `TERMINAL_PING` parameter and displays it in a user-friendly format using the `Print()` function.

4. **OnInit()**: This event handler is called when the indicator is initialized. It calls the `GetGMTOffset()`, `GetLocalTime()`, and `GetBrokerPing()` functions to retrieve and display the initial values. It also sets a timer using the `EventSetTimer()` function to refresh the information every 60 seconds.

5. **OnTimer()**: This event handler is called when the timer set in the `OnInit()` function expires. It refreshes the GMT time offset, local time, and broker ping by calling the corresponding functions.

6. **OnDeinit()**: This event handler is called when the indicator is deinitialized. It clears the timer using the `EventKillTimer()` function and displays a message using the `Print()` function.

## Product Description

Clock GMT Live MT4 is a custom indicator for MetaTrader 4 (MT4) that provides real-time information about the GMT time offset of the broker, the local time of the trader, and the ping of the broker. This information is essential for optimizing forex trading strategies based on the current broker conditions.

With Clock GMT Live MT4, traders can easily monitor the time offset between their broker and GMT, ensuring accurate timing for their trades. The indicator also displays the local time of the trader, allowing them to keep track of market sessions and important trading events.

In addition, Clock GMT Live MT4 provides the ping of the broker, which indicates the latency or delay in executing trades. By monitoring the broker's ping, traders can assess the speed and reliability of their trading platform, enabling them to make more informed trading decisions.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that demonstrates how this indicator can work. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/clock-gmt-live-mt4-review-optimize-forex-trading-with-real-time-broker-info/).
