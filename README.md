# FPL TradingView Indicators

A collection of professional-grade TradingView indicators for SPX, SPY, and ES trading.

## FPL Cheatcode

Multi-timeframe moving average indicator with VWAP integration.

### Features
- 8 customizable moving averages across different timeframes
- Color-coded for easy identification:
  - Default timeframe: Blues (50/200 SMA/EMA)
  - Hourly: Yellow/Orange (20 EMA, 200 SMA)
  - Daily: Red theme (20 EMA, 200 SMA)
- VWAP with dotted line style
- Flexible MA types: SMA, EMA, SMMA, WMA, VWMA
- Customizable source and offset settings
- Smart timeframe handling

## SR Levels

Support and resistance level visualizer for multiple symbols.

### Features
- Multi-symbol support (SPX, SPY, ES/MES)
- Dynamic color zones:
  - Green: Price above zone
  - Red: Price below zone
  - White: Price within zone
- Fixed US market hours (9:30 AM - 4:00 PM)
- Optional zone extension
- CSV input format: Name,Symbol,Low,High

### Example Input
```
Support,SPY,450.5,451.0
Resistance,SPX,4505,4510
Gap Fill,ES,4500,4505
```

## License
Mozilla Public License 2.0
