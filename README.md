# Playstore-Dataset
# Problem Statement:
The Google Play Store is the largest app market in the world. It generates more than double the downloads of the Apple App Store but makes only half the money as the Apple Store. Explore and analyze the data to discover the key factors responsible for app engagement and success.

# Objective:
The objective of this project is to deliver insights to understand customer demands better and thus help developers to popularize the product.
# Data set used:
Play_store_df
User_review_df
Merged_df (resultant of above two df after merging them)

Scientific Computing tool & Data manipulation:

Numpy
Pandas
  
Visualization libraries used:
Matplotlib
Seaborn
Plotly

# Steps involved:
# Loading the dataset
We created a directorial path for the play store dataset, using the Pandas read function we read it. It has a shape (10841,13) which means it has 10841-row labels and 13 features or column labels.After reading it we found which are the dependent variables and which are the independent variables, there is one dependent variable which is the number of installs or just installs, others are independent variables.

# Cleaning and Transforming Data
Cleaning is the process of removing undesired features, values, or any suffix, prefix, or anything which can produce an exception. Transforming is completely a different process, transforming is required to ensure the consistent data type of features because inconsistent data type will generate an obstacle during the execution of the program. These two processes have specific subprocesses as follows.



# Unwanted Data Removal
In this step we ensured to make a data type of feature consistent by removing characteristics from the values of features, to make them usable. Our data set has features installs which store the number of installs as per categories, but it has a (+) sign added at the end of its values, therefore we removed that plus sign. Feature size contains values regarding the application size, it has Mb and k as a suffix in its values, that’s why it is needed to replace k with k/1000, remove MB and k.
Feature reviews have the values of the number of reviews for each category, it is coming with some unwanted characteristics with its values, hence we removed. The last update is a feature that stores the date of the last update for each application of each category. But it was given as an object we feed to pandas to the Date Time method and there we go; we have successfully converted it into a Date Time object.

# Null values Treatment
Two features of our data set have many null values, the first one is size and the second one is rating feature, so we filled null values with a mean, median, and mode because we can assume that the size of the application could be an average of sizes available for a particular category and talking about rating, we have taken the median of rating for each category, and then we filled Nan with a mode for categorical data.

# Number of installations

From the below plot highest installs of the apps are crossing a Million and then 10 Million, very few apps are crossing the 500M and dream install 1B. Some apps like Instagram, YouTube, Facebook, WhatsApp, etc. are crossing the dream install 1B.





![newplot (3)](https://user-images.githubusercontent.com/78207836/143770263-a50e6738-6e64-4472-aedf-3b6814bf9cd6.png)


# Free vs Paid 

Here we can see that 92.6% of apps are free and 7.38% of apps are paid on Google Play Store, so we can say that most of the apps are free on Google Play Store. 

![download (10)](https://user-images.githubusercontent.com/78207836/143770402-6416b1d3-9a19-4acc-ab58-6e1312d78138.png)


# Updated Apps

In the below plot, we plotted the apps updated or added over the years comparing Free vs. Paid, by observing this plot we can conclude that before 2011 there were no paid apps, but with the years passing free apps has been added more in comparison to paid apps, By comparing the apps updated or added in the year 2011 and 2018 free apps are increases from 80% to 96% and paid apps are goes from20%to4%. So we can conclude that most of the people are after free apps.

![download (1)](https://user-images.githubusercontent.com/78207836/143770957-e6c2ae85-39c2-4cd1-a288-0631884c73b5.png)


# Conclusion:

As per our EDA, an ideal application on the google play store should obey the following properties/characteristics
1. Category Type: Before 2011 there were no paid apps, but with the years passing free apps has been added more in comparison to paid apps, By comparing the apps updated or added in the year 2011 and 2018 free apps are increased from 80%% to 96% and paid apps are gone from 20% to 4%. So, we can conclude that most people are after free apps.
2. Installs vs Rating: Some Semi-popular apps are crossing a Million and then 10 Million, and only a few apps are able to go beyond the 500M and 1B mark. Popular apps under the Social media category like Facebook, WhatsApp, Instagram have more than 1B installations.
3. Rating vs Installs vs Type: Free apps are preferred over paid apps and the ratings are in the range of 4 to 5. Therefore the free Apps are most downloaded as compared to paid apps, Hence Developers should focus more on free apps. Users prefer more free apps. Most of the apps present in the play store are more or less of the same size so size doesn’t affect their decision much.
 4. The most installed category: As we have explored applications belonging to the category gaming and followed by communication are being installed the most, this is the clue to choose the category.
 5. User Reviews: User Reviews often contain valuable feedback and suggestions for improving the app. Analyzing the top trends and issues for the app enables us to assess which parts of the app or game to focus on. It also shows where to invest in the business to improve the offering and create a more successful app or game.
 6. Ratings: App rating is a reflection of how users respond to the app. Learn what affects rating and what we can do to influence it.



