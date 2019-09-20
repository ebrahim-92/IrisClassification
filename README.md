# IrisClassification
Demonstrate classification with random forests algorithm in python
For this assignment, I decided to use a dataset on iris flowers and the random forest classifier algorithm to classify my chosen dataset. 
I chose to use random forests instead other popular algorithm because it is highly accurate due to the number of decision trees it incorporates into the process.
Also, the random forests algorithm does not suffer from overfitting because it averages out all predictions to remove biases. 
The only issue with random forests is it can be slow in making predictions due to the number of decision trees involved in the process.
	The random forests algorithm also offers a feature selection indicator, scikit-learn. 
  Scikit-learn provides an extra variable with the model, showing the relative importance or contribution of each feature in the prediction.
  It automatically computes the relevance score of each feature in the training phase and then it scales the relevance down so that the sum of all the scores is 1. 
  The score chooses the important features and leaves out insignificant ones for the building of the model.
	Random forests also use gini importance or mean decrease in impurity (MDI for short) to calculate the importance of each feature. 
  Gini importance is also known as the total decrease in node impurity. 
  This is how much the model fit or accuracy decreases when you drop a variable.
  The larger the decrease, the more significant the variable is. Here, the mean decrease is a significant parameter for variable selection.
  The Gini index can describe the overall explanatory power of the variables.
For this assignment, I built a model on the iris flower dataset, which is a very famous classification set. 
It comprises the sepal length, sepal width, petal length, petal width, and the type of flowers. 
There are three species or classes: setosa, versicolor, and virginia. 
The model I built, was made to classify the type of flower. 
The dataset is available in the scikit-learn library or it can be downloaded from the UCI Machine Learning Repository.
The first step in building this model was to import the iris datasets library from scikit-learn and load the iris dataset into my code. 
I then printed the target and feature names to verify the dataset was loaded into my code correctly. 
I then decided to print the first five rows of the dataset, as well as the target variable for the whole dataset, to get an idea on the data I will work with. 
Next, I created a data frame using pandas, followed by splitting the variables.
First, I separated the columns into independent and dependent variables (also known as features and labels). 
Then, I split the dependent and independent variables into a training set and a test set.
After splitting the variables, I trained the model on the training set and performed predictions on the test set.
After the training phase I checked the accuracy of the model using actual and predicted values. 
Thankfully, my model’s accuracy was at 95.55 percent.
Also, in my model I created a random forests classifier to classify my dataset (the whole goal of this project).
In my project, the accuracy could have been increased if I decided to use cross validation to remove low importance features.
I decided not to use cross validation as I had a high accuracy on my model, and it met the requirements needed for this project. 
Hopefully, next time I will actually use cross validation to increase accuracy of the model.
