Titanic Survival Prediction Pipeline
Predicting Survival on the Titanic
History
The sinking of the Titanic is one of the most infamous disasters in history. After colliding with an iceberg on April 14, 1912, the Titanic tragically sank, leading to the death of 1502 out of the 2224 people on board. The loss of life was profound, yet by analyzing the patterns and attributes of those on board, we can make reasonably accurate predictions about which passengers were more likely to survive. Factors such as gender, age, and social status played significant roles in determining survival rates, revealing societal priorities and privileges of the time. Women, children, and the upper class were disproportionately more likely to survive.

Goals
The main objective of this project is to build a Machine Learning pipeline that processes the Titanic dataset, engineers relevant features, and predicts which passengers are most likely to survive. This project provides an opportunity to explore key machine learning concepts and gain insights from historical data.

Project Outline
Prepare the Dataset
The Titanic dataset includes information on various passenger characteristics, such as:

PassengerId: Unique ID for each passenger.
Survived: Target variable (0 = Did not survive, 1 = Survived).
Pclass: Passenger class (1 = Upper, 2 = Middle, 3 = Lower).
Name, Sex, Age: Personal details.
SibSp, Parch: Family relationships on board.
Ticket, Fare: Ticket details.
Cabin: Cabin number (if known).
Embarked: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).
Before building the prediction model, we need to prepare and clean the dataset by handling missing values, converting categorical variables, and engineering new features.

Configuration
Ensure you have Python installed, along with necessary packages:

pandas
scikit-learn
numpy

Separate Data into Train and Test Sets
The data is split into training and test sets, where the training set will be used to train the model, and the test set will be used to evaluate its performance:

Preprocessing Steps
Several preprocessing steps are performed to clean and prepare the data for modeling:

Handling missing data (e.g., filling missing Age, Cabin values).
Encoding categorical variables (Sex, Embarked).
Scaling continuous features (e.g., Fare, Age).
Class to Extract the Letter from Cabin Variable
A custom class is created to extract the letter portion of the Cabin variable, as it provides valuable information:

Pipeline
A machine learning pipeline is constructed to streamline the process of data preprocessing and model training:

Make Predictions and Evaluate Model Performance
After building the model, predictions are made on the test data and the model's performance is evaluated:

Conclusion
This project demonstrates how machine learning can be used to predict survival on the Titanic by analyzing key passenger attributes. The pipeline processes raw data, applies feature engineering, trains a model, and evaluates its performance, providing insights into survival probabilities.
