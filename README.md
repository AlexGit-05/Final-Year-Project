# 🌍 Air Pollution Analysis in Nairobi, Kenya  

---

## 📜 Overview  

This repository contains the final-year project files for analyzing and modeling air pollution in **Nairobi, Kenya**, focusing on particulate matter (**PM2.5**, **PM10**) and their relationship with temperature and humidity. The analysis employs **ETL processes**, **Exploratory Data Analysis (EDA)**, and predictive modeling using the **Vector Autoregressive (VAR)** model.  

---

## 🌐 Project Description  

Air pollution poses a serious challenge in urban areas worldwide, including Nairobi, Kenya. **PM2.5** (fine particulate matter) and **PM10** (coarse particulate matter) are major pollutants exceeding WHO's recommended limits in Nairobi. This project investigates the **dynamic relationship** between air pollution and meteorological factors (temperature and humidity) using time-series data collected from **58 locations** across Nairobi from **January 2018 to February 2023**.  

### ✨ Research Objectives  
1. Understand how **temperature** and **humidity** affect **PM2.5** and **PM10** levels.  
2. Explore the relationship between **PM2.5**, **PM10**, **temperature**, and **humidity**.  
3. Identify pollution trends over time and investigate **seasonal patterns**.  
4. Develop a predictive model to forecast **air pollution events**.  

### 🔍 Methodology  
- **ETL Process**: Hourly measurements aggregated and cleaned for analysis.  
- **Exploratory Data Analysis (EDA)**: Patterns and trends of air pollutants over time.  
- **Modeling**: Time-series analysis using the **VAR model** to study dynamic relationships and predict pollution levels.  

---

## ⚙️ **Key Features**

- **ETL Process**:
  - Imports large-scale, monthly CSV files of air quality data.
  - Filters required variables (PM2.5, PM10, temperature, humidity).
  - Cleans and aggregates hourly measurements.
  - Combines all data into a unified dataset for analysis.  

- **EDA**:
  - Visualizes pollution trends and seasonal patterns.  
  - Examines the relationship between air quality and meteorological factors.  

- **Predictive Modeling**:
  - Builds a **Vector Autoregressive (VAR)** model to analyze and forecast pollution levels.
  - Evaluates the impact of meteorological variables on air pollutants.  

---

## 🧑‍💻 **Usage**

### 1️⃣ Data Preprocessing  
Use the `Data Preprocessing.Rmd` file to:
- Load and process raw CSV files.
- Perform cleaning, filtering, and aggregation of the data.
- Explore initial trends and relationships in the data through **EDA**.

### 2️⃣ Predictive Modeling  
Use the `Modeling.Rmd` file to:
- Load the cleaned and compiled dataset.
- Train and validate the **VAR model**.
- Analyze and interpret model predictions.

---

## 🔍 **Technologies & Tools**

- **Languages**: R  
- **Libraries**:
  - `tidyverse`: Data manipulation and visualization.  
  - `lubridate`: Handling and formatting date/time data.  
  - `vars`: Vector Autoregressive (VAR) modeling.  
  - `ggplot2`: Data visualization.  

---

## 📊 Data Overview  

The dataset consists of hourly measurements for:  
- **PM2.5**: Fine particulate matter.  
- **PM10**: Coarse particulate matter.  
- **Temperature**: Recorded in degrees Celsius.  
- **Humidity**: Measured as a percentage.  

### Data Source:  
Collected from **58 locations** in Nairobi County, Kenya, between **January 2018 and February 2023**.  

---

## 📈 Expected Outcomes  

- Insights into **temporal patterns** and **seasonal trends** of air pollution in Nairobi.  
- Quantified relationships between **meteorological factors** and **pollutant levels**.  
- A validated **predictive model** for forecasting air pollution events.  
- Policy recommendations to mitigate air pollution in urban environments.  

---

## 🚀 Getting Started  

### Prerequisites  
Ensure R and the required libraries (`tidyverse`, `vars`, `lubridate`, `ggplot2`) are installed.  

### Running the Project  

1. **Data Preprocessing**:  
   Open and run `Data Preprocessing.Rmd` to clean and preprocess the data.

   **EDA:**
   During data preparation and pre analysis we performed clustering using K Means of which the 58 regions were grouped into 6 clusters.  Two distinct clusters were selected based on the average temperature, humidity and particulate matter. Cluster 1 represented the areas with low temperature and high humidity (blue) Cluster 2 represented points with high temperature and low humidity (red).
   
![geomap](https://github.com/AlexGit-05/Final-Year-Project/blob/main/geomap.png)

3. **Modeling**:  
   Open and run `Modeling.Rmd` to train the VAR model and analyze results.  

---

## 🛠️ Future Work  

- Extend the analysis to include additional pollutants (e.g., NO2, SO2).  
- Explore the impact of urban policies on air quality trends.  
- Develop an interactive dashboard for real-time pollution monitoring.  
