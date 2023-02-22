# Machine-Learning---01
Prediction using Decision Tree Classifier

1.Introduction
Decision trees are one of many supervised learning algorithms available to anyone looking to make predictions of future events based on some historical data and, although there is no one generic tool optimal for all problems, decision trees are hugely popular and turn out to be very effective in many machine learning applications. Decision tree uses the tree representation to solve the problem in which each leaf node corresponds to a class label and attributes are represented on the internal node of the tree. We can represent any Boolean function on discrete attributes using the decision tree.

2.	Data Exploration: 
Let’s explore the dataset. It shows which users have purchased an Iphone. Our objective in this project is to predict if the customer will purchase an Iphone or not given their gender, age and salary. The sample rows are shown below. The column Gender is alphanumeric which is converted to numeric values. The columns “Gender”, “Age”, “Salary” are selected as features and the column “Purchase Iphone” is selected as a target.

![image](https://user-images.githubusercontent.com/21077069/220509378-91ff25c4-aabf-44ca-aabf-15d2ce27c2b9.png)

3. Load the dataset
We will assign the three independent variables “Gender”, “Age”, “Salary” to X. 
The dependent variable that we need to predict – “Purchased iPhone” will be assigned to y.

4. Convert Gender to Number
The classification algorithm in sklearn library cannot handle the categorical (text) data. In our data, we have the Gender variable which we have to convert to numerical format. 
We will use the class LabelEncoder to convert text data of Gender variable to number.

5. Split the data into training and test set
We will use the train_test split method to split our data into training and testing set. We will use 25% data for testing purpose.

The train-test split is a technique for evaluating the performance of a machine learning algorithm. It can be used for classification or regression problems and can be used for any supervised learning algorithm. The procedure involves taking a dataset and dividing it into two subsets. The first subset is used to fit the model and is referred to as the training dataset. The second subset is not used to train the model; instead, the input element of the dataset is provided to the model, then predictions are made and compared to the expected values. This second dataset is referred to as the test dataset. Train Dataset: Used to fit the machine learning model. Test Dataset: Used to evaluate the fit machine learning model. The objective is to estimate the performance of the machine learning model on new data: data not used to train the model.

6. Feature Scaling and Fit the Classifier
We will be using the DecisionTreeClassifier from the sklearn.tree library. When we create the object of DecisionTreeClassifier, we will set the criterion parameter as entropy.

7. Make Predictions
Now that we have trained the model, let’s make some predictions using the test dataset. 
