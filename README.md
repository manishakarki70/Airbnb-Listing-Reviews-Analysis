# Airbnb-Listing-Reviews-Analysis

This project analyzes Airbnb listings and reviews data, focusing on Paris, to uncover trends and insights about hosts, neighborhoods, and pricing. The analysis is performed using Python and leverages libraries such as pandas, seaborn, and matplotlib for data manipulation and visualization.

**Key Steps in the Analysis:**

1. Data Loading and Initial Exploration:

     º  The dataset is loaded from a CSV file (Listings.csv) using pandas.read_csv with appropriate encoding and parsing options.
   
     º  Initial exploration includes inspecting the first few rows (head()), checking data types and memory usage (info()), and converting the host_since column to a datetime format.
   
2. Filtering and Selecting Relevant Data:

      º  The dataset is filtered to focus on listings in Paris using a query on the city column.
   
      º  Relevant columns such as host_since, neighbourhood, city, accommodates, and price are selected for further analysis.

3. Handling Missing Data:

      º  Missing values in the filtered dataset are identified using isna().sum().

4. Descriptive Statistics:

      º  Summary statistics for the Paris listings are generated using describe().

5. Specific Queries:

      º  Listings with zero accommodations and zero price are identified using a query.
   
6. Neighborhood-Level Analysis:

     º  The average price per neighborhood is calculated using groupby and agg, and the results are sorted by price.

7. Accommodation Capacity Analysis:

     º  The average price for listings in the "Elysee" neighborhood is analyzed based on accommodation capacity.

8. Time-Series Analysis:

     º  Listings are resampled by year to analyze trends over time, such as the number of new hosts and average prices.

9. Data Visualization:

     º  Bar plots are created to visualize:

        → Average listing prices by neighborhood.

        → Average listing prices by accommodation capacity.
   
     º  Line plots are used to show:

        → The number of new Airbnb hosts in Paris over time.

        → Average Airbnb prices in Paris over time.
   
     º  A combined plot with dual y-axes illustrates the relationship between new hosts and average prices over time, highlighting the impact of 2015 regulations.

**Tools and Libraries:** 

      º pandas: For data manipulation and analysis.

      º seaborn: For creating aesthetically pleasing visualizations.

      º matplotlib: For advanced plotting and customization.

**Insights and Goals:**

 The project aims to provide insights into:

      º The distribution of Airbnb prices across Paris neighborhoods.

      º The relationship between accommodation capacity and pricing.

      º Trends in new Airbnb hosts and pricing over time, particularly in response to regulatory changes.

The analysis is designed to help stakeholders, such as policymakers, hosts, and potential guests, better understand the dynamics of the Airbnb market in Paris.
  
