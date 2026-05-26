# Momentum-Based Strategy — Industry Portfolio

This project tests a cross-sectional momentum strategy across 49 Fama-French industry portfolios using 93 years of monthly return data (1931 to 2023). It ranks industries by trailing 12-month cumulative returns, constructs concentrated long portfolios of the top 5 industries, and compares equal-weighting against inverse-volatility weighting on both average and worst-case performance metrics.

## Strategy Design

- **Data:** Fama-French 49 industry monthly returns
- **Signal:** Trailing 12-month cumulative return, excluding the most recent month (standard momentum skip)
- **Selection:** Top 5 industries by momentum rank each month
- **Weighting schemes:** Equal-weight (20% each) and inverse-volatility weighted
- **Rebalancing:** Monthly
- **Backtest period:** 1931 to 2023
- **Bias controls:** Formation period uses lagged returns and volatility estimates throughout to eliminate look-ahead bias

## Strategy Selection

Equal-weighting was selected as the primary strategy based on worst-case performance at the 25th percentile of rolling five-year windows. Equal-weight delivered a worst-case CAGR of 13.44% versus 13.00% for inverse-volatility weighting, demonstrating that the additional complexity of volatility-based weighting did not improve tail-risk outcomes over this sample.

## Performance Summary

| Metric | Equal-Weight | Inverse-Volatility | EW All Industries | Market Portfolio |
|---|---|---|---|---|
| CAGR | 17.40% | 16.84% | 11.53% | 1.55% |
| Worst-Case CAGR (25th pct) | 13.44% | 13.00% | 8.45% | 0.82% |
| Sharpe Ratio | 0.84 | 0.85 | 0.63 | 0.39 |
| Worst-Case Sharpe (25th pct) | 0.71 | 0.70 | 0.53 | 0.20 |

The equal-weight momentum strategy delivers approximately 50% higher returns than equal-weighting all 49 industries and over 10x the market portfolio return across the full sample. Even in the worst 25% of five-year rolling periods, the strategy maintained double-digit annualized returns while both benchmarks fell below 9%.

## Key Findings

- Cross-sectional momentum generates persistent alpha across 93 years of data with consistent risk-adjusted performance
- Equal-weighting outperforms inverse-volatility weighting on worst-case tail outcomes despite marginally lower unconditional Sharpe ratio (0.84 vs 0.85)
- Strategy selection based on worst-case CAGR rather than average performance produces more robust results across varying market regimes
- Both weighting schemes significantly outperform passive benchmarks in both central tendency and tail-risk metrics

## Files

- `project_3.ipynb` — full pipeline: data loading, signal construction, portfolio formation, performance evaluation
- `project_3.docx` — draft report with methodology explanation
- `data/` — CSV input files (Fama-French industry returns and factor data)

## Tools

Python, pandas, numpy, matplotlib, seaborn

## How to Run

Open `project_3.ipynb` in Jupyter Notebook or VS Code. Ensure CSV files are in the `data/` folder. Run cells top to bottom — all outputs are self-contained.

---

*Author: Safwan Khan — MS in Quantitative Finance, Northeastern University*
