# 📊 Analysis of Flight Delays and Cancellations in the Pacific Northwest

## 📌 Project Overview

This project analyzes flight and weather data from the Pacific Northwest during the first half of 2022 to understand factors affecting departure delays and cancellations. The analysis focuses on two major airports:

- **SEA** – Seattle-Tacoma International Airport  
- **PDX** – Portland International Airport  

The goal is to provide insights to help airlines and passengers optimize operations and travel planning.

---

## 📂 Datasets

### 1. **flights2022.csv**
Contains detailed flight information including:
- `dep_time` – Departure time (hhmm, `NA` if cancelled)
- `dep_delay` – Departure delay in minutes (negative for early)
- `origin` – Origin airport code (SEA or PDX)
- `airline` – Airline name
- `dest` – Destination airport code

### 2. **flights_weather2022.csv**
Extends flight data with weather conditions such as:
- `visib` – Visibility in miles
- `wind_gust` – Wind gust speed in mph

---


## 📈 Key Analyses Performed

### 1. **Data Loading & Exploration**
- Loaded and inspected both flight and weather datasets
- Checked data structure, missing values, and column types

### 2. **Data Manipulation**
- Created `is_cancelled` flag based on missing `dep_delay` values
- Added `route` column by combining origin and destination airports
- Aggregated data to analyze delays and cancellations by:
  - **Route**
  - **Airline**

### 3. **Visualizations**
- Top 9 routes with the highest number of cancellations
- Top 9 airlines with the highest average departure delays

---

## 📊 Visual Insights

### 1. **Route Cancellations**
- Identified the top 9 routes with the most cancellations
- Visualized using a bar chart for clear comparison

### 2. **Airline Delays**
- Highlighted airlines with the highest average departure delays
- Presented in a bar chart with rotated labels for readability

---

## 🚀 How to Run

1. Clone or download the repository.
2. Ensure the datasets (`flights2022.csv` and `flights_weather2022.csv`) are in a `data/` folder.
3. Open `notebook.ipynb` in Jupyter Notebook or JupyterLab.
4. Run all cells to reproduce the analysis.

---
