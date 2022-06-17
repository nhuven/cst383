# Predicting Regional Video Game Sales

## Authors
- Aimen Altaiyeb
- James Meaden
- Josiah Sanchez
- Kevin Daill
- Nathan Huvan

## Introduction
We will predict the sales for a video game in one region based on the sales from the other regions.

## Selection of Data
Video Game Sales with Ratings, downloaded from Kaggle:
https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings
The dataset contains sixteen different feature such as: the name of the game, the platform, and the publisher just to name a few. Our report will focus on the genre and sales features.

## Goal:
To help video game companies determine what location they can expect favorable sales results based on salse data from other regions.

## Features
There are sixteen different features, of the sixteen our report will focus on the following features:
- Genre
- NA_Sales
- EU_Sales
- JP_Sales
- Other_Sales
- Global_Sales

## Methods
### Tools:
- Numpy, Pandas, Matplotlib, scipy.stats, and Seaborn for data analysis and visualization
- sklearn.model_selection, sklearn.preprocessing, and sklearn.neighbors to implement KNN and Linear Regression
- Used Google Colab connected to Git
### Inference methods:
Used KNN and Linear Regression to get the MSE and RMSE to predict sales in Countries

## Results
We were able to predict the sales of video games in one region based on the sales data in another region. One of the best predictions with the lowest RMSE values was the impact the sales in Europe have on the Other region. Testing the KNN Regression model with different values of k had little impact on the RMSE value. (In our report we have provided the default with k =5 and uniform weight along with another with k=9 and distance weight.) If there were more features, an improvement in MSE and RMSE could be achieved.

## Discussion
A lot of the predictions that we found have lots of correlations to one another. One of the comparisons that we can see between each of the different regions. Most notably, when it comes to Europe and North America which share the same interests in terms of genre. Due to these similarities, we can easily determine the North American sales with the Europe sales. However, that does not work vice versa. Instead of being able to determine the Europe sales with North America, we are able to determine this through Other region sales. However, since RPG's tend to dominate the Japanese market and a similar interest here in North America we can predict the Japanese market sales with North America.

## Summary

The most important findings would be the bar plots of the KNN Regression results that show the impact of sales from other regions. One interesting observation is there seems to be a quality factor that contributes to the amount of money a game can bring in. For example, the first pie chart shows Sports with the most number of sales but Platform games bring in the most money as shown in the subsequent pie chart. The support for this is not conclusive because there could have been games where the cost was high and consumers were still willing to pay the price even if the game turned out to be bad. It would be interesting to see a feature added for the number of video games where a refund was given or use the critic score feature. This would do a better job of proving price equals quality.