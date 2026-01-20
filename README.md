# Momentum-Based Strategy – Industry Portfolio (College Project)

This project explores a momentum-based strategy using monthly industry return data. It selects top-performing industries based on trailing 12-month returns and compares equal-weighting vs inverse-volatility weighting schemes.

## Key Features

- **Data**: Fama-French 49 industry returns  
- **Ranking**: Based on cumulative 12-month momentum returns  
- **Portfolio**:  
  - Top 5 industries by momentum  
  - Equal-weighted (20% each) vs Inverse-volatility weighted  
- **Rebalancing**: Monthly  
- **Backtest Period**: 1931–2023  

## Performance Summary

- **CAGR**: 17.40%  
- **Worst-Case CAGR (25th percentile)**: 13.44%  
- **Sharpe Ratio**: 0.84  
- **Worst-Case Sharpe (25th percentile)**: 0.71  
- **vs Benchmarks**: 50% higher returns than equal-weighting all industries (11.53%), 10x market portfolio (1.55%)  

## Files Included

- `project_3.ipynb`: Notebook with code and analysis  
- `project_3.docx`: Draft report with initial explanation  
- `data/`: Contains CSV input files  

## Tools Used

- Python  
- pandas, numpy  
- matplotlib, seaborn  

## How to Run

Open the notebook using **Jupyter Notebook** or **VS Code**.  
Ensure that the CSV files are located in the `data/` folder.  

Note: *This was my first attempt at implementing a momentum strategy using real data. It contains early mistakes and has been kept public for transparency and learning purposes.*

---

**Author**: Safwan Khan  
*(MS in Quantitative Finance, Northeastern University)*
