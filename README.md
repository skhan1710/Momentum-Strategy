Momentum-Based Strategy – Long-Short Portfolio (College Project)

This project implements a momentum-based long-short strategy using monthly industry return data. 
The strategy goes long on top-performing industries and shorts the worst-performing ones, based on trailing 12-month returns.

Key Features

- Data: Fama-French 49 industry returns
- Ranking: Based on cumulative past 12-month return (excluding latest)
- Portfolio:
  - Long top 30% (130% total weight)
  - Short bottom 10% (30% total weight)
- Rebalancing: Monthly
- Backtest Period: 1929–2023

Performance Highlights

- CAGR: 18.43%
- Sharpe Ratio: 0.74
- Sortino Ratio: 1.02
- Max Drawdown: -73.4%
- Rolling 5-Year Sharpe: Peaked at 2.05 (April 1946)

Files Included

- `project_3.ipynb`: Full code + analysis
- `project_3.docx`: Report draft with explanation
- `/data/`: Contains CSV input files

Tools Used

- Python
- pandas, numpy
- matplotlib, seaborn

How to Run

Open the notebook using Jupyter or VS Code. Make sure your CSV files are inside the `data/` folder.

---

**Author**: Safwan Khan (MS in Quant Finance @ Northeastern University)
