# CREDITCARD
Data Science Project for Credit Card Fraud Detection System.

1. Importing Modules
   - pandas is used for data analysis on structured datasets such as CSV files.
   - train_test_split is used for splitting a large data frame into training and testing subsets.
   - RandomForestClassifier is used for creating algorithms for classification tasks.
   - accuracy_score calculates the accuracy of the model created.
     
2. Basic Dataset Functions
   - The dataset is loaded into the 'dataset' data frame using the read_csv function.
   - .head() function helps to get the 1st 5 rows of the data frame.
   - The .info() function helps you to get the summary of the entire data frame including names of columns, number of null values, memory usage etc.
   - The .shape() function helps you to get the number of rows and columns in the data frame.
   -   The count of empty values are then calculated.

3. PREPARING DATA FOR TRAINING
   - We first create a new data frame named 'X' by dropping the 'Class' column.
   - We then assign the 'Class' columns to another data frame named 'Y'.
   - Then we split the dataset into training and testing subsets with 20% of the dataset for training and 80% for testing.
     
4. Training and Evaluating
   - We train a model using Random Forest Classifier algorithm and fit the training datasets into it.
   - We then create a prediction variable to predict the model.
   - The accuracy score is calculated by using the testing subsets.
     
5. MANUAL TESTING
   - We create a function which takes time and amount as the input. The dataset is loaded first into a data frame named 'data'.
   - We then calculate the closest transaction in the dataset which matches the values entered by the user.
   - We then fetch the row corresponding to this transaction and check if the 'Class' columns value is 1 or not.
   - If it matches 1, the function prints 'Fraud Case' else otherwise.
