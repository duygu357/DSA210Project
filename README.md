# Understanding Consumer Behaviour of EV car buyers


## Project Overview
Electric vehicles (EVs) are at the forefront of the global transition toward sustainable transportation. With advancements in technology, growing environmental concerns, and shifting consumer preferences, the factors that drive EV adoption are more complex than ever. This project leverages data science techniques to analyze EV consumer behavior, with a particular focus on understanding how geographic and performance-related variables influence purchasing decisions. By integrating spatial data, EV sales figures, and brand performance metrics, this project aims to uncover the key trends and predictors that will help stakeholders—from manufacturers and marketers to policymakers—navigate the growing EV market.

## Project Motivation
The automotive industry is undergoing a major transformation as consumers pivot from traditional combustion engines to electric vehicles. Despite technological improvements, consumer acceptance remains a critical factor in the success of EVs. This project is motivated by the need to:

- Forecast Adoption Trends: Identify and quantify the factors that drive consumer decisions toward EVs, enabling better market forecasting.
- Support Strategic Decision-Making: Provide insights that can guide manufacturers in optimizing product features, pricing, and marketing strategies.
- Enhance Consumer Understanding: Find how factors such as geographic altitude, charging infrastructure, and brand reliability impact buyer behavior, fostering a smoother transition to sustainable transportation.

  
## Objectives
- Identify Consumer Behavior Drivers: Examine how environmental and performance factors—including spatial characteristics, charging station availability, and vehicle performance metrics influence EV purchasing decisions.
- Analyze Key Predictors: Determine which variables, such as charging time, range, price, and body style, have the strongest impact on consumer behavior.

  
## Dataset
The project will integrate two types datasets with 14 different features;

> Spatial Data:
- Average Altitude: The average altidute of the cities.
- Charging Station Locations: The total number of electric vehicle charging stations available in a specific city or region.
- Air Pollution: The percentage of air pollution attributed death to explore whether one of the motivation of the consumers is environmental concerns or not.
> EV Sales and Performance Data:

- Acceleration Second: The time (in seconds) the vehicle takes to accelerate (from 0 to 100 km/h). This is a performance parameter reflecting the vehicle's acceleration capabilities.
- Top Speed: The maximum speed the EV can achieve, measured in kilometers per hour. It provides insight into the vehicle’s performance limits.
- Range: The estimated distance the vehicle can travel on a single charge, expressed in kilometers. 
- Efficiency: The energy efficiency of the EV, measured in watt-hours per kilometer. Lower values indicate higher efficiency and better energy conservation.
- Fast Charge: The rate of fast charging expressed as the additional range (in kilometers) provided per hour of fast charging.
- Power Train: Details about the EV’s powertrain configuration, including the type of electric motor(s) and drivetrain layout (e.g., front-wheel, rear-wheel, all-wheel drive). This affects both performance and efficiency.
- Body Style: The overall design or structure of the vehicle (e.g., sedan, hatchback, SUV, coupe). It influences consumer preferences based on aesthetics and utility.
- Seats: The number of passenger seats in the vehicle. This detail indicates the vehicle’s capacity, which can be important for family or commercial use.
- PriceEuro: The price of the EV expressed in euros. This variable is a crucial economic factor.
- Sales: Number of cars in particular model that is bought in 2023.
> Brand Analysis
- Brand: The manufacturer of the electric vehicle (EV), such as Tesla, Nissan, or BMW. This variable helps identify the company behind each model.
- Car accident rates: To understand the security of the brands from the consumers' perspective, percentage of car accidents of the brands will be used. Having a whole World data is almost impossible that's why smaple size will be shrinked to USA only.
 

> The main resources of the project's dataset;
- EV sales and performance features  will be taken from (can be obtained in .csv format) ;
https://www.kaggle.com/datasets/geoffnel/evs-one-electric-vehicle-dataset
- Air pollution deaths from fossil fuels, 2015 (can be obtained both .csv and .json format);
https://ourworldindata.org/grapher/pollution-deaths-from-fossil-fuels?tab=table
- Car accidents vs. brands;
https://www.lendingtree.com/insurance/brand-incidents-study/


## Tools and Technologies
The project will be implemented using:

- Python: The primary programming language for data analysis and modeling.
- Pandas & GeoPandas: For data manipulation, preprocessing, and geospatial data handling.
- Matplotlib & Seaborn: For creating visualizations like scatter plots, heatmaps, and geographic maps.
- SciPy: For hypothesis testing and statistical analysis.

## Analysis Plan
- Data Collection & Preprocessing:

Import and merge datasets from various sources given in the dataset section, ensuring consistency in units and formats.
Clean the data by handling missing values and standardizing variables.

- Data Visualization:

Using different type of plottig techniques -scatter, heatmap- to discover the relations. For example;
1. Scatter plot of accelaration second vs sales;
2. To compare performance metrics, bar chart of the brand vs performance paarameters can be plotted.
3. Track changes in air pollution indices with line chart over time to see if there’s a correlation with EV adoption.

- Hypothesis Testing & Predictive Modeling:

Formulate and test hypotheses such as;
H₀: Geographic and performance-related factors have no significant effect on EV consumer behavior.
Hₐ: One or more factors significantly influence EV adoption.
Apply regression analysis to quantify the impact of variables like charging station density, and brand reliability.
Use clustering algorithms to segment consumers based on their preferences and behavior.
- Trend and Sensitivity Analysis:

Evaluate how regional differences in altitude and charging infrastructure correlate with EV sales.
Analyze the sensitivity of consumer behavior to changes in vehicle performance attributes and brand reputation.

## Example;

It can be constructed a scatter plot with the Air Pollution Index on the x-axis and monthly EV sales on the y-axis. A rising trend in this graph may indicate that higher pollution levels are associated with increased EV adoption, suggesting that environmental concerns are motivating consumers.
Or by segregating regions into those with high and low densities of charging stations, it can be generated comparative visualizations. This analysis will help determine whether areas with more charging points experience higher EV sales, potentially reflecting enhanced consumer confidence due to improved accessibility.

## Conclusion
By the end of this project, the goal is to provide insights that answer these research questions such as:

- Which geographic and performance related factors most influence EV adoption?
- How do charging infrastructure and air pollution impact consumer decision-making?
- What role do brand safety metrics play in shaping consumer sentiment?
- How can manufacturers and policymakers leverage these insights to drive a smoother transition to sustainable transportation?
- This project not only aims to analyze EV adoption trends but also to build a roadmap for the rapidly growing EV market. The findings are expected to offer a comprehensive view of consumer behavior in the EV sector.

