# Project 1: Titanic

This week in class we went over some basic statistics, learned some Python programming concepts, and also learned how to navigate files, packages, and libraries using the command line. Great start! At this point you should be chomping at the bit to do some Data Science. If so, good - because it's time for Project 1!

For our first project, we're going to take a look at the Titanic manifest. We'll be exploring this data to see what we can learn using the mad skills covered in class.

## Prework
Fork and clone this repo. At the end of this project, you'll submit a pull request containing an iPython notebook that answers the questions below.

## Step 1: Reading the data

1. Go to [https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data) and download the "train.csv"
2. If you scroll down the page a bit, you should see a data dictionary explaining each of the columns. Take a minute to familiarize yourself with how the csv is structured.
3. Create an iPython notebook and load the csv into pandas.

## Step 2: Cleaning the data
1. What column has the most missing data? How many cells in that column are empty?
2. What column has the second most missing data? How many cells in that column are empty?
3. Delete all rows where 'Embarked' is empty
4. Fill all empty cabins with **¯\\_(ツ)_/¯**

## Step 3: Feature extraction
1.  We have two columns that deal with family: `SibSp` and `Parch`. Create a new column called `FamilyCount` which will be the sum of `SibSp` and `Parch`. For example, if I have 2 `SibSp` and 1 `Parch` then `FamilyCount` should be 3.
2. Reverends have a special title in their name. Create a column called `IsReverend`: 1 if they're a reverend, 0 if they're not.

## Step 4: Exploratory analysis
1. What `percentage` of people survived? (Hint: take the mean of the 'Survived' column)
2. What gender fared the worst? What was their survival rate?
3. What was the survival rate for each 'Pclass'?
4. Did any reverends survive?
5. What is the survival rate for IDK cabins ("¯\\_(ツ)_/¯")
6. What is the survival rate for people whose `Age` is empty?
7. What is the survival rate for each port of embarkation?
8. What is the survival rate for children (under 12) in each `Pclass`?
9. Did the captain of the ship survive? Is he on the list?
10. Of all the people that died, who had the most expensive ticket? How much did it cost?

Bonus: Using the data, come up with the most interesting finding (e.g. All kids under the age of 3 survived). Winner gets a prize!

## Step 5: Plotting
1. Create a pairplot in seaborn, using `Survived` as the hue
2. Create a heatmap showing how each feature/label correlates with one another
3. Create a box and whisker plot to learn more about `Age`
4. Create a histogram of ticket prices

Bonus: For each `Pclass`, create a violin plot for `Age`
