# Debt-to-GDP Impact Analysis

## Overview

This is a personal research project exploring the relationship between government debt-to-GDP ratios and economic outcomes across 23 first-world countries over 30 years (1995-2024).

## Purpose

To empirically examine whether government debt levels significantly impact:
- GDP growth
- Worker welfare (real wage proxy)
- Unemployment rates
- Inflation

## Key Finding

**Debt-to-GDP ratios explain less than 5% of economic outcome variance.**

This finding is based on correlation analysis of the available data. The remaining variance (>95%) is explained by other factors not measured in this study.

## What's Included

This directory contains a single Jupyter notebook with the complete analysis:

- **debt_analysis_notebook.ipynb** - Interactive analysis with all code, visualizations, and findings

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```bash
jupyter notebook debt_analysis_notebook.ipynb
```

The notebook will:
1. Fetch data from World Bank API (requires internet connection)
2. Calculate correlations and statistics
3. Generate all visualizations inline
4. Present findings with honest interpretation

## Data Source

All data is sourced from the World Bank Open Data API:
- Government Debt-to-GDP Ratio (GC.DOD.TOTL.GD.ZS)
- GDP Growth (NY.GDP.MKTP.KD.ZG)
- GDP Per Capita Growth (NY.GDP.PCAP.KD.ZG)
- Inflation (FP.CPI.TOTL.ZG)
- Unemployment Rate (SL.UEM.TOTL.ZS)

## Countries Analyzed

USA, United Kingdom, Germany, France, Japan, Canada, Italy, Australia, Spain, Netherlands, Switzerland, Sweden, Belgium, Austria, Norway, Denmark, Finland, Ireland, New Zealand, Singapore, South Korea, Iceland, Luxembourg

## Methodology

1. Data collection from World Bank API
2. Calculation of real wage proxy (GDP per capita growth - inflation)
3. Correlation analysis (Pearson)
4. Range-based performance comparison
5. Statistical significance testing

## Key Findings (What We Can Prove)

1. **Weak Correlations**
   - GDP Growth: r = -0.10 (explains 1.1% of variance)
   - Worker Welfare: r = -0.21 (explains 4.6% of variance)
   - Unemployment: r = +0.11 (explains 1.2% of variance)

2. **Limited Explanatory Power**
   - Debt-to-GDP explains less than 5% of economic outcome variance
   - Over 95% of variance is explained by other factors

3. **Range Analysis**
   - Moderate debt (30-90%) performs slightly better than extremes
   - But differences are small relative to variability within ranges

## What We Cannot Prove

This analysis does not quantify the specific contribution of other factors such as:
- Policy quality
- Productivity growth
- Demographics
- Global economic conditions

These would require additional data and multivariate analysis beyond the scope of this study.

## Limitations

- Correlation does not imply causation
- Country-specific factors not fully captured
- Historical data may not predict future outcomes
- Real wage proxy is an approximation
- Analysis focuses on linear relationships

## Disclaimer

This analysis is for educational and research purposes only.

## License

This is a personal research project. Data is sourced from publicly available World Bank datasets.
