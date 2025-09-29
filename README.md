# Citi Bike Trip Analysis Dashboard – January 2020

This project explores Citi Bike trip data for **January 2020** to uncover how people in New York City use shared bikes. The dataset comes from the [Citi Bike System Data](https://citibikenyc.com/system-data), which provides detailed trip histories, including trip duration, start and end stations, user type, gender, and year of birth.

---

## 📊 Project Overview

The analysis was performed in **Excel** using pivot tables and charts to transform raw trip records into meaningful insights.  
The core objective was to understand **riding patterns** - how often people ride, where they pick up bikes, how long trips last, and how user demographics affect trip behavior.

Key questions explored:

- Which stations are the most popular starting points?  
- How do **customers vs. subscribers** use the service across the week?  
- Do certain **age groups** ride longer or more often?  
- What does the relationship between **user age and average trip duration** look like?  

---

## 🗂️ Dataset Details

- The **original dataset** contained fields up to **`gender` (column O)**:  
  - Ride ID and Bike ID  
  - Trip Duration (seconds)  
  - Start & Stop Time and Date  
  - Start & End Station details with lat/long  
  - User Type (Customer or Subscriber)  
  - Gender (0 = unknown, 1 = male, 2 = female)  
  - Year of Birth  

For this project, we primarily focused on:  
- **`tripduration_in_min`** – ride length in minutes  
- **`age`** – calculated from year of birth  
- **Station IDs and names** – to identify hotspots  

---
## 🔎 Steps in Exploratory Data Analysis (EDA)

Following a structured EDA process ensures that insights are both accurate and actionable. The key steps applied here include:

1. **Data Understanding & Collection**  
   - Identify dataset source (Citi Bike system data).  
   - Understand fields available (trip duration, user demographics, station info).  

2. **Data Cleaning & Preparation**  
   - Convert trip duration from seconds to minutes.  
   - Handle missing or invalid values (e.g., birth year anomalies, trip outliers).  
   - Create calculated columns like `age` and `DayofWeek`.  

3. **Univariate Analysis**  
   - Explore single variables: distribution of ages, trip durations, user type breakdown.  
   - Detect skewness or outliers in trip durations.  

4. **Bivariate/Multivariate Analysis**  
   - Age vs. average trip duration.  
   - User type vs. day of week usage.  
   - Station popularity by counts.  

5. **Visualization & Pattern Recognition**  
   - Use scatter plots, bar charts, and pivot visuals in Excel.  
   - Identify trends (commuting vs. leisure, popular stations, long-tail trips).  

6. **Interpretation & Storytelling**  
   - Translate raw outputs into insights about urban mobility and rider behavior.  
   - Connect findings back to real-world use cases (commuting, tourism, infrastructure planning).  

---

## 📈 Dashboard

The dashboard consolidates insights into one view:

- **Top 20 pick-up stations** – Grove St PATH and Sip Ave dominate usage.  
- **Customer vs. Subscriber usage by weekday** – Subscribers account for most rides, with peaks during weekdays.  
- **Age group–wise rental counts** – The **25–34** segment leads, followed by 35–44.  
- **Average trip duration by age group** – Older groups (65+) take slightly longer trips on average.  
- **User age vs. trip duration scatter plot** – Shows variability in trip lengths with some outliers.  

---

## 📷 Dashboard Snapshot

  <img width="1627" height="912" alt="Citibike analysis" src="https://github.com/user-attachments/assets/ce7a8b84-6e13-480c-9954-89c1bf96e820" />


For a detailed view, you can also check the [Dashboard PDF](https://github.com/pratimaprasad17/EDA_Excel_CitiBikeNY/blob/f1334c337e3287959b3faa200bc4c9c5212e783d/Citibike%20NY%20Jan%202020%20Analysis.pdf).

You can view the complete dataset and analysis performed in this [Excel file](./JC-202001-citibike-tripdata.csv)

---

## 🔍 Key Insights

1. **Station Popularity**  
   High-traffic hubs like Grove St PATH and Sip Ave highlight commuter corridors.  

2. **User Behavior**  
   - Subscribers dominate weekdays → reflects regular commuting patterns.  
   - Customers appear more during weekends → likely tourists or occasional riders.  

3. **Age Dynamics**  
   - Most riders fall between 25–44 years.  
   - Average trip duration increases slightly at the extremes (18–24 and 65+).  

4. **Trip Duration Variability**  
   While most trips cluster under 15 minutes, a few outliers show unusually long rides, which could indicate errors or special use cases.  

---

## 📌 Conclusion

This exploratory analysis highlights how **station demand, rider type, and age** influence Citi Bike usage. While younger adults dominate total rides, older riders tend to spend more time per trip. Subscribers show clear commuting behavior, while casual customers represent flexible, leisure-driven usage.  

This kind of breakdown not only informs **urban mobility planning** but also helps **bike-sharing operators** optimize station placement, service offerings, and marketing strategies.  

---

## 🚲 Next Steps

Potential improvements and extensions:  
- Repeat the analysis across multiple months for seasonal trends.  
- Compare station usage with **geospatial maps** for richer context.  
- Introduce predictive analysis to forecast demand at specific stations.  

---

### Author  
📌 *This analysis was conducted as part of an exploratory data analysis exercise to showcase storytelling with real-world datasets.*
