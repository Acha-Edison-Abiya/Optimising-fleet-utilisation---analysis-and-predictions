# Optimizing-fleet-utilization---analysis-and-predictions of utilization rate
Analyse the utilisation of fleet vehicles to identify underused assets and make data-driven recommendations for optimising the fleet size and composition, improving efficiency, safety and cost-effectiveness. 
# Objectives

The main objective of this project is to optimize the fleet size and composition for the City of Toronto by identifying underutilized and overutilized vehicles. The project aims to answer the following key 
## questions:

- Which vehicles are underutilized or overutilized?
- How does utilization vary across departments and times of the year?
- What is the optimal number and type of vehicles needed to meet demand?
- How do depreciation and lifecycle status impact vehicle utilization rates and maintenance costs?
- Perform clustering analysis to identify patterns in vehicle usage and maintenance to optimize fleet management?
- Predict vehicle utilization rates using key operational and maintenance variables?
- # Methodology

The analysis focused on identifying the utilization rate of vehicles and comparing them within the same type to detect outliers. A balanced approach to fleet management was recommended, with emphasis on matching vehicle types to departmental needs and adjusting for seasonal demand.

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

