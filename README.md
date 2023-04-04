# Motivation

Rather than buying physical cookbooks, many aspiring cooks and bakers are turing to websites such as Pinterest and food.com for recipes to try. Similar to many patrons and researchers, I am attracted to recipes with high ratings and trendy or health conscious ingredients. However, how reliable are the ratings from the general population? I sought to look into answering the following questions: 

  1. Are the distribution of ratings for recipes based on their category consistent? For instance, bread can be difficult and time consuming to make so will bread type recipes have lower ratings? 
  2. Overtime, does the prevalence for certain 'health' foods increase? 
  

________________________________________________________

# Data

The dataset was downloded from Kaggle: https://www.kaggle.com/datasets/irkaal/foodcom-recipes-and-reviews

________________________________________________________

# Methodology

Python was used to load the data into Pandas dataframes. Matplotlib and Seaborn were used to create visualizations for analysis. 

The recipe categories in the dataset were numerous and inconsistent, so the recipes were sorted into six main categories for analysis: desserts, bread, breakfast/brunch, quick, healthy, and holidays. Any recipes that did not fit these categories were not considered. 

Regex was used to identify recipes with trendy and health conscious ingredients such as cauliflower, quinoa, and coconut. 

________________________________________________________

# Analysis
## Overall Rating Distribution

![OverallDistribution](https://user-images.githubusercontent.com/111457464/229893983-b8a4a355-679f-4e01-a8f0-87a33990b30f.png)

* The mean rating is 4.63 with a standard deviation of 0.64. The median is 5.00. The distibution of ratings is highly skewed in favor of a high rating. The count of recipes at each rating was scaled using the Square Root Function in order to better visualize the distribution. 

## Rating Distribution by Category

![ViolinPlot](https://user-images.githubusercontent.com/111457464/225732871-300f29d7-cba3-4db9-9d51-2cefcbbd1c90.png)

* Each category has a similar distribution with a mean between 4.6 and 4.7 stars and a median of 5.0. This indicates that the category of recipe has little impact on how it is rated. This was contrary to my hypothesis that bread recipes may have lower mean ratings due to the difficulty and time they can take. 

* The highly skewed distributions also indicate that the recipe ratings have little meaning as half of rated recipes have a rating of 5 stars. While it might be difficult to discern the best recipes based on their rating, less favorable recipes are easily identified with ratings of 4 or below since 4.5 and 5 stars appear to be cheap. 

## Trendy Ingredients Over Time

![Trendy](https://user-images.githubusercontent.com/111457464/229894457-8f9b2e9e-f842-4471-8844-592455d2eb10.png)

* Quinoa, coconut, and cauliflower were chosen as trendy ingredients as they are popular substitutes for bread and rice, other oils and milks, and potatoes, respectively. The percentage of recipes that contain the ingredients rather than the raw number of recipes with the ingredients was used because the number of recipes loaded to Food.com was inconsistent. 

* The prevalence of all three "trendy" ingredients have increased over time indicating that recipe producers began catering to an audience looking for healthy options as time went on. Coconut has the greatest popularity which could be due to its versability as a milk, oil, sweetener, and flour. There is a clear decrease in all three ingredients after 2019 which is likely due to the decreased number of recipes availble for the year 2020. 
