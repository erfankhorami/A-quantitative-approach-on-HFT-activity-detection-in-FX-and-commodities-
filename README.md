INSTITUTIONAL FOOTPRINT & ORDER FLOW INTENSITY (OFI)

This notebook implements a quantitative market microstructure analysis framework
designed to identify institutional participation, HFT absorption, and iceberg-style
order behavior using tick-level data.

The analysis combines volume profile theory, statistical anomaly detection,
machine learning (Isolation Forest), and order flow aggregation into a single,
interactive visualization.

-----------------------------------------------------------------------

CORE COMPONENTS

1. Volume Profile (VP)
   - Tick-weighted volume distribution
   - Point of Control (POC)
   - Value Area High / Low (VAH / VAL)

2. HFT Absorption Detection
   - Isolation Forest applied to rolling volatility and duration
   - Identifies low-volatility, high-participation absorption zones

3. Heat Bubble Anomalies
   - Z-score based log-return spikes
   - Bid and ask side differentiation
   - Visual intensity proportional to statistical impact

4. Order Flow Intensity (OFI)
   - Aggregates anomaly intensity over fixed time windows
   - Normalized intensity classification:
       * Noise
       * Institutional
       * Iceberg

5. Interactive Visualization
   - Multi-timeframe candlesticks
   - Toggleable analytical layers
   - Dedicated OFI histogram subplot

-----------------------------------------------------------------------

DATA SOURCE

- MetaTrader 5 tick data
- Requires MetaTrader 5 running and logged in
- Results depend on broker tick quality and liquidity

-----------------------------------------------------------------------

INTENDED USE

This project is intended for:
- Market microstructure research
- Institutional footprint analysis
- Quantitative trade context analysis

This is NOT:
- A trading bot
- A signal generator
- A financial recommendation

-----------------------------------------------------------------------

NOTES

- The notebook is research-grade and exploratory
- Parameters are instrument-specific and must be tuned
- Designed for high-frequency and intraday analysis

-----------------------------------------------------------------------

LICENSE

Private research use unless explicitly stated otherwise by the author.
