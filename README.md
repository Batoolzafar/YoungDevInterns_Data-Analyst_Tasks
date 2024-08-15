# YoungDevIntern-Internship
## About the Dataset
The example dataset of seaborn used in this task is the most famous titanic dataset. This dataset is best for analysis as well as creating dashboards and machine learning models. Morever, it is related to one of the most unprecedented events in world history which makes the task even more interesting.
## Task 1: Perform Advanced Data Analysis with Python
### This original dataset contains 15 columns generally but some columns were added just for analysis.
### Most of the column names were changed to make them self explanatory.
### Some repeated columns and duplicate rows in the dataset were removed.
### Many columns were added just for analysis and were removed afterwards.

### Objective:
Throughout the project I went through the following steps:
     1- Manipulating column names
     2- Dropping extra columns
     3- Dropping Duplicates 
     4- Dropping Outlier
     5- Replacing values 
     6- Handling Null Values
     7- Analysis

1- Manipulating column names     
The initial column names were replaced to make them self explanatory. This not only helped me in analysis but will also be helpful to others viewing the project.

2- Dropping extra columns
While analyzing the columns I noticed that some of them were repeated with different values. For example, 
    1- 'Embarked' had the short form of town and 'embark_town' was filled with full town names.
    2- 'Survived' had values 1 and 0, unlike 'survival_status' which was filled with True and False instead.
    3- 'Class' had class numbers written in letters contrary to passenger class filled with integral values.
After munging, the following 12 columns were ready for analysis:
a) passenger_class:  The three classes of people (categories = 1,2,3)
b) gender: (categories = male,female)
c) age: ages of passengers
d) sibling/spouse: number of siblings or spouses with individuals 
e) parent/children: number of parent or children with individuals
f) fare: fare paid to get on board
g) individual_type: categories: (man,woman,child)
h) adult_male: man above 18 (categories = yes,no)
i) deck: Levels of ship, from A on top all the way to G at the bottom (categories = A,B,C,D,E,F,G)
j) embark_town: From where the passengers got on board (categories = Southampton, Cherbourg, Queenstown)
k) survival_status: Alive or dead (categories = True, False)
l) alone: single or with family (categories = True, False)

3- Dropping Duplicates 
Suprisingly, dropping duplicates reduced the data from 891 to 784 rows.

4- Dropping Outlier
While observing the data summary using .describe(), one of the 'fare' column had a fairly large difference between 75 percentile and the maximum value which had the risk of disturbance in analysis. This outlier was removed reducing rows to 781.
  
5- Replacing values 
Values in some colummns were True and False which were replaced with yes and no instead.

6- Handling Null Values
Following columns had the null values:
      1-deck = 581 
      2-age = 106 
      3-embark_town = 2
Though deck has a lot of null values and normally such type of column is removed but it has a really important role in analysis. Furthermore, there are various factors in dataset that can help us determine the deck.
Based on additional information gained, the people on each deck belong to different classes yet they have segregations and different provided facilities.    

Age was easily filled using adult male columns and aggregating ages based on certain criterias.

Two additional columns: fare_range and adult_range were also made to ease the process and were removed after served purpose.
     







 
