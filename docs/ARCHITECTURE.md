# Architecture

This indicator is structured as a single Pine Script file with clearly separated sections.

## Sections (high level)
1. **Inputs**: grouped UI inputs (Entry, Fakeout, Safety, HTF overlay, Shape Senator, etc.)
2. **Calcs & helpers**: ATR/tolerances + reusable line/label helpers
3. **HTF Confluence Overlay**: D / 4H / 1H trendline detection via `request.security()` and alignment scoring
4. **Pivot capture**: collects confirmed pivots into arrays (no lookahead; pivots confirm after `rightBars`)
5. **State machine**: trade state (`inTrade`, `tradeDir`, pending break confirmation)
6. **Action line engine**: finds best candidate trendline (touches, slope direction, breach checks)
7. **Shape Senator**: detects triangle/wedge compression patterns from active support/resistance lines
8. **Fakeout/confirm filter**: optional reclaim window before confirming entry
9. **Safety line & bootstrap stop**: immediate protective stop, then optional diagonal ratchet logic
10. **Trade review artifacts**: keep last break line, freeze at exit, etc.

## Design principles
- **Determinism**: pivots are only stored at confirmation (`bar_index - rightBars`), HTF uses `lookahead_off`.
- **Object hygiene**: uses persistent `line`/`label` handles and deletes when disabled.
- **Guards**: uses `not na(...)` checks before drawing.

See `docs/INPUTS.md` for the full parameter index.
