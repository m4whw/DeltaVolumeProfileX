<div align="center">

# DeltaVolumeProfileX (DELTAVP)

**Tick-accurate volume profile with bid-ask delta for NinjaTrader 8**

POC · Value Area (VAH/VAL) · Traded Range · VWAP · Session, Template & Manual-Window profiles

[![Platform](https://img.shields.io/badge/platform-NinjaTrader%208-1f6feb)](https://ninjatrader.com)
[![Version](https://img.shields.io/badge/version-3.0.0-2ea043)](CHANGELOG.md)
[![License](https://img.shields.io/badge/license-Proprietary-red)](LICENSE.txt)

[**Download**](dist/DeltaVolumeProfileX.dll) · [Install & Usage](INSTALL_AND_USAGE.md) · [Website](https://mohamed-abdelaziz.com/en) · [License](LICENSE.txt)

</div>

---

## Overview

**DeltaVolumeProfileX** shows *where volume actually traded* — not where price simply spent
time. Volume-at-price is built from **real trades** (Tick Replay used when available for exact
historical bid-ask delta), so every profile reflects the real auction: the **Point of Control**,
the **Value Area** (VAH/VAL), the **traded range** high/low, and **VWAP**.

<div align="center">
<img src="assets/screenshot-1.jpg" alt="DeltaVolumeProfileX on a NinjaTrader chart" width="80%">
</div>

## Features

- **Tick-accurate** volume-at-price from real trades — never bar volume.
- **True bid-ask delta**, exact historically when Tick Replay is enabled; tick-rule fallback otherwise.
- **POC / Value Area / Range / VWAP** levels — each independently coloured, styled, extended.
- **Three profiling modes:** automatic session profiles, a Trading-Hours **template**, or a custom time window.
- **Interactive manual window** — drag to move, drag the edges to resize, optional anchor-to-last-bar.
- **Row Size (ticks)** to match the resolution of any profile you compare against.
- Works on **time, Renko, Range, Tick and Volume** bars (Tick Replay recommended for non-time bars).
- Built for real-time: O(1) per trade on the hot path, snapshot-based rendering, flat memory.

<div align="center">
<img src="assets/screenshot-2.jpg" alt="Session profiles with delta" width="80%">
</div>

## Install

1. Close NinjaTrader.
2. Download [`dist/DeltaVolumeProfileX.dll`](dist/DeltaVolumeProfileX.dll) and copy it into:
   `Documents\NinjaTrader 8\bin\Custom\`
3. Start NinjaTrader → on a chart: **Indicators → DeltaVolumeProfileX → Add**.

Full steps and recommended settings: **[INSTALL_AND_USAGE.md](INSTALL_AND_USAGE.md)**.

> Enable **Tick Replay** on the chart's Data Series for exact historical delta and precise
> attribution on Renko/Range/Tick bars.

## Compatibility

| | |
|---|---|
| Platform | NinjaTrader 8 (8.1.x) |
| Instruments | Any (futures, stocks, forex, crypto CFDs) — tuned for NQ / ES / Gold |
| Data | Tick Replay recommended; works without it using the tick rule |

## License

Proprietary and commercial. **Licensed, not sold.** Copying, modification, reverse engineering,
redistribution, resale or sub-licensing is prohibited without written permission. See
[LICENSE.txt](LICENSE.txt).

This indicator is an **analytical tool only** — it is not financial advice and does not guarantee
any result. Trading futures involves substantial risk.

---

<div align="center">

**© 2026 Mohamed Abdelaziz** · [mohamed-abdelaziz.com](https://mohamed-abdelaziz.com/en)

<sub>نسخة عربية مختصرة: مؤشر بروفايل حجم دقيق على مستوى التِك مع دلتا العرض/الطلب لـ NinjaTrader 8 —
POC وVAH/VAL والمدى وVWAP، بأوضاع جلسات وقالب توقيت ونافذة يدوية. أداة تحليلية فقط وليست ضمان ربح.
منتج تجاري مرخّص — يُمنع النسخ أو إعادة التوزيع أو الهندسة العكسية. التحميل من مجلد dist والتعليمات في
ملف التثبيت.</sub>

</div>
