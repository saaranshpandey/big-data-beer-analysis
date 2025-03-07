# Big Data Analysis: Beer

**CIS 545: Big Data Analytics (Spring 2024)**  
Assignment – Beer Data Analysis

---

## 1. Overview
This project examines a large-scale beer dataset to explore consumption trends, brewery characteristics, and user ratings. The analysis uses big data techniques in a PySpark/AWS environment to handle and process millions of records efficiently.

---

## 2. Dataset
- **Data Source:** Beer-related data (e.g., brewery info, beer descriptions, user reviews/ratings)
- **Features:**  
  - Brewery name and location  
  - Beer style and alcohol by volume (ABV)  
  - Ratings (numeric scores, textual reviews)  
  - Timestamps of reviews or check-ins  

---

## 3. Analytical Approach
1. **Data Ingestion:**  
   - Loaded data files into Spark for distributed processing.
   - Ensured proper schema inference and data type assignments.

2. **Data Cleaning & Transformation:**  
   - Filtered null or invalid entries (e.g., missing beer name, out-of-range ABV).
   - Consolidated textual reviews and standardized rating columns.
   - Removed duplicates and handled outlier values.

3. **Exploratory Data Analysis (EDA):**  
   - Computed basic statistics (mean rating, distribution of ABV, etc.).
   - Identified popular beer styles, top breweries, and seasonal trends.
   - Examined correlations between ABV, style, and ratings.

4. **Scalability & Performance:**  
   - Employed PySpark for distributed operations on large datasets.
   - Utilized AWS cluster resources for efficient data processing and memory management.

---

## 4. Key Findings
- **Popular Beer Styles:** IPAs generally received the highest average ratings, followed closely by stouts.
- **High ABV vs. Rating:** A slight positive correlation exists, indicating beers with higher ABV often receive better ratings.
- **Brewery Trends:** Certain regional breweries consistently rank among top-rated. Seasonal variations were observed in user ratings and style preferences.
- **Data Scale:** Spark’s distributed capabilities handled multi-million record datasets without crashing, illustrating the power of big data frameworks for analytics.

---

## 5. Conclusion & Future Work
- **Data-Driven Brewery Insights:** Breweries can leverage these analyses to tailor beer offerings according to consumer preferences and trends.
- **Further Exploration:** Incorporate user demographics, social media sentiment, and weather data to enrich beer consumption insights.
- **Real-Time Analysis:** Implement streaming approaches (e.g., Spark Streaming) for real-time recommendation or alert systems (e.g., trending beer styles, new releases).

---
