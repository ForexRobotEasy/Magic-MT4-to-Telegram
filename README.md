# Magic MT4 to Telegram

This code is a sample implementation of a program that sends real-time updates of trading positions from MetaTrader 4 (MT4) to Telegram. It utilizes the Telegram API to send messages to a specific chat ID.

## How it works

1. The code includes the necessary Telegram library `Telegram.mqh`.
2. Global variables `token` and `chatID` are declared. These variables should be replaced with the Telegram bot token and chat ID obtained from the Telegram BotFather.
3. The `sendTelegramMessage` function is defined to send a message to Telegram. It creates an instance of the `CTgBot` class, sets the Telegram bot token and chat ID, and then sends the message using the `SendMessage` method.
4. The `checkTradingPositions` function is defined to check for changes in trading positions. It first checks if trading is allowed using the `IsTradeAllowed` function.
5. If trading is allowed, it proceeds to get the number of open positions using `OrdersTotal`.
6. If there are open positions, it iterates through each position and checks if it has been closed. If a position has been closed, it sends a notification to Telegram using the `sendTelegramMessage` function.
7. The `OnStart` function is the entry point of the program. It calls the `checkTradingPositions` function to check for changes in trading positions.

## Product Description

**Magic MT4 to Telegram** is a software tool developed by the Forex Robot Easy Team that allows traders to receive real-time updates of their trading positions on the MT4 platform through the Telegram messaging app.

With Magic MT4 to Telegram, traders can stay informed about the status of their trades without the need to constantly monitor their trading platform. The program sends notifications to a specified Telegram chat whenever a trading position is closed.

Key Features:
- Real-time updates: Get instant notifications of closed trading positions directly on your Telegram app.
- Easy setup: Simply replace the provided Telegram bot token and chat ID with your own and you're ready to receive updates.
- Customizable messages: Modify the message content sent to Telegram to suit your preferences.

Please note that ForexRobotEasy is not the official developer of Magic MT4 to Telegram. We provide this sample code to demonstrate how the product works. To find the official developer and learn more about the product, please visit the official website at [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/magic-mt4-to-telegram-review-real-time-forex-updates/).

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/magic-mt4-to-telegram-review-real-time-forex-updates/).
