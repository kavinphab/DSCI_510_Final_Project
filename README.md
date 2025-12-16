Bear Necessities: Finding the Chicago Bears’ Next Draft Gem
Course: DSCI 510
Team Members:
Kavin Phabiani — kphabian@usc.edu — USC ID: 6414233457
Peter Park — pspark@usc.edu — USC ID: 4240400712

This project uses a data-driven analytical approach to determine the Chicago Bears’ most urgent positional need for the 2026 NFL Draft and to identify the top NCAA prospects who best fit that need. The analysis compares Bears’ team-level performance against league averages using z-score standardization and evaluates college football players using composite performance metrics.

project-root/
│
├── src/
│   ├── get_data.py           # Collects raw NFL and NCAA data via APIs
│   ├── clean_data.py         # Cleans and processes raw JSON into CSVs
│   ├── run_analysis.py       # Performs analysis and ranks draft prospects
│   └── visualize_results.py # Generates plots and visualizations
│
├── data/
│   ├── raw/                  # Raw JSON data from APIs
│   └── processed/            # Cleaned CSV files
│
├── results/
│   ├── bears_vs_league_zscores.csv
│   ├── position_group_needs.csv
│   ├── top_cfb_prospects_for_bears_need.csv
│   ├── position_needs_barplot.png
│   └── top_prospects_barplot.png
│
└── README.md

python3 -m venv venv
source venv/bin/activate
pip install requests pandas numpy matplotlib
python src/get_data.py
python src/clean_data.py
python src/run_analysis.py
python src/visualize_results.py
