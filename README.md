# 🚲 Cyclistic Bike-Share Analysis 
**Uncovering Cyclistic trip data to drive membership growth.**  

## 📌 Project Overview  
This project is the **Google Data Analytics Capstone Case Study**, where I analyzed how annual members and casual riders use Cyclistic bikes differently. The objective is to provide insights that can help the marketing team design data-driven strategies to convert casual riders into annual members — a key factor for Cyclistic’s long-term growth and profitability.  

---

## 🎯 Objectives
- Understand behavioral differences between annual members and casual riders  
- Identify usage patterns by ride length, day of week, monthly and trip purpose  
- Develop data-driven recommendations for converting casual riders into members  

---

## 🛠️ Tools & Skills  
- **Tools:** Excel (Power Query, PivotTables, Charts, Dashboard)  
- **Skills:** Data wrangling, exploratory data analysis (EDA), visualization, business storytelling, KPI design  

---

## 📊 Data  
- **Source:** [Cyclistic’s historical trip data (12 months)](https://divvy-tripdata.s3.amazonaws.com/index.html) provided by Motivate International Inc.  
- **Size:** 12 monthly CSVs combined (~5.8M rows × 13 columns)
- **Key Variables:**  
  - `ride_id` – unique trip identifier  
  - `started_at` / `ended_at` – trip start and end timestamps  
  - `rideable_type` – bike type (classic, docked, electric)  
  - `member_casual` – user type (annual member or casual rider)

## 🔍 Process   

### 1. Preparation & Cleaning Steps
- Downloaded last 12 months of trip data   
- Combined 12 CSVs using Power Query  
- Removed unnecessary columns (`start_station_id`, `end_station_id`, `start_lat`, `start_lng`, `end_lat`, `end_lng`)  
- Added derived columns:  
  - `Month` (Jan–Dec)  
  - `Day Name` (Mon–Sun)  
  - `Hour` (0–23)  
  - `ride_duration` (duration of ride = `end_at – start_at`)  
  - `Season` (Spring, Summer, Fall, Winter)  
- Filtered out bad data (negative/NULL ride lengths)  
- Removed duplicate rows  

### 2. Exploratory Analysis
- Total number of users 
- Number of rides per month
- Number of rides by day of week
- Number of rides by hour
- Average ride duration by user type  
- Distribution of ride types between members and casuals  

---

## 📈 Key Metrics & Findings  
- **Total Users:** 5.77M  
  - Members: 3.66M (64%)  
  - Casual Riders: 2.10M (36%)  
- **Average Ride Duration:**  
  - Overall: 18 minutes  
  - Members: 13 minutes   
  - Casual Riders: 26 minutes  
- **Peak Usage Patterns:**  
  - Season: Summer  
  - Month: September  
  - Day: Saturday  
  - Hour: 5–6 PM  
- **User Behavior Differences:**  
  1. Members ride consistently on weekdays, with peaks around 8 AM and 5 PM → commuter behavior  
  2. Casual riders peak on weekends and ride longer trips → leisure/tourist behavior  
  3. Members favor weekday usage; casual riders favor weekend usage  
- **Bike Type:**  
  - Electric Bike: Members 1.85M, Casual 1.05M  
  - Classic Bike: Members 1.75M, Casual 0.97M  
  - Electric Scooter: Members 0.06M, Casual 0.08M  
  - 👉 Both groups prefer bikes (electric/classic). Scooters are rarely used.  

---

## 📊 Visualizations (Excel Dashboard)  
- **Donut Chart** → Member vs. Casual distribution  
- **Bar Charts** → Total ride per month, Total ride per day, total ride by ride types
- **Line Chart** → Ride frequency per hour, average ride duration  
- **KPI Cards** → Average ride duration, peak season, month, day, and hour  

> 🖼️ Dashboard Overview <img width="7084" height="4500" alt="dashboard_overview" src="https://github.com/user-attachments/assets/deb77019-d369-470a-a1ca-078f638557e4" />


---

## 📌 Recommendations  

1. **Membership Growth Potential**  
   - Casual riders make up 36% of total users and take longer trips. Converting even a portion into annual members would significantly increase revenue.  

2. **Seasonal & Tourist Campaigns**  
   - Ridership peaks in Summer, especially in September. Launch targeted marketing during these months and offer weekly passes for tourists.  

3. **Weekend-Focused Memberships**  
   - Casual riders are most active on weekends. Introduce discounted weekend memberships or leisure bundles to drive conversion.  

4. **Electric Bike Incentives**  
   - Both groups use electric bikes heavily. Create electric bike–inclusive membership options or loyalty perks to encourage conversion.  

---

## 📫 Contact
Created by Nik Muhammad Akmal. Connect with me on [LinkedIn](https://www.linkedin.com/in/nmakmal/)
