# data_science_project1
This is a data science project using Jupytr notebooks and pandas to load datasets and combine them together

Industry I selected: Agriculture

Data sets I used: 
- US crop Data
    - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_crops_data.csv
- US forest data
  - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_forest_data.csv
- US land data
  - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_land_data.csv

How these combined data sets can be used together:
- To predict how much land usage changes based off of crops grown 
- To extrapolated how the specific crops planted and affect forests
- Make predictions on which crops will be planted next by finding correlations between crops

Clean and Transform:
After going through the data sets, the only columns with null values were the value_footnotes and area. For each seperate data frame, I made each NaN cells within the value_footnotes column the mode of the whole column. The reason for using the mode is because the pieces of data within the value_footnotes column cannot be ordered and they are letters so using the median or the meaan is not viable. Next, The area column had to be filled in the final data frame because of the same reason as the value_footnotes. 
