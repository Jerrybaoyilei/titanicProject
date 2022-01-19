# titanicProject
My attempt on the titanic survival data analysis, using Machine Learning to predict the survival of passengers.

Data is downloaded from Kaggle. 

1. Ploted survival against different features, including embarked location, number of parent/children, number of siblings/spouses, etc. 
2. Dealt with null values
  2.1 Filled cabin null values with a string 
  2.2 Presumed the missing embarked location is Soutampton because most passengered embarked from there
  2.3 Used average ticket fare to full in missing fare values
3. Feature engineering, including dividing titles into 6 categories, creating ticket number groups
4. Predicted missing ages using other highly correlated variables
5. Explored peer effects by dividing peopel with same surname into 2 groups: survived male that are older than 12 years old, and women and children under 12 that didn't survive. Then, modify the group features to make sure they have a higher probabiility of being predicted as survived/not survived
6. Built different machine learning models, compared performance, and made the final prediction using the trained model on the test data
