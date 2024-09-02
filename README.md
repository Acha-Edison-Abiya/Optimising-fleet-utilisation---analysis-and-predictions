# Optimizing-fleet-utilization---analysis-and-predictions of utilization rate
# Objectives
The objective of this project was to optimize the City of Toronto’s fleet management by addressing critical questions related to vehicle utilization and maintenance. The project aims to the following:
## key questions & Objectives 
- Identify underutilized and overutilized vehicles to ensure efficient fleet usage - (Which vehicles are underutilized or overutilized?
- Analyze how vehicle utilization varies across different departments and times of the year to better allocate resources. 
- Determine the optimal number and type of vehicles needed to meet current and future demand. 
- Examine the impact of depreciation and lifecycle status on vehicle utilization rates and maintenance costs to inform replacement and maintenance strategies.- Perform clustering analysis to uncover patterns in vehicle usage and maintenance, enabling data-driven decisions for fleet optimization.
- Develop a predictive model to forecast vehicle utilization rates using key operational and maintenance variables, helping to preemptively manage fleet efficiency.
# Methodology
###### Data Collection and Preprocessing:
Gathered and cleaned data on vehicle characteristics, usage, maintenance costs, and lifecycle status.
Standardized and prepared the dataset for analysis, ensuring accuracy and consistency.
###### Utilization Analysis:
Calculated utilization rates to identify underutilized and overutilized vehicles.
Analyzed utilization patterns across different departments and throughout the year to understand variations and peak demand periods.
###### Depreciation and Lifecycle Analysis:
Investigated the relationship between depreciation, lifecycle status, and their impact on utilization rates and maintenance costs.
Assessed how vehicles in different lifecycle stages (e.g., “In Service,” “End of Life”) were used and maintained.
###### Clustering Analysis:
Applied K-means clustering to group vehicles based on usage patterns, maintenance costs, and other key variables.
Identified distinct clusters to better understand vehicle performance and to guide fleet optimization strategies.
##### Regression Analysis:
Developed a regression model to predict vehicle utilization rates based on operational and maintenance variables.
Used the model to forecast potential underutilization or overutilization, aiding in future fleet planning.
##### Recommendations:
Based on the findings from the analyses, provided actionable recommendations for optimizing fleet size, composition, and resource allocation.
## Dataset
The simulated dataset contains 1500 records of information related to fleet assets used by the City of Toronto. The main objective of this dataset is to analyze vehicle utilization and optimize fleet size and composition. The dataset includes various attributes that describe the vehicles' characteristics, usage, and associated costs.
Dataset Columns 
- Asset_ID: A unique identifier for each vehicle or piece of equipment in the fleet.
- Asset_Type: The type of asset, such as Heavy Vehicle, Light Vehicle, or Special Equipment.
- Purchase_Date: The date on which the asset was purchased. This can help in analyzing the age of the asset and its lifecycle stage.
- Lifecycle_Status: The current lifecycle status of the asset, e.g., In Service, End of Life. This indicates whether the asset is still in use or has   been decommissioned.
- Maintenance_Costs: The total cost incurred for maintaining the asset over its lifetime.
- Replacement_Cost:The estimated cost to replace the asset with a new one. This is useful for financial planning and decision-making.
- Depreciation_Value: The depreciation value of the asset, representing how much value it has lost over time.
- Fuel_Type: The type of fuel the asset uses, such as Gasoline or Electric. This can impact both costs and environmental considerations.
- Fuel_Efficiency: The efficiency of the asset's fuel consumption, typically measured in kilometers per liter or miles per gallon.
- Mileage: The total distance traveled by the asset, usually measured in kilometers. This is a key indicator of vehicle usage.
- Hours_in_Use: The total hours the asset has been in use. This metric helps assess the intensity of use beyond just distance traveled.
- Department: The department to which the asset is assigned, such as Public Works, Transportation, or Emergency Services. This helps in analyzing usage patterns across different city departments.
- Trips_per_Year:The number of trips the asset makes per year. This is another key indicator of how frequently the vehicle is being used.
# Key Results
## Which vehicles are underutilized or overutilized?
- Overutilized Vehicles: Heavy vehicles exhibited higher utilization rates, indicating they are frequently in demand and may require fleet expansion to meet operational needs.
- Underutilized Vehicles: Light vehicles and special equipment showed lower utilization rates, suggesting that these assets are underutilized and could be considered for downsizing or repurposing.
- Outliers: Vehicles with utilization rates significantly above or below the average for their type were identified as outliers, warranting closer inspection for potential reallocation or adjustment in fleet size.
![image](https://github.com/user-attachments/assets/840f9166-baa2-4621-914a-43696eaa9a8a)


## How does utilization vary across departments?
- High Utilization Departments: Departments such as Emergency Services and Public Works showed consistently higher vehicle utilization rates, reflecting their critical and frequent operational demands.
- Moderate to Low Utilization Departments: Departments like Administrative Services and Parks & Recreation had lower vehicle utilization rates, indicating that their fleet may be larger than necessary for their needs.
- Seasonal Variations: Utilization rates also varied seasonally, with certain departments experiencing peak demand during specific times of the year, such as increased Parks & Recreation vehicle use during summer.
![image](https://github.com/user-attachments/assets/9e3c9c38-fe85-461f-af80-a1b26854172b)


## What is the optimal number and type of vehicles needed to meet demand?
- Heavy Vehicles: Given their high utilization rates, especially in departments like Emergency Services and Public Works, an increase in the number of heavy vehicles is recommended to meet the consistent and high demand.
- Light Vehicles: These vehicles showed moderate utilization. The current fleet size for light vehicles appears adequate, but minor adjustments could be made based on specific departmental needs and usage patterns.
- Special Equipment: Due to lower utilization rates, the fleet size for special equipment could be reduced or reallocated to departments where they might be more needed, optimizing the overall fleet composition.
- Balanced Fleet Strategy: A dynamic approach is recommended, adjusting the fleet composition seasonally and based on real-time demand. This ensures that each department has the right type and number of vehicles throughout the year.

## How do depreciation and lifecycle status impact vehicle utilization rates and maintenance costs?
- Depreciation vs. Utilization Rate: Vehicles with higher depreciation tend to have lower utilization rates, indicating that older or more depreciated vehicles are used less frequently compared to newer ones.
- Depreciation vs. Maintenance Costs: As vehicles depreciate, maintenance costs generally increase. This suggests that older, more depreciated vehicles are more costly to maintain, which may contribute to their lower utilization.
- Lifecycle Status vs. Utilization Rate: Vehicles in the “In Service” stage have higher utilization rates, while those categorized as “End of Life” or “Maintenance” exhibit significantly lower usage, reflecting their limited availability and operational capacity.
- Lifecycle Status vs. Maintenance Costs: Vehicles nearing the “End of Life” stage or frequently in “Maintenance” incur higher maintenance costs, reinforcing the need to consider lifecycle status when planning fleet maintenance and replacement strategies.
![image](https://github.com/user-attachments/assets/c0e2b5aa-0e76-4fc5-9f0a-6876922184b1)

## Perform clustering analysis to identify patterns in vehicle usage and maintenance to optimize fleet management?###### Cluster Identification:
- Cluster 0 (Red): Represents vehicles with lower mileage, lower maintenance costs, and lower utilization rates. These vehicles are likely newer or less used, indicating potential underutilization.
- Cluster 1 (Blue): Contains vehicles with higher mileage, higher maintenance costs, and higher depreciation values, reflecting older and more heavily used vehicles. These vehicles also show higher utilization rates.
- Cluster 2 (Green): Consists of vehicles with moderate values across mileage, maintenance costs, and utilization rates, suggesting a balanced usage pattern.
###### Utilization Patterns:
- Vehicles in Cluster 1 have the highest utilization rates, which aligns with their higher mileage and older status.
- Cluster 0 shows the lowest utilization rates, pointing to possible underutilization of newer or less active vehicles.
- Cluster 2 demonstrates moderate utilization, indicative of balanced fleet usage.
###### Maintenance and Depreciation Insights:
- Cluster 1 vehicles, with higher maintenance costs and depreciation values, highlight the increased costs associated with older, heavily used vehicles.
- The lower maintenance costs in Cluster 0 correlate with newer or less utilized vehicles, which may require less frequent servicing.
###### Recommend Action:
- The analysis suggests a need to further evaluate underutilized vehicles in Cluster 0 for potential reallocation or downsizing.
- Vehicles in Cluster 1 may require close monitoring for maintenance and potential replacement due to their high usage and associated costs.
- Cluster 2 vehicles appear to be optimally used, but periodic reviews are recommended to maintain balanced utilization.
  ![image](https://github.com/user-attachments/assets/75f0e935-f0d7-45c0-9e2c-0ea21fe15c90)
  
## Predict vehicle utilization rates using key operational and maintenance variables?
###### Significant Predictors:
- Mileage: A strong positive correlation was observed between mileage and utilization rate, indicating that vehicles with higher mileage are generally more utilized.
- Maintenance Costs: Higher maintenance costs were also positively associated with higher utilization rates, suggesting that vehicles requiring more upkeep are often those in frequent use.
- Depreciation Value: Depreciation value showed a moderate correlation with utilization, where older vehicles with higher depreciation tend to have varied utilization patterns.
##### Model Performance:
- The regression model was able to explain a significant portion of the variance in utilization rates, indicating that the selected variables are effective predictors.
- However, the model also highlighted some limitations, particularly in capturing extreme cases of underutilization or overutilization, suggesting that additional factors or more complex models might be needed for better accuracy.
#### Practical Implications:
- The model can be used to predict which vehicles are likely to become underutilized or overutilized, allowing fleet managers to proactively address potential inefficiencies.
- By understanding the key drivers of utilization, the city can optimize vehicle assignments and maintenance schedules to ensure a balanced and cost-effective fleet.

## Conclusion
The comprehensive analysis conducted in this project has provided valuable insights into the City of Toronto’s fleet management. By identifying underutilized and overutilized vehicles, we’ve highlighted areas where resource allocation can be optimized, ensuring that every vehicle is used to its fullest potential. The examination of utilization across departments and seasonal variations revealed the need for dynamic fleet management strategies that respond to changing operational demands.

Our exploration of depreciation and lifecycle status underscored the importance of timely vehicle replacement and maintenance to minimize costs and maintain high utilization rates. Clustering analysis further refined our understanding of vehicle usage patterns, enabling more targeted decisions regarding fleet composition and management. Finally, the regression model developed in this project offers a predictive tool that can anticipate future utilization rates, allowing for proactive adjustments to fleet operations.
