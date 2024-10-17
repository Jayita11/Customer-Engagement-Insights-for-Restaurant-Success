# Yelp Restaurant Business Analysis


## Project Background:
Yelp is a web and mobile platform where users can discover, review, and share experiences about local businesses through crowd-sourced reviews. It allows users to submit reviews, photos, and tips, while also browsing ratings and insights from others. Yelp covers a wide range of businesses, from restaurants to services, and offers features like search filters, business profiles, and customer feedback.



## Problem Statement:
In the highly competitive restaurant industry, it is essential for stakeholders to understand the factors that drive business success. This project leverages the Yelp dataset to explore the relationship between user engagement (such as reviews, tips, and check-ins) and key success metrics (including review count and ratings) for restaurants.



## Research Objectives:
![WhatsApp Image 2024-10-16 at 9 21 10 PM](https://github.com/user-attachments/assets/1775289f-a152-445c-9afa-ae8c2e9ffd00)


## Hypothesis:
- **Higher levels of user engagement** (more reviews, tips, and check-ins) correlate with **higher review counts, average ratings**, and overall business success for restaurants.
- **Positive sentiment** in reviews (useful, funny, cool) significantly contributes to **higher average ratings** and **increased review counts** for restaurants.
- Restaurants with specific attributes (e.g., parking, alcohol availability, happy hour) will have **higher average ratings** and greater customer satisfaction compared to those without these features.
- **Elite users** have a greater influence on restaurant visibility and ratings compared to non-elite users, leading to a disproportionate contribution to restaurant success.
- **Regional and seasonal trends** affect restaurant success, with restaurants in certain cities and seasons showing **higher engagement, ratings, and review counts**.

An interactive Tableau dashboard accompanies this project to provide a dynamic and visual exploration of the findings [here]. 

The SQL queries regarding various business questions and data preparation for the Tableau dashboard can be found [here].

## Data Overview:
This dataset is a curated subset of Yelp, containing comprehensive information about businesses across eight major metropolitan areas in the USA and Canada.

The original data is provided by Yelp in the form of six JSON files: **business**, **review**, **user**, **tip**, **checkin**, and **photos**. For convenience, these JSON files have been stored in a database to facilitate efficient data retrieval and analysis.

- **Compressed Dataset Size**: 4.04 GB  
- **Uncompressed Dataset Size**: 8.65 GB  
- **Dataset Coverage**: From 2004 to 2022  
- **Dataset Source**: [Yelp Dataset](https://www.yelp.com/dataset)

![diagram](https://github.com/user-attachments/assets/0cca0f9a-8f94-4db8-86a4-fd8bc642893a)

## Executive Summary
The analysis for the Yelp Restaurant business was conducted using **SQLite**, **Python**, and **Tableau**. SQLite was utilized through Python to perform the data analysis, generating insights from the dataset, which were then visualized. Additionally, **Tableau** was used for further analysis, creating interactive dashboards to provide a comprehensive representation of the findings.

### SQLite & Python Analysis, Visualization and Findings

### How many restaurant businesses exist, how many are currently open, and what are the descriptive statistics for review count and star rating? Additionally, which restaurants have the highest number of reviews and the highest ratings?

- Out of 150K businesses, 52K are in the restaurant industry, and 35K of those restaurants are currently open.


![yelp_1](https://github.com/user-attachments/assets/963c904d-36c2-42bd-9667-3a94adfc691b)

- There is no direct correlation between high ratings and high review counts; restaurants with perfect ratings often have fewer reviews.
- Review count reflects user engagement but not necessarily overall customer satisfaction or business performance.
- Success in the restaurant industry is influenced by more than just ratings or review counts, as businesses with lower ratings can still attract higher customer engagement, and top-rated restaurants may have limited exposure.

### Do restaurants with higher engagement (reviews, tips, check-ins) tend to have higher ratings?

- The data reveals a general upward trend in average review, check-in, and tip counts as ratings increase from 1 to 4 stars.
- Restaurants with a 4-star rating demonstrate the highest overall engagement across reviews, check-ins, and tips, suggesting that user interaction peaks at this rating.
- Interestingly, engagement metrics (reviews, check-ins, tips) begin to decline slightly at 4.5 stars and drop more significantly at the 5-star level.
- The dip in engagement at 5 stars may indicate a saturation point where fewer customers feel the need to provide additional feedback, or it could suggest that only a small, highly satisfied customer base frequents these top-rated establishments.

  ![yelp_2](https://github.com/user-attachments/assets/87c7100e-f61c-4abc-86fa-9c8572a6d6fb)


### Is there a correlation between the number of reviews, tips, and check-ins for a business?

- These correlations suggest that user engagement across different platforms (reviews, tips, and check-ins) is interlinked; higher activity in one area tends to be associated with higher activity in others.
- Businesses should focus on strategies that boost all types of user engagement, as increases in one type of engagement are likely to drive increases in others, enhancing overall visibility and interaction with customers.
![yelp_8](https://github.com/user-attachments/assets/420ef8ec-a9a9-402e-93a0-d330689523c8)
### Is there a difference in the user engagement (reviews, tips, and check-ins) between high-rated and low-rated businesses?

- Data indicates a clear correlation between higher ratings and increased user engagement across reviews, tips, and check-ins.
- This pattern underscores the importance of maintaining high service and quality standards, as these appear to drive more reviews, check-ins, and tips, which are critical metrics of customer engagement and satisfaction.
- Businesses should focus on strategies that boost all types of user engagement, as increases in one type of engagement are likely to drive increases in others, enhancing overall visibility and interaction with customers.

 ![yelp_3](https://github.com/user-attachments/assets/72b74b57-9504-4a82-a634-376193f7f902)

### How do restaurant attributes like parking, alcohol, happy hour, TV availability, noise level, smoking, and 24-hour availability correlate with star ratings?

- Alcohol availability and happy hour offerings have a moderate positive correlation with star ratings, indicating that these amenities tend to increase customer satisfaction and receive slightly higher ratings.
- Parking and TV availability have weaker correlations with star ratings, showing a less pronounced effect on customer satisfaction.
- Noise level, smoking policies, and 24-hour availability show little to no influence on star ratings.
- Focusing on enhancing amenities like alcohol and happy hour can significantly boost customer satisfaction, while other features may not have a strong impact on ratings.
- Overall, businesses should consider focusing on alcohol service and happy hour promotions as these factors appear to have the greatest positive influence on customer ratings, while amenities like TVs and 24-hour availability may not significantly boost ratings.
  
![Screenshot 2024-10-16 at 11 18 52 PM](https://github.com/user-attachments/assets/4e1fa962-dd31-4475-a883-9dd89ca8e674)

### How do the success metrics (review_count or avg_rating) of restaurants vary across different states and cities?

- **Philadelphia** emerges as the top city with the highest success score, indicating a combination of high ratings and active user engagement.
- Following Philadelphia, **Tampa**, **Indianapolis**, and **Tucson** rank among the top cities with significant success scores, suggesting thriving restaurant scenes in these areas.
- The success metrics vary significantly across different states and cities, highlighting regional differences in dining preferences, culinary scenes, and customer engagement levels.
- Identifying cities with high success scores presents opportunities for restaurant chains to expand or invest further, while areas with lower scores may require targeted efforts to improve ratings and increase user engagement.
  
![Screenshot 2024-10-16 at 11 19 55 PM](https://github.com/user-attachments/assets/b9f9304b-c423-429a-8975-a16693d44624)


### Which cities have the highest number of restaurants, and how does restaurant distribution compare across city areas?

- **Philadelphia** stands out with a strong restaurant presence, signaling a thriving food culture and opportunities for food-related tourism and local business growth.
- Cities like **Tampa** and **Indianapolis** show competitive dining markets, attracting both locals and tourists.
- **Edmonton** highlights a strong restaurant scene in Canada, reflecting cultural diversity and economic growth.
- **Tucson**, **Nashville**, and **New Orleans** have vibrant food scenes, driving local economies and attracting food enthusiasts and supporting local economies.
- Smaller cities such as **Reno** and **Boise** demonstrate emerging restaurant markets, catering to growing populations and regional tourism.
  
![Screenshot 2024-10-16 at 11 21 12 PM](https://github.com/user-attachments/assets/29ce6e71-44ab-4a69-85b3-2a9770c149a5)

### How do restaurants in different cities compare in terms of categories and average ratings?

- **Philadelphia** shows a diverse range of restaurant categories, with pizza and Chinese cuisine making up a significant portion, but with lower average ratings.
- **Tucson** and **Indianapolis** have higher average ratings, particularly for Mexican cuisine, suggesting strong customer satisfaction in these categories.
- The variation in restaurant categories and ratings across cities highlights regional preferences and areas for potential improvement, especially in cities with lower average ratings like Philadelphia.

![yelp_4](https://github.com/user-attachments/assets/3f2932ac-941f-464f-bef2-b159d2eafb8a)

### Is there any difference in engagement of elite users and non-elite users?

- **Elite users** are individuals who have been recognized and awarded the "Elite" status by Yelp for their active and high-quality contributions to the platform, such as frequent and detailed reviews, photos, and check-ins, among other criteria.
- Elite users, despite being significantly fewer in number, contribute a substantial proportion of the total review count compared to non-elite users.
- Elite users often provide detailed and insightful reviews, which can influence other users' perceptions and decisions regarding a business.
- Reviews from elite users may receive more attention and visibility on the Yelp platform due to their status, potentially leading to higher exposure for businesses.
- Establishing a positive relationship with elite users can lead to repeat visits and loyalty, as they are more likely to continue supporting businesses they have had good experiences with.

![yelp_5](https://github.com/user-attachments/assets/1d719dc1-cd33-43ea-8b41-c600b44774ff)

### What are the busiest hours for restaurants?

- The busiest hours for restaurants, based on user engagement, span from **4 pm to 1 am**.
- Knowing the peak hours allows businesses to optimize their staffing levels and resource allocation during these times to ensure efficient operations and quality service delivery.
- User engagement is concentrated during evening and night hours, indicating higher demand for dining out during these times, possibly influenced by work schedules, social gatherings, and leisure activities.
  
![Screenshot 2024-10-16 at 11 27 16 PM](https://github.com/user-attachments/assets/1e1ddc35-5221-436a-80f2-ad2453684d9e)

### How many users have left tips to more businesses than reviews, and how does user engagement vary between leaving tips and reviews?

- Most users are more likely to leave **reviews** than tips, indicating that reviews are the preferred form of engagement.
- A smaller but significant group of users engages equally in leaving both tips and reviews, showing a balanced interaction.
- Few users prioritize leaving tips over reviews, suggesting that tips are less common but may still offer valuable insights for businesses.
- Businesses should focus more on encouraging reviews while also recognizing the value of tips as a form of user engagement.
- 
![yelp_6](https://github.com/user-attachments/assets/171a423b-f847-46e9-b76d-76566d3e55ec)

### Are there any patterns in user engagement over time for successful businesses compared to less successful ones?

- Successful businesses, especially those with higher ratings (above 3.5), demonstrate consistent or increasing user engagement over time.
- High-rated restaurants maintain a steady or growing level of user interaction, indicating strong customer interest and satisfaction.
![yelp_9](https://github.com/user-attachments/assets/69ebaab9-4a35-43d7-a81e-3fd31e5fd104)
### Are there any seasonal trends in the user engagement for restaurants?

- Tip engagement shows a declining trend, while review engagement follows an upward trajectory, suggesting a shift in how customers interact over time.
- Seasonal trends are evident, with peak engagement occurring at the beginning and end of the year (around November to March), highlighting key periods for increased customer activity.
![yelp_10](https://github.com/user-attachments/assets/7a25a08e-7895-4dfc-853d-c8f988ccfbbf)
### How does the sentiment of reviews and tips (useful, funny, cool) correlate with the success metrics of restaurants?

- **Useful**, **funny**, and **cool** counts from reviews are strongly correlated with review count, suggesting that more engaging and well-received reviews lead to higher overall review activity.
- Useful counts have the strongest correlation with other engagement metrics (review count, cool count), indicating that reviews perceived as helpful play a key role in driving engagement.
- Higher counts of **useful**, **funny**, and **cool** reviews are associated with a higher success score, highlighting the importance of engaging user feedback for restaurant success.
- Overall, user sentiment metrics contribute significantly to a restaurant's performance, with higher engagement across these categories linked to better business outcomes.
  
![Screenshot 2024-10-16 at 11 30 36 PM](https://github.com/user-attachments/assets/ab379aae-cf10-4e91-ac7f-0032c77464ca)

### Do users who post more reviews tend to have more fans, and how does this relationship manifest for the top 10 users with the most fans?

- For all users, there is a moderate positive correlation between the number of reviews and the number of fans, suggesting that higher review activity is generally associated with more fans.
- Among the top 10 users, however, this correlation weakens significantly, implying that once users reach a certain level of fame, additional reviews do not necessarily lead to more fans.
- **Funny** and **cool** reviews tend to correlate more with user engagement metrics (useful, funny, cool counts), while average rating has a weak negative correlation with these metrics.
- High engagement metrics such as useful, funny, and cool reviews are key drivers of fan growth for these top users, emphasizing the value of high-quality, engaging reviews over sheer quantity.

![yelp_7](https://github.com/user-attachments/assets/e008cc11-72d4-416a-a5e7-be36c46a3cf5)






### Tableau Analysis & Dashboard
#### Home Page
- This is the Home Page for the Yelp Restaurant Analysis Tableau dashboard.The page allows easy navigation to various detailed dashboards through clickable icons.
  
- Each icon directs to a specific section, including Overview, Geographic Insights, User Interaction, Reviews, and Ratings.
  
- Users can explore different aspects of the Yelp restaurant data by selecting the relevant dashboard based on their needs.

  ![home](https://github.com/user-attachments/assets/66fdc970-6f39-46f5-9cc6-8b01834df2a5)
  
#### Overview Dashboard
- Nearly 67% of restaurants are currently open, indicating a majority of the restaurant industry is active, while 33% are closed, which may point to challenges in the market.

- Pennsylvania (PA) leads significantly, followed by Florida (FL) and Tennessee (TN), suggesting that these states have the highest concentration of restaurants and could be key markets for growth opportunities.

- Philadelphia stands out with the highest number of restaurants, followed by Tampa, Nashville, and Tucson, indicating strong restaurant activity in these urban areas and potential hubs for dining culture.
  
- The geographic distribution shows significant clusters of both open and closed restaurants in key regions, with larger markets like Pennsylvania and Florida having a higher concentration of operational restaurants, which suggests these areas are resilient despite market challenges.
  
  ![Screenshot 2024-10-16 at 9 36 15 PM](https://github.com/user-attachments/assets/252ef865-c041-429d-afb7-648a836f683c)

#### Geographic Analysis Dashboard
- North Redington Beach stands out with the highest average review count, suggesting a strong customer engagement in this area, while cities like Manayunk and Tarpon Springs also show high review activity, indicating these are key markets for user interaction.
  
- California (CA) leads with the highest average review count, followed by Nevada (NV) and Louisiana (LA). These states show significantly more user engagement per restaurant, making them key regions for business opportunities.
  
- The geographic distribution shows high concentrations of restaurants in key states such as California, Florida, and Pennsylvania, which are major hubs for dining culture and could be prioritized for expansion and marketing efforts.

![Screenshot 2024-10-16 at 9 40 36 PM](https://github.com/user-attachments/assets/0f94993d-a793-407e-a2a1-b86b56064636)

#### User Analysis Dashboard
- John leads with the most fans, followed by Michael and David, suggesting that these users have the greatest influence within the platform. These top users likely drive significant visibility and engagement for the restaurants they review.
  
- The useful attribute dominates user interactions, with 2.6 million useful votes, followed by cool and funny votes. This suggests that users value helpful reviews the most, making it essential for businesses to encourage meaningful and informative reviews.
  
- The number of users and reviews peaked around 2011-2015, with a noticeable drop in recent years. This highlights an opportunity to re-engage users and stimulate review activity to match earlier participation levels.
  
![Screenshot 2024-10-16 at 9 37 23 PM](https://github.com/user-attachments/assets/8c6f1eeb-c8d3-404a-b6bc-3b7424db90f2)

#### Reviews Analysis Dashboard
- The vast majority of reviews (around 81%) are positive, reflecting overall customer satisfaction, while 19% are negative, indicating areas for improvement in certain restaurants.
  
- McDonald's leads significantly in terms of review count, followed by Taco Bell and Chick-fil-A, suggesting these brands have high visibility and customer interaction on the platform.
  
- Review counts peaked around 2018-2019, with a decline in recent years. This suggests a potential decline in user engagement or external factors affecting customer feedback activity, signaling an opportunity to re-engage users.
  
- Restaurants in New Orleans dominate the list of businesses with the most reviews, showing strong engagement from customers in that area and highlighting New Orleans as a key hub for restaurant activity and feedback.

![Screenshot 2024-10-16 at 9 37 59 PM](https://github.com/user-attachments/assets/410cd6b6-e386-46fe-a73b-32975785fc26)

#### Ratings Analysis Dashboard
- The majority of ratings fall between 3.5, 4 and 4.5 stars, suggesting that most restaurants receive positive feedback, with a smaller portion receiving ratings below 3. This indicates a generally high level of customer satisfaction.
  
- A large portion of restaurants have 4 and 4.5 stars, making this the most common rating range. Only a small fraction of restaurants have 2.5 stars or below, which highlights the high performance of most restaurants on the platform.
  
- Most restaurants have been rated good, with a few receiving neutral or bad ratings. This highlights the overall positive performance of restaurants, while those with neutral or bad ratings may need to focus on customer service improvements to enhance their reputation.

![Screenshot 2024-10-16 at 9 38 07 PM](https://github.com/user-attachments/assets/7fed9e69-6236-4b7d-bd77-0ce6a415b61c)

