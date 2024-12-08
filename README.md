# Netflix Content Analytics: Uncovering Insights with Power BI

## Introduction
Netflix, a giant in the streaming industry, hosts a massive catalog of TV shows and movies that cater to diverse audiences worldwide. Understanding the underlying patterns in this content can provide critical insights for decision-making and audience engagement. In this project, Power BI was used as a powerful tool to analyze Netflix’s data and develop actionable insights.

This end-to-end project involves data cleaning, transformation, modeling, and visualization to deliver an insightful dashboard that captures various metrics such as content ratings, votes, genres, and geographic distributions.

---

## About the Data
The dataset used in this project was sourced from a public GitHub repository: [PowerBIbro's GitHub profile](https://github.com/powerbibro/powerbibro). It contains key details about Netflix titles, including:

- **Title**: Name of the show or movie.
- **Rating**: Audience rating (e.g., 7.8).
- **Votes**: Number of votes received by each title.
- **Genre**: Category of the title, such as Action, Drama, or Comedy.
- **Country**: The primary country of origin for the content.
- **Listing Type**: Indicates whether the content is a movie or TV show.

This dataset is a rich source for examining trends in ratings, the popularity of genres, and the geographic spread of Netflix's catalog.

---

## Methodology
1. **Data Collection**:
   The dataset was downloaded directly from the GitHub repository in CSV format.
   
2. **Data Cleaning and Transformation**:
   All data cleaning and transformations were conducted within Power BI using Power Query, ensuring seamless integration with the data model.

3. **Data Modeling**:
   A star schema was adopted to simplify the analysis and establish relationships between tables like Listings, Ratings, and Countries.

4. **Data Analysis and Visualization**:
   Comprehensive dashboards were created in Power BI to showcase insights using various visualizations, including bar charts, pie charts, and maps.

---

## Data Cleaning and Transformation
Using Power BI's **Power Query** Editor, the following transformations were applied:

1. **Handling Missing Values**:
   - Rows with significant missing data in critical fields (like Title or Rating) were removed.
   - Non-critical missing fields were filled with placeholder values.

2. **Column Splits and Merging**:
   - Split multi-value columns like genres into individual entries for cleaner analysis.
   - Merged certain country labels for consistency (e.g., "United States" and "USA").
   
3. **Data Type Corrections**:
   - Converted numerical fields like Ratings and Votes to their appropriate data types.
   - Corrected text fields to ensure proper capitalization.

4. **Derived Columns**:
   - Added calculated columns for metrics such as `Votes per Title` and percentage contributions.

---

## Data Structure
Below is the cleaned structure of the dataset:

| **Field Name**       | **Data Type**  | **Description**                         |
|-----------------------|----------------|-----------------------------------------|
| Title                | Text           | Name of the Netflix content             |
| Rating               | Decimal        | Average audience rating (0–10 scale)    |
| Votes                | Integer        | Number of audience votes                |
| Genre                | Text           | Primary genre of the content            |
| Country              | Text           | Country of origin                       |
| Listing Type         | Text           | Movie or TV show                        |

![image](https://github.com/yungstarry/Netflix_DA/blob/main/DatastuctureNetflix.png?raw=true)
![image](https://github.com/user-attachments/assets/79b1b00b-99df-4fb1-a4c4-24b65aed8487)
![image](https://github.com/user-attachments/assets/ebb83cbc-2626-4a27-b356-fa8d3200e019)


---

## Data Model Overview
![image](https://github.com/user-attachments/assets/0133c4b9-e157-49a7-8304-3c9805228edd)


---

## Analysis
The analysis focuses on uncovering patterns in Netflix's catalog. Key visualizations and metrics include:

1. **Number of Titles by Rating Group**:
   - A bar chart reveals the distribution of Netflix titles across rating groups, highlighting the dominance of titles in the mid-range (6–8 ratings).

2. **Average Ratings and Number of Titles by Genre**:
   - A combined bar and line chart provides insights into how various genres perform based on ratings and the number of titles.

3. **Geographical Distribution of Netflix Titles**:
   - A bubble map visualizes the concentration of Netflix content by country, emphasizing the heavy contribution from the United States and the United Kingdom.

4. **Votes per Title**:
   - A table ranks countries by their average number of votes per title, showcasing audience engagement by region.

---

## Dashboard Insights
The dashboard captures several key takeaways:

1. **Most Titles Are Rated Between 6 and 8**:
   - Titles in this range dominate the catalog, indicating Netflix's focus on content that appeals to a broad audience.

2. **Movies vs. TV Shows**:
   - TV shows tend to have slightly higher average ratings compared to movies, reflecting deeper audience engagement with serialized content.

3. **Top Contributing Countries**:
   - The United States leads in content production, followed by the United Kingdom and Japan.

4. **Genre Performance**:
   - Genres like Documentary and Animation have higher average ratings but lower title counts, suggesting they cater to niche audiences.

5. **Audience Votes**:
   - Popular titles (e.g., Stranger Things, Money Heist) receive significantly higher votes, indicating fan loyalty and widespread viewership.

![image](https://github.com/yungstarry/Netflix_DA/blob/main/DashboardNeflix.png?raw=true)
![image](https://github.com/yungstarry/Netflix_DA/blob/main/ChartNetflix1.png?raw=true)
![image](https://github.com/yungstarry/Netflix_DA/blob/main/ChartNetflix2.png?raw=true)
![image](https://github.com/yungstarry/Netflix_DA/blob/main/ChartNetflix3.png?raw=true)


---

## Recommendations
1. **Expand Genre Variety**:
   - Netflix could consider investing in underrepresented but highly rated genres like Documentaries and Animation to attract niche audiences.

2. **Focus on Regional Content**:
   - Growing contributions from countries like Japan and India suggest an opportunity to further localize and diversify Netflix's content library.

3. **Enhance Engagement for Lower-Rated Titles**:
   - Introduce features like recommendations or better categorization to improve the visibility of mid-range titles.

4. **Leverage Highly Engaged Regions**:
   - Countries with high engagement (votes per title) present opportunities for targeted marketing and exclusive content launches.
