# Taghi/Gemini Sequential V9: A Pine Script® Indicator

This document provides an overview and instructions for using the "Taghi/Gemini Sequential V9" indicator, a Pine Script® tool designed for technical analysis on TradingView.

## What it Does

The Taghi/Gemini Sequential V9 is an advanced version of the widely used TD Sequential indicator, created to identify potential turning points in the market. It does this by counting a series of price bars that meet specific criteria. The indicator plots these counts directly on your chart, providing visual cues for potential trend exhaustion or reversal signals.

The indicator includes two main components:

- **Setup (1-9):** This phase looks for nine consecutive closes that are lower than the close four bars prior for a buy setup, or higher for a sell setup. A completed setup "9" is a key signal.
- **Countdown (1-13):** This phase begins after a completed setup. It counts bars based on a different set of rules, with a completed "13" often indicating a strong reversal signal.

## Key Features

This version includes several advanced features to enhance accuracy and customization:

- **Aggressive Countdown:** An option to use more sensitive criteria for the countdown.
- **Strict 13 Qualifier:** A strict rule that requires the low (for a buy countdown) or high (for a sell countdown) to be below/above the corresponding bar 8 of the countdown to qualify the final signal.
- **TD Combo Qualification:** An additional rule that adds a new qualification to the buy/sell signals.
- **TDST Lines:** The indicator can plot TDST (TD Support and Resistance) lines, which act as dynamic support and resistance levels.
- **Perfection Markers:** Marks a setup "9" with a "P" to indicate a "perfected" setup, which can increase the reliability of the signal.

## How to Use It

1.  **Open the Pine Editor:** In TradingView, navigate to the Pine Editor at the bottom of your chart.
2.  **Copy and Paste:** Copy the entire code from this document and paste it into the Pine Editor, replacing any existing code.
3.  **Add to Chart:** Click the "Add to Chart" button in the upper right corner of the Pine Editor. The indicator will appear on your chart.
4.  **Adjust Settings:** You can modify the indicator's behavior by clicking the "Settings" gear icon next to its name on the chart. This will open a dialog box with all the input options, allowing you to customize the display and logic to fit your trading style.

## Settings Explained

- **Start Countdown After Same-Direction Setup:** Enables the countdown to begin immediately after a 9-bar setup.
- **Reset Countdown On Opposite Flip:** Resets the countdown if a price flip in the opposite direction occurs.
- **Use Aggressive Countdown:** Uses a less conservative rule for counting bars in the countdown phase.
- **Strict 13 Qualifier:** Requires a specific price relationship on the 13th bar to validate the signal.
- **13 Qualifier Mode:** Allows you to choose between `Close vs bar 8` and `Low/High vs bar 8` for the strict 13 qualification.
- **Show Setup Numbers (1-9):** Displays the numbers for the setup phase.
- **Show Countdown Numbers (1-13):** Displays the numbers for the countdown phase.
- **Show Only Final Signals (B9, S9, 13):** Hides all intermediate numbers, showing only the final buy/sell signals.
- **Show Perfection Markers (P):** Displays the "P" marker for perfected setups.
- **Show TDST Lines:** Plots the TDST support and resistance lines.
- **Show TDST Stop Loss (SL):** Displays a "SL" marker when the TDST line is broken, indicating a potential stop-loss event.
- **Breakout Strength:** A setting to define how far the price needs to break a TDST line to be considered a breakout.
- **Show TD Reaction Line:** Displays a line to show the 13-bar reaction level.
