# Used_Cars_Analysis
An in depth analysis of used cars data. The analysis aimed to answer the following questions:

1. How does the mileage on a car effect its price?
2. What is the average price of a car by year for any car manufactured in 2011 or later?
3. What is the average price of a car for the top 10 most represented car brands?
4. Which brands are the most valuable and which brands are the least valuable?
5. What are the most common brand model combinations?
6. Which states have the most expensive cars, and which ones have the least?

### Breakdown

#### Data Cleaning
- Dropped any unnecessary columns from the dataset
- Removed outliers from the 'price' and 'mileage' columns
- Removed "Salvage Insurance" vehicles and kept "Clean Vehicles" only

#### Data Engineering
A few examples:
- Created a new column called mileage_bins which took the mileage column and put it into bins of 10,000 miles each
- Created a new column called "pm_ratio" by dividing the price column by the mileage column
- Created a new column called "value earned" which standardized the pm_ratio column to be between 0 and 10 (0 being lowest value, 10 being highest value). Using the values in this column is how I determined the "most valuable" and "least valuable" car brands.

#### Data Visualization
- Used the plotly library to plot bar charts and histograms to visualize the answers to the questions.
