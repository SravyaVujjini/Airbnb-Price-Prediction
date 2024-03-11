# Beyond the Hotel: A Deep Dive into Airbnb in Asheville, NC

This project focuses on understanding the details of Airbnb listings through the exploration of two core questions:

1. What would be the average price of an Airbnb listing based on its location, size, and the availability time of the year? How do these pricings vary with respect to the factors considered?
2. What factors contribute most to the guest’s perceived value of a listing – Review Score?

The primary objective is to determine the average price of Airbnb listings based on the considered factors, aiming to empower both hosts and guests with valuable insights that seek to facilitate more informed decisions during the listing and booking processes. By delving into the key factors influencing the pricing of Airbnb listings, we aim to provide hosts with actionable insights to optimize their offerings.

## Data Source
Our dataset, acquired from Inside Airbnb (http://insideairbnb.com/get-the-data/), is titled “Airbnb Listings in Asheville, NC”. 

## Data Cleaning and Exploration

- In our data cleaning and exploration process, we narrowed our focus to specific variables relevant for our research questions.
- We addressed missing values by imputing the median to maintain the central tendency of the data. Additionally, we extracted numeric values and converted categorical variables to numeric format.
- During the analysis of distribution of prices, we observed a rightward skewness, indicating a concentration of listings at the lower end. To address this, we applied a log transformation on the Airbnb listing prices, aiming to mitigate the influence of extreme values and achieve a distribution closer to normal.

 ![image](https://github.com/SravyaVujjini/Airbnb-Price-Prediction/assets/121740546/c6e3cf48-0ad1-422b-b6e2-88c38d763366)

## Modeling

- We have modeled our data with a simple linear regression model , a generalized linear model (GLM), a robust linear model and a random forest model.
- The Random Forest Regressor operates by constructing a multitude of decision trees during training and outputs the mean prediction of the individual trees for regression tasks.
- It excels in handling complex relationships within data, reducing overrfitting, and
providing robust predictions by aggregating the outputs of multiple decision trees




## Results

- The model explained 60.62% of the variance in the pricing data, approximately 57.08% of the variance in the weighted review scores.

![image](https://github.com/SravyaVujjini/Airbnb-Price-Prediction/assets/121740546/84d1cf59-a866-4220-9e9d-f30a13d00291)

![image](https://github.com/SravyaVujjini/Airbnb-Price-Prediction/assets/121740546/49d9f2d8-fbfe-4dbf-9411-f63d05628fde)

- Cleanliness and check-in experience turned out to be the most influential factors of positive guest experience. This finding is in line with the hospitality industry standards emphasizing first impressions and core amenities.


![image](https://github.com/SravyaVujjini/Airbnb-Price-Prediction/assets/121740546/9b12ac0a-fe70-422f-b74d-c5987efd8af1)


