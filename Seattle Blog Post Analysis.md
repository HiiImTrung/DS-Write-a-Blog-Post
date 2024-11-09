







<h2 id='part1'>Seattle Airbnb Analysis</h2>


In this blog post, using the Seattle Airbnb (https://www.kaggle.com/datasets/airbnb/seattle/data) dataset from Kaggle, we would like to deep dive and discuss these three business-oriented questions:

1. What are the seasonal trends in pricing across Seattle?
2. What factors impact a listing's average rating or occupancy?
3. Are there certain neighborhoods or property types with the highest bookings?


<h3 id='Context'>Context</h3>

Since 2008, guests and hosts have used Airbnb to travel in a more unique, personalized way. As part of the Airbnb Inside initiative, this dataset describes the listing activity of homestays in Seattle, WA.


<h3 id='Exploration'>Exploration</h3>

We first access and explore the Seattle Airbnb dataset, gaining insights into its structure and contents.

<h3 id='Data Preparation'>Data Preparation</h3>

After exploring the data, we preprocess it to ensure it's ready for analysis. This involves handling missing values, encoding categorical variables, and cleaning inconsistencies.

<h3 id='Finding results'>Finding results</h3>



Q1: What are the seasonal trends in pricing across Seattle?

Prices in Seattle tend to peak in the summer months, suggesting high demand in warmer weather.

![image.png](attachment:image.png)

Q2: What factors impact a listing's average rating or occupancy?

1. Correlation Heatmap Findings:
Review Scores vs. Review Count: The correlation between review_scores_value and review_count is -0.037, which is very close to zero. This indicates almost no correlation between the number of reviews a listing has and its review score. In other words, whether a listing has many reviews or few does not appear to impact the review score significantly.

2. Price vs. Review Score Scatter Plot:
The scatter plot shows the distribution of review scores across different price points. The following trends are observable:

High Concentration of Scores around 10: Many listings have review scores near the maximum of 10, suggesting that a majority of listings are rated positively, regardless of price.

Wide Price Range with High Scores: Listings with high review scores (8-10) are spread across a wide range of prices, indicating that guests tend to leave good reviews regardless of the listing's price.

Sparse Low Scores: There are fewer listings with review scores below 7, and these are scattered across various price ranges. Low scores are not concentrated in any specific price range, suggesting that factors other than price may drive lower review scores.

Summary:
Overall, these findings suggest that review scores are generally positive and not strongly influenced by either price or the number of reviews. Guests may value factors unrelated to price when leaving high ratings, which could indicate the importance of non-monetary aspects such as cleanliness, location, or service quality in determining review scores.

![image.png](attachment:image.png)

Q3: Are there certain neighborhoods or property types with the highest bookings?

Top Neighborhoods by Average Reviews:

International District has the highest average number of reviews, indicating a popular area with likely high bookings or demand.

Harrison/Denny-Blaine and Whittier Heights also show high average review counts, suggesting these areas are in demand and may experience frequent bookings.

Other High-Interest Neighborhoods:

Neighborhoods such as Riverview, South Delridge, and Georgetown also have relatively high average review counts, indicating they attract significant interest and engagement from visitors.


![image.png](attachment:image.png)

 Key Insights and Conclusions
1. **Seasonal Price Trends**: Prices in Seattle tend to peak in the summer months, suggesting high demand in warmer weather.
2. **Factors Affecting Ratings**: Guests may value factors unrelated to price when leaving high ratings, which could indicate the importance of non-monetary aspects such as cleanliness, location, or service quality in determining review scores.
3. **Popular Neighborhoods**: The analysis indicates that certain neighborhoods, particularly International District and Harrison/Denny-Blaine, likely experience higher bookings due to their popularity as reflected in review counts.
