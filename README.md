# Motivation

Rather than buying physical cookbooks, many aspiring cooks and bakers are turing to websites such as Pinterest and food.com for recipes to try. Similar to many patrons and researchers, I am attracted to recipes with high ratings and trendy or health conscious ingredients. However, how reliable are the ratings from the general population? I sought to look into answering the following questions: 

  1. Are the distribution of ratings for recipes based on their category consistent?
  2. Overtime, does the prevalence for certain 'health' foods increase? 
  3. 

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

![ViolinPlot](https://user-images.githubusercontent.com/111457464/225732871-300f29d7-cba3-4db9-9d51-2cefcbbd1c90.png)

Each category has a similar distribution with a mean between 4.6 and 4.7 stars and a median of 5.0. This indicates that the category of recipe has little impact on how it is rated. The highly skewed distributions also indicate that the recipe ratings have little meaning as half of rated recipes have a rating of 5 stars. While it might be difficult to discern the best recipes based on their rating, less favorable recipes are easily identified with ratings of 4 or below since 4.5 and 5 stars appear to be cheap. 


![Trendy](https://user-images.githubusercontent.com/111457464/225747984-442dbd0f-0b14-4865-8ed3-90ca0ae3d603.png)
