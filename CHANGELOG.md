# Changelog

All notable changes to DeltaVolumeProfileX (DELTAVP).

## 3.0.0 — 2026-08

First public release.

- Tick-accurate volume-at-price built from real trades (Tick Replay used when available for
  exact historical bid-ask delta; tick-rule fallback otherwise).
- POC, Value Area (VAH/VAL), traded range high/low and VWAP, each independently styleable.
- Three profiling modes: automatic sessions, Trading-Hours template, and custom time window.
- Interactive manual window (drag to move / resize, optional anchor-to-last-bar).
- Row Size (ticks) to match another profile's resolution.
- Correct on time, Renko, Range, Tick and Volume bars.
- Real-time design: O(1) per trade, snapshot-based rendering, bounded memory.
- Optional on-profile totals (volume / delta) for numeric comparison against other profiles.

_Distributed as a protected, obfuscated assembly. Source is not public._
