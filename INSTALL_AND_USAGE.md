# DeltaVolumeProfileX (DELTAVP)

**Copyright © 2026 Mohamed Abdelaziz. All rights reserved.**
Website: https://mohamed-abdelaziz.com/en
Licensed software — see `LICENSE_EULA.txt`. Copying, redistribution, resale or reverse
engineering is prohibited.

---

## What it is

A tick-accurate **session / range volume profile** for NinjaTrader 8 that shows where volume
actually traded, with **bid-ask delta**, **POC**, **VAH/VAL** (value area), the **traded range
high/low**, and **VWAP**. Volume-at-price is built from real trades — not from bar volume — so
the distribution reflects real business done at each price.

**It is an analytical tool. It is not financial advice and does not guarantee any result.
Trading futures involves substantial risk.**

## Key features

- Tick-accurate volume-at-price; exact **historical bid/ask delta** when Tick Replay is on.
- Automatic **session profiles** (instrument sessions, a Trading Hours template, or a custom
  time window) and a drag-resizable **manual window**.
- POC / Value Area / Range / VWAP levels, each independently styleable and extendable.
- Works on time, Renko, Range, Tick and Volume bars (Tick Replay recommended for non-time bars).

## Install

1. Close NinjaTrader.
2. Copy `DeltaVolumeProfileX.dll` into:
   `Documents\NinjaTrader 8\bin\Custom\`
3. Start NinjaTrader.
4. On a chart: **Indicators → DeltaVolumeProfileX → Add**.

> Do **not** place any `.cs` source of this indicator in `bin\Custom\Indicators\` at the same
> time — NinjaTrader would compile a duplicate type and refuse to load.

## Recommended setup

- Enable **Tick Replay** on the chart's Data Series for exact historical delta and precise
  attribution on Renko/Range/Tick bars.
- For results that match another volume profile, set **Row Size (ticks)** to the same tick
  resolution that profile uses.

## Key settings

| Group | Setting | Purpose |
|-------|---------|---------|
| 1. Volume | Row Size (ticks) | Histogram resolution — match it to any profile you compare against |
| 1. Volume | Value Area % | Value-area coverage (default 70) |
| 2. Delta | Delta Source | Bid/Ask (needs Tick Replay historically) or Tick Rule |
| 3. Lines | POC / Value area / Range / VWAP | Colour, style, width, visibility, extend |
| 5. Session / Window | Profile Mode | Sessions vs a single Manual Window |
| 5. Session / Window | Trading hours | Data-series sessions, a template, or a custom window |
| 5. Session / Window | Anchor To Last Bar | Keep the manual window pinned to the latest bar |
| 6. Style | Show Totals | Print total volume / delta under each profile |

## Support

https://mohamed-abdelaziz.com/en
