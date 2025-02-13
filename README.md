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

## Emini Player Zones

Zone visualization indicator for ES/SPX trading.

### Features
- Multi-symbol support (ES/MES, SPX/US500)
- Dynamic color zones:
  - Green: Price above zone
  - Red: Price below zone
  - White: Price within zone
- Configurable market hours
- Optional zone extension (left/right)
- ES-SPX price adjustment
- CSV input format: Low,High,_,Type
- Raw zone type labels displayed directly

### Example Input
```
4500,4505,,bcz
4510,4515,,ir
4520,4525,,is
```

## License
Mozilla Public License 2.0
