**This is my first Udacity Data Science Project**

# Link to Medium Blog

https://medium.com/@egutierrezolmedo/exploring-seattle-homestays-7b028561ce48

# Seattle Airbnb Data Analysis

This project analyzes Airbnb data for Seattle to gain insights into rental prices and customer satisfaction.

## Project Description

This project uses data from Airbnb listings in Seattle to explore factors that influence rental prices and customer satisfaction. The analysis includes:

- Exploring the relationship between property type and review scores
- Investigating the correlation between host response time and review scores
- Analyzing the influence of proximity to top tourist attractions on rental prices

## Datasets

The main dataset used in this project is the Airbnb listings data for Seattle. This dataset includes information about each listing such as the property type, price, review score, host response time, and location (latitude and longitude).

## Requirements

This project uses Python 3 and the following libraries:

- pandas
- numpy
- matplotlib
- seaborn
- geopy
- folium

## Results

The main findings of this project include:

- Property type and host response time have a significant impact on review scores.
- Proximity to top tourist attractions is correlated with higher rental prices.

## Future Work

Future work could include a more detailed analysis of the text of the reviews to gain more insights into customer satisfaction, and an analysis of the impact of other factors such as amenities and property size on rental prices.

## How to Run

1. Clone this repository.
2. Install the required libraries.
3. Run the Jupyter notebook.

## License

N/A

## Data Cleaning

Before the analysis, the data was cleaned to handle missing values and incorrect data types. Here's a summary of the cleaning steps:

1. **Missing Values:** Columns with a high percentage of missing values were dropped. For the remaining columns, missing values were filled with appropriate values. For example, missing values in 'review_scores_rating' were filled with the mean rating.

2. **Incorrect Data Types:** Some columns were converted to the correct data types. For example, 'price' was converted from a string to a float, and 'host_response_time' was converted from a string to a categorical variable.

3. **Outliers:** Outliers in 'price' and 'review_scores_rating' were identified and handled. For 'price', listings with prices more than 3 standard deviations from the mean were considered outliers and were removed. For 'review_scores_rating', a similar approach was used.

4. **Location Data:** The latitude and longitude columns were used to calculate the distance from each listing to each of the top tourist attractions in Seattle. These distances were added as new columns to the DataFrame.

After cleaning, the data was ready for analysis.