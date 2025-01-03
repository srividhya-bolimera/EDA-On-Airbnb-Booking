# EDA on Airbnb NYC 2019 Dataset

## Project Overview
This project involves performing **Exploratory Data Analysis (EDA)** on the Airbnb NYC 2019 dataset, which contains information about 49,000 Airbnb listings. The goal is to uncover patterns, trends, and insights to assist hosts and Airbnb in making data-driven decisions.

## Dataset
- **Source**: Airbnb NYC 2019 Dataset
- **Size**: 49,000 entries with 16 attributes
- **Attributes**:
  - `id`: Unique listing ID
  - `name`: Property name
  - `host_id`: Host identifier
  - `host_name`: Host name
  - `neighbourhood_group`: Location (e.g., Manhattan, Brooklyn)
  - `neighbourhood`: Specific area
  - `latitude` & `longitude`: Geographic coordinates
  - `room_type`: Type of room (e.g., Entire home, Private room)
  - `price`: Price per night
  - `minimum_nights`: Minimum booking duration
  - `number_of_reviews`: Total reviews
  - `last_review`: Date of last review
  - `reviews_per_month`: Average reviews per month
  - `calculated_host_listings_count`: Total listings by a host
  - `availability_365`: Days available for booking

## Objectives
1. Analyze price distribution and identify trends.
2. Explore the popularity of room types and neighborhoods.
3. Study host behavior and customer preferences.
4. Provide actionable insights for hosts and Airbnb management.

## Process
### 1. **Data Wrangling**
- Loaded the dataset and conducted initial exploration (`head()`, `tail()`, `info()`).
- Handled missing values by imputing with placeholders like "Unknown."

### 2. **Exploratory Data Analysis (EDA)**
#### Key Analyses:
- **Price Distribution**: Most properties priced between $75–$500; outliers exist.
- **Room Type Analysis**:
  - Entire homes: 52%
  - Private rooms: 45.7%
  - Shared rooms: 2.4%
- **Neighborhood Analysis**:
  - Manhattan and Brooklyn dominate listings (85% combined).
  - Staten Island has the highest availability.
- **Host Analysis**:
  - A few hosts manage a large number of listings, indicating market concentration.

#### Tools Used:
- **Visualizations**:
  - **Price Distribution**: A histogram illustrates the range of listing prices, showing most properties fall between $75 and $500. Outliers indicate luxury or budget accommodations.
  - **Room Type Analysis**: Bar plots depict the prevalence of room types, highlighting the dominance of entire homes and private rooms over shared spaces.
  - **Neighborhood Insights**: Scatter plots and heatmaps show listing density and average prices by location, revealing popular and high-demand areas.
  - **Host Distribution**: Bar charts identify top hosts with multiple listings, showcasing market concentration.
  - **Correlation Analysis**: Heatmaps visualize relationships between features such as price, reviews, and availability, providing insights into influencing factors.

### 3. **Insights and Recommendations**
#### Insights:
- Manhattan commands higher prices due to demand.
- Listings with high prices have fewer reviews.
- Entire homes/apartments are the most preferred room type.

#### Recommendations:
- **For Hosts**:
  - Invest in entire homes in popular neighborhoods.
  - Experiment with shared rooms for niche markets.
- **For Airbnb**:
  - Promote less popular neighborhoods to balance demand.
  - Collaborate with top-performing hosts for marketing.

## Future Work
- Apply machine learning to predict pricing.
- Conduct sentiment analysis on customer reviews.
- Explore trends over multiple years.
