# PineScript: NeuralMA Strategy Framework

This repository contains an advanced trading strategy framework developed in Pine Script for the TradingView platform. It integrates a sophisticated neural network signal grading engine with a comprehensive suite of custom-built filtering tools to enhance signal quality and user control.

## Overview

The core of this framework uses a neural network to analyze multiple market contexts (momentum, volatility, trend structure) and assign a quality grade (from A+ to F) to potential trade signals. I have built an extensive set of features around this engine to create a complete and practical trading tool.

## Core Features & My Contributions

While the base neural network logic was adapted from the publicly available "Trend Architect Lite" script, the majority of the functional code in this framework is my original work.

*   **Advanced Moving Average (MA) Filtering System:**
    *   **Directional Filtering:** Isolate signals that are either Trend-Following or Counter-Trend.
    *   **Z-Score Distance Filter:** A volatility-based filter to avoid chasing over-extended price action.
    *   **MA Contact Filter:** Option to ignore signals that occur when price is consolidating at the moving average.
    *   **Multi-Timeframe Confirmation:** Includes a secondary MA that can be plotted from a higher timeframe to ensure alignment with the broader market trend.

*   **Full Trading Session Integration:**
    *   **Session-Based Filtering:** Enable or disable signals based on the active trading session (Sydney, Tokyo, London, New York).
    *   **Automated DST Logic:** Session times automatically adjust for Daylight Saving Time.
    *   **Visual Session Boxes:** Clearly highlights market hours directly on the chart.

*   **Enhanced Usability & Customization:**
    *   **Streamlined Alerts:** A clean and practical alert system for easy integration with trading automation platforms.
    *   **Advanced Visuals:** Full control over signal colors and chart aesthetics with pre-built color themes.

## Acknowledgements

The foundational neural network signal analysis and grading functions in this script are adapted from the **"Trend Architect Lite"** indicator. My work focuses on building a robust strategic framework *around* this excellent core engine.

## How to Use

1.  Copy the code from the `NeuralMA_Framework.pine` file.
2.  Open the Pine Editor in [TradingView](https://www.tradingview.com/).
3.  Paste the code into the editor.
4.  Click "Add to chart".
5.  Adjust the settings in the indicator menu to fit your trading style and market.
