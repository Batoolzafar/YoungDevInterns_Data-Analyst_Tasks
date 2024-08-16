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
<ul><li>passenger_class:  The three classes of people (categories = 1,2,3)</li>
     <li>gender: (categories = male,female)</li>
     <li>age: ages of passengers</li>
     <li>sibling/spouse: number of siblings or spouses with individuals</li>
     <li>parent/children: number of parent or children with individuals</li>
     <li>fare: fare paid to get on board</li>
     <li>individual_type: categories: (man,woman,child)</li>
     <li>adult_male: man above 18 (categories = yes,no)</li>
     <li>deck: Levels of ship, from A on top all the way to G at the bottom (categories = A,B,C,D,E,F,G)</li>
     <li>embark_town: From where the passengers got on board (categories = Southampton, Cherbourg, Queenstown)</li>
     <li>survival_status: Alive or dead (categories = True, False)</li>
     <li>alone: single or with family (categories = True, False)</li>
</ul>

3- Dropping Duplicates 
Suprisingly, dropping duplicates reduced the data from 891 to 784 rows.

4- Dropping Outlier
While observing the data summary using .describe(), one of the 'fare' column had a fairly large difference between 75 percentile and the maximum value which had the risk of disturbance in analysis. This outlier was removed reducing rows to 781.
  
5- Replacing values 
Values in some colummns were True or False which were replaced with yes or no instead.

6- Handling Null Values
<p>Following columns had the null values:</p>
<ul>
     <li>deck = 581</li>
     <li>age = 106</li>
     <li>embark_town = 2</li>
</ul>
Though deck has a lot of null values and normally such type of column is removed but it has a really important role in analysis. Furthermore, there are various factors in dataset that can help determine the deck.
Based on additional information gained, the people on each deck belong to different classes yet they have segregations and different provided facilities.    
They have paid fares based on classes and decks. In order to find the most probable deck we can't depend on any one factor. There are different passenger classes on each deck and all the classes within each deck may be paying different fares. For example, the first class passengers on deck B might be paying less fare on deck C.

Age was easily filled by aggregating ages based on certain criterias. For example, null ages for adult women were filled with the mean age of adult women.

Two additional columns: 'fare_range' and 'adult_range' were also made to ease the process and were removed after served purpose.

7- Analysis
By looking at the data, the first question to arise is: who survied?
First, we analyzed the 'survival_status' based on different categories. 
<ul>
     <li>Out of all the passengers only 41% survived.</li>
     <li>Of those 74% were females.</li>
     <li>Among all women 76% were lucky to survive while only 18% of all man and 59% children were able to make it.</li>
     <li>By categorizing the survival status with respect to decks, B was the safest deck with the survival ratio of 69% whereas 75 of every 100 individuals lost their 
      lives in deck G.</li>
     <li>Since titanic is famous for class discrimination, 63% of the first class passengers were saved by providing facilities while 74% of third class people drowned.</li>
     <li>51% of people with families survied.</li>
     <li>Adult males </li>
     <li></li>
     <li></li>
     <li></li>
     <li></li>

</ul>
Later on doing the statistical analysis, I came to know that
All the heavy fairs "actually outliers" were paid by first class passengers but some of the first class passengers paid no fare at all







 
