# AQI_Forecast_Project
Using Machine Learning and Deep Learning (like LSTM) to build a predictive model for the Air Quality Index (AQI). This project aims to provide accurate, real-time air quality forecasts by analyzing time-series data.
Air Quality Index (AQI) Analysis & Forecasting for Indian Cities Forecasting for Indian Cities 💨
An internship project for Wipro DICE ID, focused on turning raw pollution data into actionable insights and a predictive model.

🚀 Project Overview
The main goal here was to analyze historical air quality data from major Indian cities like Delhi, Mumbai, and Bengaluru. The project involved everything from cleaning messy raw data to conducting a full-scale Exploratory Data Analysis (EDA) to uncover pollution patterns. The final step was to build and compare time-series models to forecast future pollution levels and suggest practical solutions based on the findings.



🛠️ Tech Stack & Libraries
Language: Python 3.8+

Data Manipulation: Pandas, NumPy

Data Visualization: Matplotlib, Seaborn

Time-Series Modeling:

statsmodels (for ARIMA)

prophet (by Facebook)

Core Environment: Jupyter Notebook

📊 The Dataset
I used a multi-year AQI dataset compiled from official Central Pollution Control Board (CPCB) sources, which I found on Kaggle.

Time Period: 2015 - 2020


Cities: Delhi, Mumbai, Kolkata, Bengaluru, and more.

Key Pollutants Tracked: PM2.5, PM10, NO2, SO2, AQI, etc.

📂 Project Structure
Here's how the repository is organized:

AQI_Analysis_and_Forecasting/
├── 📂 data/
│   ├── raw/              # The original .csv dataset
│   └── processed/        # Cleaned data ready for analysis
├── 📂 notebooks/         # All the project's Jupyter Notebooks
├── 📂 reports/
│   └── figures/          # Saved plots and visualizations
├── .gitignore          # Tells Git what to ignore
├── README.md           # You're reading it!
└── requirements.txt    # All the Python packages needed to run this
⚙️ Getting Started
To get this project running on your local machine, follow these steps.

1. Clone the Repo

Bash

git clone <your-repo-url>
cd AQI_Analysis_and_Forecasting
2. Create a Virtual Environment It's always a good practice to keep project dependencies isolated.

Bash

# Create the environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
3. Install Dependencies This will install all the libraries listed in requirements.txt.

Bash

pip install -r requirements.txt
4. Run the Notebooks Launch Jupyter and run the notebooks in the notebooks/ folder in this order:

01_Initial_Data_Exploration.ipynb

02_Forecasting_Models.ipynb

💡 Key Findings & Outcome
After all the analysis and modeling, here's what I found:

Delhi is the Hotspot: Delhi consistently had the worst air quality among the cities studied, especially during the winter.

Winter is the Danger Zone: There's a clear seasonal trend. Pollution levels shoot up starting in October and peak from November to January.

Prophet > ARIMA for this Task: While both models worked, Prophet's forecast was more accurate. It did a better job handling the strong yearly seasonality and holiday effects (like Diwali).

The final outcome was a clear, data-driven summary of India's urban pollution problem. The model successfully forecasted pollution trends for the next year, leading to a few key recommendations like implementing stricter emission controls during peak winter months and using the forecast to promote green zones in high-risk areas.
