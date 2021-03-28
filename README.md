# What is this?

MT5 EA

日本語ドキュメント[README.ja.md](README.ja.md)

# Installation

1. regist <a href="https://clicks.affstrack.com/c?c=574014&l=ja&p=0">XMtrading</a> Standard type is recommended
1. Download and install <a href="https://clicks.affstrack.com/c?c=574014&l=ja&p=4">MetaTrader 5</a>
1. Installation [PhaseShift.ex5](PhaseShift.ex5) for MT5 EA Directory
1. Recommended currency USDJPY And Chart is M1
1. run <b>XMTrading MT5</b> 
1. Tools => Opstions => Expert Advisors => 『Allow WebRequest for listed URL:』 add `https://jw0tzq2rp3.execute-api.ap-northeast-1.amazonaws.com`



# Parameters

| Parameter name | means |
|--|--|
|EA_Magic| Magic number |
|Lot| Number of lots used in one order|
|TotalLotLimit|TotalLotLimit|
|TotalPosLimit|TotalPositionLimit|
|StopLoss|StopLoss(point)|
|TakeProfit|TakeProfit(point)|
|ResetProfit|ResetProfit (point) <small>(※1)</small>|
|MaPeriod|MovingPeriod for calculating the Average (moving average) index|
|AdxPeriod|Period for calculating ADX (Average Directional Movement) indicators|
|TradeWait|Waiting time for the next order with the same magic number  <small>(※2)</small>|
|SellAdx|ADX value to be judged at the time of sell order|
|BuyAdx|ADX value to be judged at the time of ordering|

#### ※1 If Profit falls below this value, it is unlikely that you will make a profit. TakeProfit is set to the same as the bid / ask price, TakeProfit is set to 0, and the position is closed the moment Profit becomes 0.
####  ※2 Even with the same magic number, buy orders and sell orders are distinguished, so you can order at the same time even during wait.
# Inquiry and Bugs

This Repository <a href="https://github.com/kiyomasa-sato-0519/PhaseShift/issues">issues</a>

# At your own risk

Good luck
