# 🏀 ShotSense: Take smarter shots

**AQX Sports Analytics Data Bowl 4.0 submission**

A zero-install web tool that answers one question: *is a player or team taking shots from the most efficient zones?*

## Solution
Upload a shot-level CSV (`player,x,y,made`, NBA court coordinates). The tool classifies every shot into 5 zones (rim, paint, mid-range, corner 3, above-break 3), computes FG% and points-per-shot per zone, draws a shot chart, and simulates how many points are gained by shifting 10% of shots out of the mid-range into the shooter's most efficient zone.

## Features
- Per-player or whole-team analysis
- Shot chart (makes in green, misses in red)
- Points-per-shot by zone
- "What if" shot-mix simulation
- Runs entirely in the browser (no backend), works on GitHub Pages

## Impact
Coaches and analysts can quickly spot inefficient shot habits and quantify the potential gain in points per 100 shots.

## Run
Open `index.html`, or enable GitHub Pages. A synthetic demo dataset is built in (randomly generated, not real data). Real data: `nba_api` ShotChartDetail (LOC_X, LOC_Y, SHOT_MADE_FLAG).

## Limitations
The simulation assumes shooting % stays constant and ignores defense and shot difficulty.
