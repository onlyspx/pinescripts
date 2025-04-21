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

## Hourly Range

Calculates and displays the high and low of the first hour of the US market session (9:30 AM - 10:30 AM ET). It also plots 1.5x and 2x range extensions based on this initial hour's range, providing potential price targets.

### Features
- Identifies first hour (9:30-10:30 ET) high and low.
- Plots 1.5x and 2x range extensions above the high and below the low.
- Customizable line styles and label visibility.
- Lines can be extended to the right.

## ORB (Opening Range Breakout)

Plots the Opening Range Breakout (ORB) levels based on a user-selected time period (5, 15, 30, or 60 minutes) after the market open. Includes optional price targets (multiples of the ORB range), breakout/retest signals, and customizable display options.

### Features
- Selectable ORB period (5, 15, 30, 60 mins or custom time).
- Plots ORB high and low.
- Optional price targets (0.5x, 1x, 1.5x, 2x, etc. of the ORB range).
- Optional display of ORB range shading and midpoint.
- Optional breakout and retest signals (BRB).
- Customizable colors and display settings.
- Timezone override for international users.

## PPP Levels

Allows users to input key trading levels (e.g., VPOC, support/resistance) and market profile levels for ES and NQ via CSV text areas. Plots these levels as customizable horizontal lines with labels on the chart.

### Features
- Input key levels via CSV (ES Level, Description).
- Input market profile levels via CSV (Description, ES Level, NQ Level).
- Plots levels as horizontal lines.
- Distinguishes VPOC levels with a different color.
- Plots ES and NQ profile levels with distinct colors.
- Customizable line style, width, and transparency.
- Toggle visibility for key levels and market profile levels separately.

## Prior Day/Week Levels

Displays various significant price levels including prior day high/low/open/close, prior week high/low/close, current day high/low/open, current week high/low/open, pre-market high/low, after-hours high/low, and the all-time high. Also includes two configurable Simple Moving Averages (SMAs).

### Features
- Plots numerous historical and current price levels.
- Includes pre-market and after-hours session highs/lows.
- Displays the calculated all-time high.
- Two configurable SMAs (default 20 and 200).
- Highly customizable visibility, colors, line styles, and widths for each level.
- Option to display levels only for the current day or extend across the chart.
- Price labels on the price axis.

## Smash Levels

Plots daily and weekly price levels for ES/SPX, and specific VIX levels, based on user-provided CSV data. Automatically adjusts ES levels based on the ES-SPX arbitrage difference input. Levels are color-coded based on price interaction.

### Features
- Input daily ES levels via CSV (Level, Label).
- Input weekly ES levels via CSV (Level, Label).
- Input VIX levels via CSV (Level, Label).
- Automatically detects symbol (ES, SPX, VIX) and adjusts levels accordingly.
- Applies ES-SPX arbitrage difference to levels when viewing SPX.
- Color-codes lines based on price interaction (green above, red below, white at level).
- Customizable line extension (left/right/none).
- Toggle visibility for daily and weekly levels.

## License
Mozilla Public License 2.0
