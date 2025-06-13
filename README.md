# Python-Project-AirBnb-Listing-2025
## Project Overview
This project performs Exploratory Data Analysis (EDA) on New York Airbnb data to uncover trends and patterns in rental listings. We use libraries like Pandas, Numpy, Matplotlib, Seabornfor cleaning, visualization, and analysis.

<p align="center">
  <img src="airbnb.png"  width="500"/>
</p>

## Objective
The goal of this project is to:
1. Analyze room types, prices, and availability across different neighborhoods.  
2. Understand host behavior and listing patterns.  
3. Detect potential outliers in prices.  
4. Provide recommendations for guests and hosts based on insights.

## Dataset
The dataset contains 20,765 entries and 22 features, including:

- **id**: Unique identifier for each listing
- __name__: Title of the Airbnb listing
- __host_name__: Name of the host
- __neighborhood_group__: Group (borough) where the listing is located
- __latitude/longitude__: Geolocation of listings
- __price__: Nightly rental price
- __room_type__: Type of accommodation (e.g., entire home, private room)
- __reviews_per_month__: Average monthly reviews for the listing
- __availability_365__: Number of available days in the year

## Steps and Workflow
### 1. Data Cleaning
+ Handle missing data: price, neighborhood, and beds columns had null values.
+ Fix data types: Converted last_review to a datetime object.
+ Remove outliers: Listings with prices > $1,000 were capped to avoid skewed visualizations.
### 2. EDA (Exploratory Data Analysis)
__1. Room type distribution:__

  - Visualized the count of each room type using bar plots.
  - Identified Entire home/apt as the most common room type.

__2. Neighborhood group insights:__

  - Analyzed price variations by boroughs.
  - Manhattan had the highest average prices.

__3. Availability trends:__


  - Used heatmaps to show correlations among price, availability_365, number_of_reviews, and beds.

__4. Price distribution:__

  - Used histograms to show the distribution of prices.
  - Majority of the listings were priced between $50 - $300.

__5. Host listings:__

  - Analyzed hosts with multiple listings using boxplots to identify key contributors.

__6. Review behavior:__

  - Used pair plots to show relationships between number of reviews, price, and availability.
### 3. Data Visualization

+ __Pairplot__: To see correlations among price, availability, and number of reviews.
+ __Heatmap__: Showing correlations among numerical features.
+ __Histograms and Boxplots__: To detect outliers in price.
+ __Bar Charts:__ Displaying room types and neighborhood group distributions.

## Key Findings and Insights
__1. Price Trends:__

+ Manhattan has the most expensive listings, followed by Brooklyn.
+ Entire homes/apartments cost significantly more than private or shared rooms.

__2. Room Type Distribution:__

+ Entire homes/apartments are the most common, but private rooms offer budget-friendly options.
  
__3. Outliers in Price:__

+ Few listings priced at $10,000+ were detected, indicating the need to filter such extreme values.
  
__4. Availability Patterns:__

+ Listings with high availability tend to have lower prices and more reviews, likely due to better guest experience.
  
__5. Host Behavior:__

+ Some hosts manage multiple listings, indicating a trend toward professional hosting.

## 🚀 How to Run This Project

**1. Clone the repository:**  
```bash
git clone https://github.com/smriti1303/Python-Project-AirBnb-Listing-2025.git
```

**2. Install the required libraries:**

Run this command in your terminal to install all necessary Python packages:

```bash
pip install pandas numpy matplotlib seaborn
```

**3. Run the Jupyter Notebook Or Python Script:**
```bash
jupyter notebook airbnb_eda_2025.ipynb
```
