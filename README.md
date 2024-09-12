# TellCo Telecom Business Analysis

## Overview
This project focuses on analyzing customer data for TellCo, a mobile service provider, to identify opportunities for growth. The challenge includes data exploration, user analysis, clustering, and dashboard development. Key sections include user overview analysis, engagement analysis, experience analysis, and satisfaction analysis.



## Key Tasks 

### 1. User Overview Analysis
- **Goal:** Identify top handsets and manufacturers.
- **Outcome:** Aggregated and analyzed user data to find top 10 handsets, top 3 manufacturers, and top 5 handsets per manufacturer.
- **Results:** Generated insights and recommendations for marketing teams based on handset usage.

### 2. User Engagement Analysis
- **Goal:** Measure and cluster user engagement metrics.
- **Outcome:** 
  - Aggregated engagement metrics (session frequency, session duration, traffic).
  - Applied k-means clustering to group users by engagement levels.
  - Plotted top 3 most-used applications and derived top 10 most engaged users per app.

### 3. User Experience Analysis
- **Goal:** Analyze user experience based on network parameters and device characteristics.
- **Outcome:** 
  - Aggregated TCP retransmissions, RTT, throughput, and handset data.
  - Clustering users based on experience metrics.
  - Analyzed throughput distribution per handset type.

### 4. Dashboard Development
- **Goal:** Build a Streamlit dashboard for visualizing insights.
- **Outcome:** Created an interactive dashboard to display the results of user overview and engagement analysis, with user-friendly navigation and clean visualizations.

## How to Run
1. Clone the repository.
2. Install dependencies using `pip install -r requirements.txt`.
3. Run the notebooks for data analysis.
4. To launch the Streamlit dashboard, run `streamlit run scripts/dashboard.py`.

## Future Work
- Add more advanced user satisfaction analysis.
- Integrate feature store in PostgreSQL.

## Project Structure
```bash
├── .vscode/                  # VSCode settings
├── .github/                  # GitHub Actions workflows
│   └── workflows
│       ├── unittests.yml
├── .gitignore                # Git ignore settings
├── requirements.txt          # Dependencies
├── README.md                 # Project documentation
├── src/                      # Source code
│   ├── __init__.py
├── notebooks/                # Jupyter notebooks for analysis
│   ├── user_overview_analysis.ipynb
│   ├── user_engagement_analysis.ipynb
│   ├── user_experience_analysis.ipynb
│   └── README.md
├── tests/                    # Unit tests
│   ├── __init__.py
└── scripts/                  # Scripts for data loading and preprocessing
    ├── load_data.py
    ├── utils.py
    ├── dashboard.py
    └── __init__.py
