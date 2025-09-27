# Emirates Airways Customer Reviews Analysis (2016–2024)

![Emirates Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Emirates_logo.svg/640px-Emirates_logo.svg.png)

## Project Overview
This project analyzes **Emirates Airways customer reviews** from 2016 to 2024. Using Python for **data preprocessing and exploratory data analysis (EDA)**, and Tableau for interactive **dashboard visualization**, the project aims to uncover insights about:

- Customer satisfaction trends over time
- Ratings for different service aspects (staff, food, ground service, WiFi, entertainment)
- Travel class-wise satisfaction (Economy, Business, First)
- Recommendation likelihood
- Route-specific feedback

The goal is to **help Emirates identify strengths, opportunities, and actionable insights** to enhance customer experience.

---

## Dataset
- **Source:** [Kaggle – Emirates Airline Customer Reviews](https://www.kaggle.com/datasets/kalyani007/emirates-airline-customer-reviews-2016-2024)
- **Rows:** ~2,000 reviews
- **Columns:**  
  - `Overall Rating` (1–10)  
  - `Staff Service`, `Food Quality`, `Ground Service`, `WiFi`, `Entertainment` (1–5)  
  - `Recommended` (Yes/No)  
  - `Travel Class`, `Route`, `Date Flown`, `Date Published`  
  - Other metadata (Aircraft, Status, Title, Review Text)

---

## Tech Stack
- **Python** – Pandas, NumPy, Matplotlib, Seaborn for preprocessing & EDA
- **Tableau** – Interactive dashboard creation
- **CSV** – Cleaned dataset storage

---

## Data Preprocessing
- Converted `Date Flown` and `Date Published` to datetime  
- Dropped null values in essential columns (WiFi, Food, Staff, Ground Service, Route, Date Published)  
- Standardized categorical columns (`Recommended`, `Travel Class`, `Status`)  
- Encoded binary `Recommended` column (Yes → 1, No → 0)  
- Verified numeric columns for proper format (ratings from 1–5; Overall Rating from 1–10)

**Cleaned dataset size:** ~1,800 rows × 15 columns

---

## Exploratory Data Analysis (EDA)

### 1. Overall Ratings
- Average rating: **7.8/10**  
- Business and First Class: **~9/10**  
- Economy: **~7/10**

### 2. Recommendation
- **85% of customers recommend Emirates**  
- Positive correlation between **high ratings and recommendation**

### 3. Service Ratings
| Service Aspect | Average Rating (1–5) |
|----------------|---------------------|
| Staff Service  | 4.7                 |
| Food Quality   | 4.2                 |
| Ground Service | 4.5                 |
| WiFi           | 3.8                 |
| Entertainment  | 4.0                 |

- Staff service and ground service are the biggest drivers of customer satisfaction  
- WiFi and Economy food are areas for improvement

### 4. Time Trends
- Review volume peaked in 2019 (~350 reviews)  
- Dip in 2020 (~120 reviews) due to COVID-19  
- Gradual recovery to 2024 (~300 reviews)  
- Average rating remained stable around **7.8–8.0**

### 5. Route & Class Analysis
- Business and First Class consistently report higher satisfaction across all routes  
- Economy ratings lower on **long-haul flights**  
- Identified routes with **lower ratings**, suggesting potential operational improvements

---

## Tableau Dashboard
The dashboard is interactive and includes:  
- Trend analysis of reviews over time  
- Breakdown of ratings by class and service aspect  
- Recommendation analysis  
- Route-based insights  

🔗 [View Dashboard Online](https://public.tableau.com/app/profile/mohammad.aman3207/viz/EmiratesAirwaysReviewDashboard/Dashboard1)

---

## Key Business Insights
1. Emirates has **strong customer satisfaction and loyalty**.  
2. Staff service and ground service are major strengths.  
3. Economy class amenities (food, seating) and WiFi are improvement opportunities.  
4. Certain routes have lower satisfaction – focus on operational efficiency.  
5. Review trends indicate the company is resilient, even after global disruptions like COVID-19.

---

## Conclusion
This project demonstrates how **data-driven insights** can guide **strategic improvements** in customer experience. By addressing targeted areas, Emirates Airways can maintain its **premium reputation** while enhancing the Economy travel experience and overall operational efficiency.

---

## Project Files
- `emirates_reviews_cleaned.csv` → Cleaned dataset ready for analysis  
- `EDA.ipynb` → Python notebook with preprocessing & analysis  
- `Tableau Dashboard` → Interactive visualizations

---

## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/<your-username>/emirates-airways-reviews.git
