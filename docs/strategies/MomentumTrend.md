# MomentumTrend

Technical analysis based on BollingerBands (BB), Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD)

Looks for potential short term reversals at the top and bottom of the Bollinger Bands confirmed by RSI and MACD.

Closing your position is in your obligation. This strategy does not trigger `Close trade` signals, hence no notification is being sent out to the supported channels.

There are two occasion when a signal is triggered by this strategy:

Sell event:

```
BollingerBand was over upper band and now lower than previous value
RSI was over upper threshold and now lower than previous value
MACD Histogram confirmed by value decreasing
```

Buy event:

```
BollingerBand was under lower band and now higher than previous value
RSI was under lower threshold and now higher than previous value
MACD Histogram confirmed by value increasing
```

## Schedule

List of cryptocurrency pair and candle resolution combinations scheduled for technical analysis by the bot for this trading strategy:

```yaml
- pair: BNBUSDT
  resolution: 1h

- pair: ETHUSDT
  resolution: 1h

- pair: ADAUSDT
  resolution: 1h

- pair: XRPUSDT
  resolution: 1h

- pair: SOLUSDT
  resolution: 15m

- pair: DOTUSDT
  resolution: 1h

- pair: LTCUSDT
  resolution: 1h

- pair: MATICUSDT
  resolution: 1h

- pair: TRXUSDT
  resolution: 1h
```
