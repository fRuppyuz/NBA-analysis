[README.md](https://github.com/user-attachments/files/28339885/README.md)
# Project Overview

This project analyzes NBA player statistics across multiple seasons (2020–2025). <br>
The goal is to explore trends in player performance, shooting behavior (especially the three-point era), <br>
and overall efficiency using data analysis and visualization techniques.

Key topics:

1) Evolution of three-point shooting in the NBA
2) Player efficiency and performance metrics
3) Correlation between gameplay statistics
4) Season-based trends and comparisons

# Project structure

├── source_code.ipynb    # Main code for project <br>
├── README.md            # Documentation <br>
├── requirements.txt     # Requirements <br>
├── nba_scraper.log      # Script logging <br>
├── nba_raw_data.csv     # Raw data after scraping <br>
├── nba_clean_data.csv   # Final data set <br>
└── charts/              # Generated PNG visualizations <br>
### Example Output
<img src="./charts/eda_correlation.png" alt="Correlation table" width="600">

# Data Collection & Reliability
The data collection process utilizes `nba_api` and `requests` with built-in error handling to ensure stable execution. <br> 
All operational logs, including status updates and potential connection issues, are recorded in the `nba_scraper.log` file. <br>
This helps in tracking the scraping progress and troubleshooting any potential interruptions during the data collection process.

# Dataset

The dataset is collected using the nba_api library (League Dash Player Stats endpoint).
It includes player-level statistics such as:

1) Points(PTS)
2) Rebounds (REB)
3) Assists (AST)
4) Minutes played (MIN)
5) Field goal stats (FG%, FG3A, FG3%)
6) Free throws (FTM, FTA, FT%)
7) Advanced metrics (PLUS_MINUS, etc.)

# Project documentation
How to Run the Project
1. Install dependencies:
pip install -r requirements.txt

2. Open Jupyter Notebook:
Open source_code.ipynb in your Jupyter environment

Then run code in this order:

1) Data Cleaning
2) EDA
3) Visualization

## Visualizations
The analysis includes various charts to visualize trends in player performance, such as:
- **Box plots:** Showing statistical distribution of player metrics.
- **Trend lines:** Representing changes across seasons (2020–2025).

All generated charts are saved as **PNG files** in the `charts/` folder (or your output directory) for easy review and reporting. <br>
These visuals are generated using `matplotlib`, `seaborn`, and `plotly`.

# Dependencies

Main libraries used:

- pandas: data manipulation and analysis
- numpy: numerical computations
- matplotlib: static data visualization
- seaborn: statistical visualization
- plotly: interactive visualizations
- nba_api: NBA data collection
- requests: HTTP requests for API access

# Key Insights
- Three-point attempts have increased significantly across seasons 
- Player efficiency varies strongly with minutes played
- NBA shows a clear shift toward perimeter-oriented offense
- Scoring distribution is highly skewed due to star players
# Author Notes

This project was developed as part of a data analysis assignment focusing on real-world sports analytics and modern NBA trends.

# Requirements

Works best with stable library versions listed in requirements.txt
