# Contributing

Contributions and reproducible bug reports are welcome.

## Before submitting an issue

Include the **ticker/exchange, market, timeframe, session, chart type, OHLC feed/adjustment choice**, relevant input settings, and the expected versus observed result. For compiler issues, include the exact Pine Editor error and line number. Please do not upload private account information or licensed proprietary indicator source.

## Pull requests

1. Keep the Pine indicator in `OutsizedAlpha_TD_Sequential_Combo_Reviewed.pine` and update the README/CHANGELOG where behaviour changes.
2. Separate signal calculations from drawing/viewport changes where possible.
3. Describe which published rule supports the change. Where source definitions vary, expose the choice and document its default rather than silently claiming official parity.
4. Supply a deterministic OHLC reproduction for signal changes and compare events before and after modification.
5. Regression-check Setup 9, deferred Sequential 13, Combo Setup validation and promotion, cancellation against originating TDST, later perfection, recycling, qualified/disqualified TDST breaks, and viewport-independent engine state.
6. Declare whether the proposed file has been **compiled in the native TradingView Pine Editor**. Independent Pine runtimes are useful checks but not certification.
7. Keep the existing MPL-2.0 notice in all modified files and respect third-party IP and trademarks.

## Scope

This is an independent public research implementation. Please do not submit leaked, reverse-extracted or proprietary Symbolik/DeMARK source as a contribution. Feature requests should be framed as independently implemented, verifiable rules.
