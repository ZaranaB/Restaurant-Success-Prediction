# Predicting Restaurant Success using Machine Learning

### Overview
The primary objective of this project is to build a restaurant success predictor. The aim to visualize several factors contributing to the popularity of a restaurant while studying the trend across various locations of the city of Bengaluru.

### Objectives  
•	To read and perform data cleaning in the raw data before beginning to train the data set.  
•	To identify any missing values in the target values or in the feature columns and fill with mean values or discard the column from prediction.  
•	To Perform Exploratory Data Analysis (EDA) on the raw dataset to analyze and visualize the fundamental attributes of the provided data set. The data analysis is an integral part to arrive our conclusion of our prediction.  
•	To Separate the Train and Test values based on the valuable features available in the raw dataset before start applying machine learning models to predict our restaurants success.  
•	To perform analysis from the applied learning model and review the best among them and visualize the accuracy.  

Inorder to better understand workings of various ML algorithms I decided to implement the following:
1. Logistic Regression: Logistic regression is an appropriate regression analysis to conduct when the dependent variable is dichotomous, and it is easy and efficient. It is a classification model, which is easy to realize and achieves good performance with based on the feature columns.

2. Random Forest: As it can be used for both classification and regression tasks while providing higher accuracy through cross validation, I chose to use this algorithm. Random forest classifier will handle the missing values and maintain the accuracy of a large proportion of data as the dataset comprises a huge volume of rows for a particular city.

3. Gradient Boosting: It is an iterative algorithm, which minimizes a loss function by recursively choosing a function that points towards the negative gradient or a weak hypothesis. It is a type of machine learning boosting which depends on the intuition that the best possible next model, when combined with prior models, minimizes the overall prediction error. 

4. KNN Classifier: This algorithm is non-parametric where the model structure is determined from the dataset. All the training data used in the testing phase which makes training faster and testing phase slower and costlier in terms of time and memory. In the worst case scenario, KNN could need more time to scan all data points and scanning all data points will require more memory for storing training data.

### Dataset Description

The shape of the dataset is 51717 x 17 and is based on the rating of each online order/dine-in experience  of the customers. The size of the csv file used in this project is 547.48 MB.

#### Data Fields

| Column Name                   | Column Description                                                                                                                        |
|-------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| `url`                         | The URL has the restaurant name and location concatenated to it of the website.                                                           |
| `address`                     | The address of the restaurant.                                                                                                            |
| `name`                        | Name of the restaurant                                                                                                                    |
| `online_order`                | Whether the review is from online order experience based on the flag Yes/No.                                                              |
| `book_table`                  | Whether the review is from dine in experience based on the flag Yes/No.                                                                   |
| `rate`                        | Rating for the order/dine-in experience left by the customer post their experience.                                                       |
| `votes`                       | The no of votes provided from the customer.                                                                                               |
| `phone`                       | The contact number of the restaurant                                                                                                      |
| `location`                    | The location of the restaurant in bangalore location                                                                                      |
| `rest_type`                   | The type of the restaurant that it offers, whether casual dining,quick bites,café & take away etc.                                        |
| `dish_liked`                  | The dishes the customer liked from their experience.                                                                                      |
| `cuisines`                    | The cuisine the restaurant offers for their customers.                                                                                    |
| `approx_cost(for two people)` | The average cost that will incur for people two for each experience.                                                                      |
| `reviews_list`                | The rating and comments provided by the customer on their experience.                                                                     |
| `menu_item`                   | The menu of the restaurant available in the Zomato website.                                                                               |
| `listed_in(type)`             | The type of the customer experience offered by restaurant like Buffet,Café & Takeaways to under if it can accommodate in person customer. |
| `listed_in(city)`             | The city that the restaurant is available.                                                                                                |

#### Data Source:
https://www.kaggle.com/himanshupoddar/zomato-bangalore-restaurants
