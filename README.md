# Airbnb Data Analysis Project

## Project Overview
This project focuses on analyzing Airbnb listing data to uncover insights related to pricing trends, neighborhood popularity, customer preferences, availability, and property types. The analysis helps understand factors affecting Airbnb prices and booking patterns.

The project demonstrates data cleaning, exploratory data analysis (EDA), visualization, and business insight generation using Python.

---

## Objectives
- Analyze Airbnb listing prices across different neighborhoods
- Identify factors affecting pricing
- Explore room type distributions
- Understand customer review trends
- Analyze availability and occupancy patterns
- Generate business insights for hosts and travelers

---

## Dataset Information
Dataset includes:
- Listing price
- Neighborhood
- Room type
- Number of reviews
- Availability
- Host details
- Location information

---

## Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Cleaning Steps
- Removed missing values
- Removed duplicate records
- Converted data types
- Handled outliers in pricing
- Standardized column names

---


## Exploratory Data Analysis

### 1. Price Distribution Analysis
- Analyzed distribution of Airbnb prices
- Identified expensive and affordable areas

### 2. Neighborhood Analysis
- Compared average prices across neighborhoods
- Identified most popular locations

### 3. Room Type Analysis
- Entire home/apartment
- Private room
- Shared room

### 4. Review Analysis
- Examined relationship between reviews and pricing
- Identified highly reviewed neighborhoods

### 5. Availability Analysis
- Analyzed yearly availability trends
- Identified highly occupied listings

---
## Visualizations
### Distribution of Prices
<img width="1000" height="600" alt="distribution_of_prices" src="https://github.com/user-attachments/assets/1785cf85-62df-4bd1-88b2-f78aa795ae36" />

### Room Type Analysis
<img width="800" height="500" alt="room_type_distribution" src="https://github.com/user-attachments/assets/e98c391b-82fd-4c68-b2e2-291e1be56652" />

### Neighborhood Analysis
<img width="1200" height="800" alt="listings_by_neighborhood_group" src="https://github.com/user-attachments/assets/a440c5db-7896-4746-87d2-d14d9008d506" />

### Price vs. Room Type
<img width="1000" height="600" alt="price_vs_room_type" src="https://github.com/user-attachments/assets/6c488c5a-374a-4ea6-b6d0-cc3acc2dd401" />

### Reviews Over Time
<img width="1200" height="600" alt="reviews_over_time" src="https://github.com/user-attachments/assets/6126ee0a-c6fb-4c44-a17a-36808f682969" />

### Top Hosts by Number of Listings
<img width="1200" height="600" alt="top_10_hosts" src="https://github.com/user-attachments/assets/dedf3ad9-6652-4158-94c0-4535410bc066" />

### Geographical Distribution of Listings
<img width="1000" height="800" alt="geographical_distribution" src="https://github.com/user-attachments/assets/f4f00866-24d5-4fd8-81ee-1e7d26acfc2a" />


### Visualizations used
- Heatmaps
- Bar charts
- Scatter plots
- Histograms
- Box plots

---

## Consolidated Insights from Airbnb Data Analysis

Based on the visualizations and exploratory data analysis, here's a summary of the key insights:

### 1. Distribution of Prices
*   The distribution of listing prices is heavily right-skewed, indicating that most listings are at lower price points, with a long tail of fewer, very expensive listings. There are likely significant outliers at the higher end.

### 2. Room Type Distribution
*   'Entire home/apt' and 'Private room' are the most common listing types, significantly outnumbering 'Shared room'.

### 3. Number of Listings by Neighborhood Group
*   Manhattan and Brooklyn are the dominant boroughs in terms of Airbnb listing volume, significantly surpassing Queens, The Bronx, and Staten Island. This highlights these two boroughs as primary centers for short-term rentals.

### 4. Price vs. Room Type
*   'Entire home/apt' listings command the highest median prices and show the widest price range. 'Private room' listings are moderately priced, and 'Shared room' listings are the most affordable.

