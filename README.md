# Momentum-Based Strategy – Long-Short Portfolio (College Project)

This project explores a momentum-based long-short strategy using monthly industry return data.  
It goes long on top-performing industries and shorts the lowest-performing ones based on trailing 12-month returns (excluding the most recent month).

## Key Features

- **Data**: Fama-French 49 industry returns  
- **Ranking**: Based on cumulative 12-month returns  
- **Portfolio**:  
  - Long the top 30% (130% weight)  
  - Short the bottom 10% (30% weight)  
- **Rebalancing**: Monthly  
- **Backtest Period**: 1929–2023  

## Performance Summary

- **CAGR**: 18.43%  
- **Sharpe Ratio**: 0.74  
- **Sortino Ratio**: 1.02  
- **Max Drawdown**: –73.4%  
- **Rolling 5-Year Sharpe**: Peaked at 2.05 (April 1946)  

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
