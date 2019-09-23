# ML_workshop_sept_23
#  Step 1:
* Installing the Dependencies for getting start
#  Step 2:
* Download the dataset from the Github Repository and Load .
#  Step 3:
* Perform the Exploratory Data Analysis.
#  Step 4:
* Perform Transformation over the data
In this step we are transforming the Date field in the dataset from string to datetime format so that we can use the date functions and find out the difference in 2 dates in number of days.
#  Step 5:
* Applying Feature Engineering
This step involves creating new features from the existing dataset and using those features to segment the users.There are very common and useful segmentation methods. We are going to implement one of them to our business: RFM.
RFM stands for Recency - Frequency - Monetary Value. Theoretically we will have segments like below:
* Low Value: Customers who are less active than others, not very frequent buyer/visitor and generates very low - zero - maybe negative revenue.
* Mid Value: In the middle of everything. Often using our platform (but not as much as our High Values), fairly frequent and generates moderate revenue.
High Value: The group we don’t want to lose. High Revenue, Frequency and low Inactivity.

# Recency:
* To calculate recency, we need to find out most recent purchase date of each customer and see how many days they are inactive for. After having no. of inactive days for each customer, we will apply K-means* clustering to assign customers a recency score

# Frequency:
* To create frequency clusters, we need to find total number orders for each customer. First calculate this and see how frequency look like in our customer database.

# Revenue:
* To create revenue clusters, we will calculate revenue from unit price and quantity of the product. We will calculate revenue for each customer, plot a histogram and apply the same clustering method.

#  Step 6:
* Applying Various Machine Learning Models
For this particular problem, we want to use the model which gives the highest accuracy. Let’s split train and test tests and measure the accuracy of different models.

# Step 7:
* Correlation Matrix
# Step 8:
* Applying Multi-Classification Model

From this result, we see that Naive Bayes is the best performing one (~64% accuracy). But before that, let’s look at what we did exactly. We applied a fundamental concept in Machine Learning, which is Cross Validation.

Cross Validation is a way of measuring this. It provides the score of the model by selecting different test sets. If the deviation is low, it means the model is stable

