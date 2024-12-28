# **EDA Project 1 - Analyzing Airbnb Market Trends**

## **Introduction**

This project aims to analyze the short-term rental market in New York using Airbnb listing data. As a consultant working for a real estate start-up, you have been tasked with providing insights into the market trends using exploratory data analysis (EDA). The data includes details such as listing prices, room types, neighborhood information, review dates, and host details. The goal is to transform and visualize this data to uncover patterns and trends in the market.

## **Files Available**

The data used in this project comes from three primary sources:

1. **`airbnb_price.csv`**: Contains information about Airbnb listing prices and locations.
   - Columns: `listing_id`, `price`, `nbhood_full`
   
2. **`airbnb_room_type.xlsx`**: Includes details about room types and descriptions.
   - Columns: `listing_id`, `description`, `room_type`
   
3. **`airbnb_last_review.tsv`**: Contains information about the last review dates and host names.
   - Columns: `listing_id`, `host_name`, `last_review`

## **Assignment Guidelines**

This assignment is open-ended, allowing you to refer to resources for assistance. For each solution, provide a brief explanation of how you arrived at the solution, including the steps taken. The submission should include all steps of the process, and each question should contain the complete code workflow.

### **Questions**

#### Basic Analysis
1. **Dates of Reviews**  
   - Find the earliest and most recent review dates and store them as `earliest_review` and `most_recent_review`.

2. **Private Room Listings**  
   - Count how many listings are private rooms and store the result in `nb_private_rooms`.

3. **Average Price Calculation**  
   - Calculate the average listing price and store it in `avg_price`.

4. **Summary Table**  
   - Create a DataFrame `review_dates` containing the calculated values: `first_reviewed`, `last_reviewed`, `nb_private_rooms`, `avg_price`.

#### Intermediate Analysis
5. **Neighborhood Trends**  
   - Find the neighborhoods with the highest and lowest average prices. Create a DataFrame with `neighborhood`, `average_price`, and `number_of_listings`.

6. **Word Analysis in Descriptions**  
   - Identify the top 10 most frequently used words in the `description` column (excluding stopwords).

#### Advanced Analysis
7. **Room Type Comparison**  
   - Compare the average prices for each `room_type` (shared room, private room, entire home/apartment). Create a bar chart to visualize the comparison.

8. **Trend Over Time**  
   - Analyze the number of reviews over time and plot a line graph of reviews per month.

9. **Scatter Plot with Regression Line**  
   - Create a scatter plot showing the relationship between `price` and `description` length, with a regression line and outliers annotated.

10. **Seaborn Strip Plot**  
    - Generate a strip plot showing prices grouped by `room_type` and distinguished by neighborhoods using the `hue` parameter.

#### Visualization Questions
11. **Bar Chart**  
    - Create a bar chart showing the count of listings for each `room_type`.

12. **Heatmap**  
    - Generate a heatmap showing the correlation between listing price and the frequency of reviews.

13. **Pie Chart**  
    - Create a pie chart to visualize the proportion of room types.

14. **Histogram**  
    - Plot a histogram showing the distribution of listing prices with price bins of $50.

15. **Violin Plot**  
    - Create a violin plot comparing price distributions across neighborhoods.

### **Bonus Questions**
1. **Outlier Detection**  
   - Use the interquartile range (IQR) method to identify listings with unusually high prices (outliers) and highlight them in a scatter plot.

2. **Interactive Visualization**  
   - Use `plotly` or `altair` to create an interactive visualization for price trends by neighborhood with tooltips displaying additional information such as `room_type` and `description`.
