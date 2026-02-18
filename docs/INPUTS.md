# Inputs reference

This file is a quick index of the main inputs grouped as they appear in TradingView.

## Break Confirmation / Fakeout Filter

| Variable | Type | Label |
|---|---|---|
| `useFakeoutFilter` | `bool` | Allow False Break (Reclaim) Filter |
| `showLockedActionLine` | `bool` | Show Active Locked Action Line |
| `reclaimBars` | `int` | Reclaim Window (bars) |
| `reclaimCloses` | `int` | Reclaim Requires Consecutive Closes |
| `confirmCloses` | `int` | Confirm Requires Consecutive Closes |

## HTF Confluence Overlay

| Variable | Type | Label |
|---|---|---|
| `showHTF` | `bool` | Enable HTF Confluence |
| `showDaily` | `bool` | Show Daily Lines |
| `show4H` | `bool` | Show 4H Lines |
| `show1H` | `bool` | Show 1H Lines |
| `showHTFLabels` | `bool` | Show Confluence Labels |
| `useHTFGate` | `bool` | Gate Entries by HTF Confluence |
| `minHTFScore` | `int` | Min Confluence Score (0-3) |
| `gateMode` | `string` | Bias |
| `gateTolATRMult` | `float` | Bias Tolerance (ATR Mult) |
| `gateNearATRMult` | `float` | Near Distance (ATR Mult) |
| `alignTolMult` | `float` | Alignment Tolerance (ATR Mult) |
| `nearMult` | `float` | Near Price Filter (ATR Mult) |
| `nBack` | `int` | Path Check Bars Back (chart bars) |
| `backTolMult` | `float` | Back-Point Tol Mult |
| `useThirdScore3` | `bool` | Score=3 uses 3-point path check |
| `htfMaxPivots` | `int` | Max Pivots per HTF |
| `fadeByDistance` | `bool` | Fade Opacity with Distance |

## Safety Line (Exit)

| Variable | Type | Label |
|---|---|---|
| `postMaxPivots` | `int` | Max Post-Entry Pivots |
| `safetyMinTouches` | `int` | Min Touches (Safety Diagonal) |
| `minSpacingSafety` | `int` | Min Bars Between Safety Pivots |
| `require2PostPivots` | `bool` | Require 2 Post-Entry Pivots for Diagonal |
| `ratchetSafety` | `bool` | Ratchet Safety (Only Tighten) |
| `ratchetHystATR` | `float` | Ratchet Hysteresis (ATR) |
| `useBootstrapStop` | `bool` | Bootstrap Safety Stop (Immediate) |
| `bootstrapMode` | `string` | EntryCandle |
| `bootstrapATRMult` | `float` | Bootstrap ATR Mult |

## Shape Senator (Triangles / Wedges)

| Variable | Type | Label |
|---|---|---|
| `enableShapes` | `bool` | Enable Shape Senator |
| `showShapeLabels` | `bool` | Show Shape Label |
| `showShapeBounds` | `bool` | Show Shape Boundaries |
| `showShapeFill` | `bool` | Show Shape Fill (polyline) |
| `fillTransparency` | `int` | Fill Transparency (0-100) |
| `showShapeProj` | `bool` | Show Shape Projection (dotted) |
| `projBars` | `int` | Projection Bars |
| `shapeFilterMode` | `string` | Off |
| `minShapeConf` | `float` | Min Shape Confidence |
| `maxApexBars` | `int` | Max Apex Distance (bars) |
| `compressRatio` | `float` | Compression Threshold (gapNow/gapThen) |
| `flatMult` | `float` | Flat Slope Threshold (ATR / 100 bars) |
| `shapeTolMult` | `float` | Breakout Strength (ATR) |

## Tolerances / Filters / Visuals

| Variable | Type | Label |
|---|---|---|
| `atrLen` | `int` | ATR Length |
| `touchMult` | `float` | Action Touch Tolerance (ATR) |
| `safetyTouchMult` | `float` | Safety Touch Tolerance (ATR) |
| `slMult` | `float` | Safety Buffer (ATR) |
| `breakConfirmATR` | `float` | Break Strength Req (ATR, 0=off) |
| `useDistAction` | `bool` | Use Distance Filter (Action) |
| `maxActionDistATR` | `float` | Max Action Line Distance (ATR) |
| `useDistSafety` | `bool` | Use Distance Filter (Safety) |
| `maxSafetyDistATR` | `float` | Max Safety Line Distance (ATR) |
| `useBarBreachCheck` | `bool` | Validate 'No Poke-Through' on ALL bars |
| `barBreachMaxBars` | `int` | Max Bars to Validate (cap) |
| `barBreachStep` | `int` | Validation Step (1=every bar) |
| `breachUseWicks` | `bool` | Breach uses Wicks (High/Low) vs Close |
| `deleteDynOnEntry` | `bool` | Delete Dynamic Lines on Entry |
| `showLabels` | `bool` | Show Labels |
| `showDynLines` | `bool` | Show Pending Lines |
| `showSafetyRay` | `bool` | Show Safety Ray |
| `debugSafety` | `bool` | DEBUG: Plot Effective Safety |

## Trade Review

| Variable | Type | Label |
|---|---|---|
| `keepLastBreakLine` | `bool` | Keep Last Break Trendline After Exit |
| `freezeBreakAtExit` | `bool` | Freeze Last Break Line at Exit |

## Trendline Settings (Entry)

| Variable | Type | Label |
|---|---|---|
| `leftBars` | `int` | Pivot Left Bars |
| `rightBars` | `int` | Pivot Right Bars |
| `maxPivots` | `int` | Max Global Pivots to Scan |
| `minTouches` | `int` | Min Touches (Action Line) |
| `minSpacingAction` | `int` | Min Bars Between Action Pivots |

