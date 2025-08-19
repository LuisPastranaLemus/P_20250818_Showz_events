# 🧭 Project Analysis
Brief Decription

Internship project at Showz Analytics Department, focused on optimizing marketing expenses through data-driven insights from web traffic, orders, and marketing spend data.

---

## 🔍 Project Overview (P-20280818_Showz_events)

Project Overview

This project analyzes user behavior, sales patterns, and marketing investments for Showz, a company specializing in event ticket sales. Using server logs, order history, and marketing spend data from January 2017 to December 2018, the goal is to evaluate how customers interact with the platform, when they start purchasing, how much revenue they generate, and how marketing costs impact profitability.

The analysis follows three main steps:

1. Data preparation – loading and cleaning datasets (visits, orders, and costs).   
2. Metric calculations and reporting – exploring user activity, conversions, sales performance, and marketing efficiency.   
3. Conclusions and recommendations – advising the marketing team on where and how to best allocate their budget.   

Key questions:

- Objectives to reach

  - User Behavior:
    - How many people use the service daily, weekly, and monthly?   
    - How many sessions per day and what is their average duration?
    - How often do users return?

  - Sales Performance:
    - When do users start making purchases after registration?
    - How many orders do they place over time?
    - What is the average purchase size?
    - What is the customer lifetime value (LTV)?

  - Marketing Efficiency:
    - How much money was spent overall, by source, and over time?
    - What is the customer acquisition cost (CAC) for each source?
    - How profitable are the investments (ROMI)?

Project Info explanation

- Datasets:
    - data/raw/visits_log_us.csv → User visits with session timestamps, device, and acquisition source.
    - data/raw/orders_log_us.csv → Orders with user ID, timestamp, and revenue.
    - data/raw/costs_us.csv → Marketing spend by source and date.

- Analysis Approach:
    - Conduct cohort analysis to evaluate user conversion times.
    - Track LTV, CAC, and ROMI across devices and acquisition sources.
    - Use visualizations to compare performance over time and across channels.

- Deliverables:
    - A Jupyter Notebook with code (in code cells) and explanations (in markdown cells).
    - Graphs and metrics supporting insights into user behavior, sales performance, and marketing ROI.
    - Final recommendations for the marketing team on budget allocation and high-performing channels.

---

## 🧮 Data Dictionary

This project has 3 different tables.

- `visits_log_us.csv` (server logs with data about website visits)   
    `column:Uid`: Unique user identifier.   
    `column:Device`: User's device.   
    `column:Start TS`: Session start date and time.
    `column:End Ts`: Session end date and time.
    `column:Source Id`: Identifier of the ad source the user is using.   

- `orders_log_us.csv` (data about orders)   
    `column:Uid`: Unique identifier of the user who placed an order.   
    `column:Buy TS`: Date and time of the order. 
    `column:Revenue`: Showz's revenue from the order.   

- `costs_us.csv` (data about marketing expenses)   
    `column:source_id`: Ad source identifier.   
    `column:dt`: Date.   
    `column:costs`: Spending on this ad source on this day.

---

## 📚 Guided Foundations (Historical Context)

The notebook `00-guided-analysis_foundations.ipynb` reflects an early stage of my data analysis learning journey, guided by TripleTen. It includes data cleaning, basic EDA, and early feature exploration, serving as a foundational block before implementing the improved structure and methodology found in the main analysis.

---

## 📂 Project Structure

```bash
├── data/
│   ├── raw/              # Original dataset(s) in CSV format
│   ├── interim/          # Intermediate cleaned versions
│   └── processed/        # Final, ready-to-analyze dataset
│
├── notebooks/
│   ├── 00-guided-analysis_foundations.ipynb     ← Initial guided project (TripleTen)
│   ├── 01_cleaning.ipynb                        ← Custom cleaning 
│   ├── 02_feature_engineering.ipynb             ← Custom feature engineering
│   ├── 03_eda_and_insights.ipynb                ← Exploratory Data Analysis & visual storytelling
│   └── 04-sda_hypotheses.ipynb                  ← Business insights and hypothesis testing
│
├── src/
│   ├── init.py              # Initialization for reusable functions
│   ├── data_cleaning.py     # Data cleaning and preprocessing functions
│   ├── data_loader.py       # Loader for raw datasets
│   ├── eda.py               # Exploratory data analysis functions
│   ├── features.py          # Creation and transformation functions for new variables to support modeling and EDA
│   └── utils.py             # General utility functions for reusable helpers
│
├── outputs/
│   └── figures/          # Generated plots and visuals
│
├── requirements/
│   └── requirements.txt      # Required Python packages
│
├── .gitignore            # Files and folders to be ignored by Git
└── README.md             # This file
```
---

🛠️ Tools & Libraries

- Python 3.11
- os, pathlib, sys, pandas, NumPy, Matplotlib, seaborn, IPython.display, scipy.stats
- Jupyter Notebook
- Git & GitHub for version control

---

## 📌 Notes

This project is part of a personal learning portfolio focused on developing strong skills in data analysis, statistical thinking, and communication of insights. Constructive feedback is welcome.

---

## 👤 Author   
##### Luis Sergio Pastrana Lemus   
##### Engineer pivoting into Data Science | Passionate about insights, structure, and solving real-world problems with data.   
##### [GitHub Profile](https://github.com/LuisPastranaLemus)   
##### 📍 Querétaro, México     
##### 📧 Contact: luis.pastrana.lemus@engineer.com   
---

