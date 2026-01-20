# Momentum-Based Strategy – Long-Short Portfolio (College Project)

This project explores a momentum-based strategy using monthly industry return data. It selects top-performing industries based on trailing 12-month returns and compares equal vs inverse-volatility weights

## Key Features

- **Data**: Fama-French 49 industry returns  
- **Ranking**: Based on cumulative 12-month returns  
- **Portfolio**:  
  - Top 5 industries by momentum 
  - Equal-weighted (20% each) vs Inverse-volatility weighted 
- **Rebalancing**: Monthly  
- **Backtest Period**: 1929–2023  

## Performance Summary

- **CAGR**: 18.43%
- **Worst-Case CAGR (25th percentile)**: 12.96%  
- **Sharpe Ratio**: 0.68 
- **Worst-Case Sharpe (25th percentile)**: 0.49 
- **Leveraged Version (130% long) CAGR**: ~20% 

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
