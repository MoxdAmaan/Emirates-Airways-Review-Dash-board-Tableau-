# Emirates Airways Customer Reviews Analysis (2016–2024)

![Emirates Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Emirates_logo.svg/640px-Emirates_logo.svg.png)

## Project Overview
This project analyzes **Emirates Airways customer reviews** from 2016 to 2024. Using Python for **data preprocessing**, and Tableau for interactive **dashboard visualization**, the project aims to uncover insights about:

- Customer satisfaction trends over time
- Ratings for different service aspects (Overall Ratings, Value for Money, Services, Comfort, etc...)
- Travel class-wise satisfaction (Economy, Business, First)
- Aircraft Ratings
- Route-specific Ratings

The goal is to **uncover strengths, opportunities, and actionable insights** to enhance customer experience.

---

## Dataset
- **Source:** [Kaggle – Emirates Airline Customer Reviews](https://www.kaggle.com/datasets/kalyani007/emirates-airline-customer-reviews-2016-2024)
- **Rows:** ~1,500 reviews
- **Columns:**    
  - `Overall Ratings`, `Staff Service`, `Food Quality`, `Ground Service`, `WiFi`, `Entertainment` (1–5)  
  - `Recommended` (Yes/No)  
  - `Travel Class`, `Route`, `Date Flown`, `Date Published`  
  - Other metadata (Aircraft, Status, Title, Review Text)

---

## Tech Stack
- **Python** – For Pre-processing
- **Tableau** – Interactive dashboard creation through various metrices and filters
- **CSV** – For storing cleaned dataset

---

## Data Preprocessing
- Converted `Date Flown` and `Date Published` to datetime format
- Dropped null values in essential columns (WiFi, Food, Staff, Ground Service, Route, Date Published)  
- Standardized categorical columns (`Recommended`, `Travel Class`, `Status`)   
- Verified numeric columns for proper format (ratings from 1–5)

**Cleaned dataset size:** ~1,800 rows × 15 columns

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
- `python_pre-processing.ipynb` → Python notebook with preprocessing  
- `Tableau Dashboard` → Interactive visualizations
