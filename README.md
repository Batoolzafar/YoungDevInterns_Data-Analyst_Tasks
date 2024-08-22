# ⏳ YoungDevIntern-Internship

## About the Dataset
<p>The example dataset of seaborn used in this project is the most famous Titanic dataset🚢. This dataset is best for analysis as well as creating dashboards and machine learning models. Morever, it is related to one of the most unprecedented events in world history which makes the task even more interesting.</p>p>

## 📝 Task 1: Perform Advanced Data Analysis with Python

<b>Outline</b>
<p>Throughout the project I went through the following steps:</p>
<ol>
     <li>Manipulating column names</li>
     <li>Dropping extra columns</li> 
     <li>Dropping Duplicates</li>  
     <li>Dropping Outlier</li> 
     <li>Replacing values</li> 
     <li>Handling Null Values</li>
     <li>Analysis (Statistical and Visual)</li>
     </ol>

### 🛠 Manipulating column names     
<p>The initial column names were replaced to make them self explanatory. This not only helped me in analysis but will also be helpful to others viewing the project.</p>

### ✂ Dropping extra columns
<p>While analyzing all 15 columns in the dataset I noticed that some of them were repeated with different values.</p>
<ol>
     <li>'Embarked' had the short form of towns and 'embark_town' was filled with full town names.</li>
     <li>'Survived' had values 1 and 0, unlike 'survival_status' which was filled with True and False instead.</li>
     <li>'Class' had class numbers written in letters contrary to passenger class filled with integral values.</li></ol>
    
<p>After munging, the following 12 columns were ready for analysis:</p>
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

### 🧨 Dropping Duplicates 
<p>Suprisingly, dropping duplicates reduced the data from 891 to 784 rows.</p>

### 🗑 Dropping Outlier
<p>While observing the data summary, one of the 'fare' column had a fairly large difference between 75 percentile and the maximum value which had the risk of disturbance in analysis. This outlier was removed reducing rows to 781.</p>
  
### 🔗 Replacing values 
<p>Values in some colummns were True or False which were replaced with yes or no instead.</p>

### 🔩 Handling Null Values
<p>Following columns had the null values:</p>
<ul>
     <li>deck = 581</li>
     <li>age = 106</li>
     <li>embark_town = 2</li>
</ul>
<b>Additional Information</b>
<p></p>
<p>Though deck has a lot of null values and normally such type of column is removed but it has a really important role in analysis. Furthermore, there are various factors in dataset that can help determine the deck.
Based on additional information gained, the people on each deck belong to different classes yet they have segregations and different provided facilities.    
They paid fares based on classes and decks. In order to find the most probable deck we can't depend on any one factor. There are different passenger classes on each deck and all the classes within each deck may be paying different fares. For example, the first class passengers on deck B might be paying less fare on deck C.</p>

<p>Age was easily filled by aggregating ages based on certain criterias. For example, null ages for adult women were filled with the mean age of adult women.</p>

<p>Two additional columns: 'fare_range' and 'adult_range' were also made to ease the process and were removed after served purpose.</p>

### 🧪 Analysis
<p>By looking at the data, the first question to arise is: who survied?
For that, we analyzed the 'survival_status' based on different categories.</p>
<ul>
     <li>Out of all the passengers only 41% survived.</li>
     <li>Of those 68% were females.</li>
     <li>Among all women 76% were lucky to survive while only 18% of all man and 59% children were able to make it.</li>
     <li>By categorizing the survival status by decks, B was the safest deck with the survival rate of 69% whereas 75 of every 100 individuals lost their 
      lives in deck G.</li>
     <li>Since titanic is famous for class discrimination, 63% of the first class passengers were saved while 74% of third class people drowned.</li>
     <li>51% of people with families survied.</li>
     <li>Most of the survivers belonged to Cherbourg town</li>
     <li>The eldest passenger to survive was an 80 year old first class passenger.</li>
</ul>
<p>Later on doing the statistical analysis, I came to know that
all the heavy fares 💸 ("actually outliers") were paid by first class passengers but some of the first class passengers paid no fare at all.</p>
<p>A new column "fare_category" was made to categorize the fares based on expensive,reasonable,inexpensive and no fares. It was found that a lot of passengers paid low fares. This proposed the idea that most of the people on board were third class which was also proved.</p>
<p>As the Cherbourg residents had the highest survival rate, they had paid the heaviest fares and would have been saved earlier.</p>
<p>The standard deviations in the age and fare columns were very high which means that people of different ages were on board who paid different fares for different facilities.</p>
<hr>
## 📝 Task 2: Creating a Dashboard

![cappppp](https://github.com/user-attachments/assets/1eee4861-5cb0-40fa-871d-3b3ca23c15ff)

This dashboard provides the overview about the survivers and non survivers of the historic wreck.








 
