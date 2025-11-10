# yulu_confidence_interval_and_central_limit_theorem_analysis

## Overview
1. About Yulu- <br>
i. Yulu is India's leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting. <br>
ii. Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and convenient! <br>
iii. Yulu has recently suffered considerable dips in its revenues. They have contracted a consulting company to understand the factors on which the demand for these shared electric cycles depends. Specifically, they want to understand the factors affecting the demand for these shared electric cycles in the Indian market. <br>
2. The company wants to know: <br>
i. Which variables are significant in predicting the demand for shared electric cycles in the Indian market? <br>
ii. How well those variables describe the electric cycle demands? <br>
3. Column Profiling: <br>
i. datetime: datetime <br>
ii. season: <br>
a. 1: Spring <br>
b. 2: Summer <br>
c. 3: Fall <br>
d. 4: Winter <br>
iii. holiday: whether day is a holiday or not <br>
iv. workingday: if day is neither weekend nor holiday is 1, otherwise is 0. <br>
v. weather: <br>
a. 1: Clear, Few clouds, partly cloudy, partly cloudy <br>
b. 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist <br>
c. 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds <br>
d. 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog <br>
vi. temp: temperature in Celsius <br>
vii. atemp: feeling temperature in Celsius <br>
viii. humidity: humidity <br>
ix. windspeed: wind speed <br>
x. casual: count of casual users <br>
xi. registered: count of registered users <br>
xii. count: count of total rental bikes including both casual and registered <br>


 
## Insights and Recommendations <br>
1. Demand Drivers Identified: <br>
i. Weather: Rentals drop by 40-60% in poor weather (rain/storms). Clear days (Weather 1)  account for 70.8% of total rentals. <br>
ii. Seasonality: Fall (Season 3) has 31% higher demand than Spring (Season 1). <br>
iii. User Base: Registered users drive 97% of total rentals. <br>
iv. Temperature: Moderate correlation (r = 0.39) rentals peak at 25-30°C. <br>
2. Statistical Insights: <br>
i. Weather and season significantly impact demand (ANOVA/Kruskal-Wallis: p < 0.05). <br>
ii. Weekdays vs. weekends show marginal difference (p = 0.065), but holidays have no significant effect (p = 0.92). <br>
3. Findings from Hypothesis Testing: <br>
i. Weekday vs. Weekend Demand: Bike rentals are significantly higher on weekdays compared to weekends. <br>
ii. Holiday Effect: Regular days see greater bike rental demand than holidays. <br>
iii. Weather Impact: Rental demand varies significantly across different weather conditions. <br>
iv. Seasonal Variations: Bike rental demand fluctuates based on the season. <br>
v. Weather-Season Dependency: Weather patterns are strongly influenced by the current season. <br>
4. Actionable Recommendations for Yulu <br>
i. Demand Optimization: <br>
a. Dynamic Pricing: <br>
- Increase prices during Fall (high demand) and offer discounts in Spring (low demand). <br>
- Surge pricing during clear weather days (Weather 1). <br>
b. Inventory Management: <br>
- Deploy 20-30% more bikes in Fall and Summer. <br>
- Reduce availability during rainy days (Weather 3/4) to cut maintenance costs. <br>
ii. User Engagement: <br>
a. Convert Casual Users: <br>
- Offer registration discounts during peak hours (e.g., "Register Today, Get 5 Free Rides"). <br>
b. Loyalty Programs: <br>
- Reward frequent riders (e.g., "10 Rides = 1 Free Weekend Pass"). <br>
iii. Operational Efficiency: <br>
a. Weather-Responsive Maintenance: <br>
- Schedule bike repairs during predicted bad weather (low demand periods). <br>
b. Strategic Marketing: <br>
- Target commuters on working days (higher median rentals) with corporate partnerships. <br>
iv. Long-Term Strategies: <br>
a. Expand Weather-Protected Stations: <br>
- Install covered bike docks in areas with frequent rain (based on weather data). <br>
b. Data-Driven Expansion: <br>
- Use spatial analysis to identify high-demand zones (e.g., near metro stations in Fall). <br>
