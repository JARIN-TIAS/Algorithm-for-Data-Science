# Algorithm-for-Data-Science  (some changes in ths data)


1. #from google.colab import drive
path=('/content/data.csv')

2. #to drop column from data frame
X = df.drop('income', axis=1)
Why axis=1?
In this context, axis=1 is used because you want to remove a column (i.e., 'income') from the DataFrame df. Columns are handled with axis=1, while rows would be handled with axis=0.

3. # If I want to drop  multiple colum # Drop multiple columns
columns_to_drop = ['education', 'city']
X = df.drop(columns=columns_to_drop)


4. # get.dummies(X['column_name']).head(10)
pd.get_dummies: This is a function in pandas that converts categorical variables into dummy/indicator variables. This process is also known as one-hot encoding.