### 5. Number of Reviews Over Time
*   The review activity shows fluctuations, with a notable spike around mid-2019. There are some unusual data points (reviews in the future), suggesting potential data entry errors that need cleaning for accurate time-series analysis.

### 6. Top Hosts by Number of Listings
*   A few hosts (e.g., Michael, David, John) have a significantly higher number of listings, indicating the presence of professional landlords or property management companies rather than just individual owners.

### 7. Geographical Distribution of Listings
*   Listings are primarily concentrated in Manhattan, Brooklyn, and Queens, with Manhattan and Brooklyn showing the highest density. This confirms non-uniform listing availability across different neighborhood groups.

### 8. Correlation Matrix of Numerical Features
*   `price` and `service fee` have a strong positive correlation, which is expected. `number of reviews` and `reviews per month` also show a strong positive correlation.
*   `minimum nights` and `availability 365` have very low correlations with other numerical variables, suggesting they are relatively independent factors.

---

## Business Impacts and Analytics Suggestions

Based on the consolidated insights, here are some business impacts and actionable suggestions:

### 1. Pricing Strategy Optimization
*   **Impact:** The right-skewed price distribution indicates a highly competitive market at lower price points and less competition at higher-end segments. Outliers suggest opportunities for premium offerings.
*   **Suggestion:** Implement dynamic pricing models that consider room type, neighborhood, availability, and seasonality. For premium listings, focus on unique amenities or experiences to justify higher prices. For competitive segments, explore strategies like offering discounts for longer stays or off-peak bookings.

### 2. Market Focus and Expansion
*   **Impact:** Manhattan and Brooklyn dominate the market, while other boroughs like The Bronx and Staten Island have significantly fewer listings. This imbalance can represent untapped potential or saturated markets.
*   **Suggestion:** For hosts and investors, target Manhattan and Brooklyn for high-demand, high-return properties, but be prepared for intense competition. Explore expansion opportunities in less saturated markets like The Bronx or Staten Island, focusing on local attractions and amenities to attract niche markets.

### 3. Host Management and Engagement
*   **Impact:** The presence of professional hosts with multiple listings significantly influences market supply. Identifying top hosts can reveal best practices.
*   **Suggestion:** For platforms like Airbnb, develop tiered support and incentive programs for professional hosts. For individual hosts, learning from top hosts' strategies (e.g., in listing descriptions, photos, amenities) can improve performance. Consider host training programs on optimizing listings and guest experience.

### 4. Listing Improvement and Differentiation
*   **Impact:** 'Entire home/apt' and 'Private room' are the most common and profitable types. The wide price range for 'Entire home/apt' suggests diverse value propositions.
*   **Suggestion:** Hosts should focus on enhancing 'Entire home/apt' and 'Private room' listings with high-quality photos, detailed descriptions, and unique amenities. Invest in features that justify higher prices, such as modern decor, premium facilities, or excellent guest services. For 'Shared room' listings, emphasize affordability, cleanliness, and security.

### 5. Data Quality and Predictive Analytics
*   **Impact:** Inconsistent data (e.g., future review dates) can skew time-series analysis and hinder accurate forecasting.
*   **Suggestion:** Implement robust data validation during collection. Leverage clean review data to predict booking trends, identify peak seasons, and anticipate demand. Develop a model to forecast occupancy rates and optimal pricing based on historical review patterns and seasonality.

### 6. Correlation-based Feature Engineering
*   **Impact:** Strong correlations between `price` and `service fee`, and `number of reviews` and `reviews per month`, can be used in predictive models. Low correlation with `minimum nights` and `availability 365` suggests they might need different analytical approaches.
*   **Suggestion:** When building machine learning models for price prediction or demand forecasting, explicitly include correlated features like 'service fee' or 'reviews per month'. For features with low correlation, consider non-linear relationships or interaction terms, or explore alternative data points that might better explain their impact.

---

## Conclusion
This project provides valuable insights into Airbnb market trends and customer behavior. The analysis demonstrates how data analytics can help optimize pricing strategies and improve customer satisfaction.

---

## Author
Nilay Singh

GitHub: https://github.com/nilaysingh09
