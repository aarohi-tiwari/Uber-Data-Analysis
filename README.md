# 🚖 Uber Data Analysis Project

This project performs an end-to-end exploratory data analysis (EDA) on Uber ride data to understand user travel behavior over time — including frequency, duration, category, distance, and purposes of trips. Visualizations were created using Python and common data science libraries.

---

## 📁 Dataset

The dataset contains **1,156** records of Uber rides in 2016, including:
- `START_DATE`, `END_DATE`: Timestamps of the ride
- `CATEGORY`: Type of ride (mostly Business)
- `START`, `STOP`: Pickup and drop locations
- `MILES`: Distance traveled
- `PURPOSE`: Reason for travel

---

## 📊 Features & Analysis Performed

- **Data Cleaning**
  - Converted date strings to datetime objects
  - Handled missing values using `fillna`
  - Removed invalid or null rows using `dropna`

- **Feature Engineering**
  - Extracted `month`, `hour`, `day`, and `day-night` period from timestamps
  - Categorical mapping for better labeling in graphs

- **Visualizations**
  - Count plots of ride `CATEGORY`, `PURPOSE`, and time-of-day (`day-night`)
  - Monthly ride volume trends with `lineplot`
  - Weekly trends using bar plots
  - Box plots and distribution plots of distance (`MILES`) with outlier filtering

---

## 📈 Key Insights

- Most rides are categorized as **Business**.
- The most common purpose for travel is **Meeting** and **Errands**.
- Ride frequency is highest during the **day** and **evening hours**.
- **Saturday** and **Friday** have the most rides.
- Majority of rides fall below **40 miles**, with a few long-distance outliers.
- Peak monthly activity in **January**, **July**, and **December**.

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🧪 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/uber-data-analysis.git
   cd uber-data-analysis
