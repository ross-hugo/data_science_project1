# data_science_project1
This is a data science project using Jupytr notebooks and pandas to load datasets and combine them together

Industry I selected: Agriculture

Data sets I used: 
- US crop Data
		- World crop prediction on countries and also crops/produce, in which I extracted the US data, because of how large the data set is (could not upload to github because of how large)
    - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_crops_data.csv
- US forest data
	- World forest product data. Again, US forest product was extracted to match the US data above. Because the data sets are so large, I believe that just the US data is sufficient 
  - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_forest_data.csv
- US land data
	- Once again, I have taken out the US data from the world land usage in agriculture
  - https://www.kaggle.com/unitednations/global-food-agriculture-statistics?select=fao_data_land_data.csv

How these combined data sets can be used together:
- To predict how much land usage changes based off of crops grown 
- To extrapolated how the specific crops planted and affect forests and subsequently the forest products
- Make predictions on which crops will be planted next by finding correlations between crops

Clean and Transform:
After going through the data sets, the only columns with null values were the value_footnotes and area. For each seperate data frame, I made each NaN cells within the value_footnotes column the mode of the whole column. The reason for using the mode is because the pieces of data within the value_footnotes column cannot be ordered and they are letters so using the median or the meaan is not viable. Next, The area column had to be filled in the final data frame because of the same reason as the value_footnotes. 
