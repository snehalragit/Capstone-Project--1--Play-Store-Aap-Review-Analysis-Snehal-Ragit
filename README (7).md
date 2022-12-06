

## ABSTRACT
Google Play Store is a digital distribution service operated by Google. Google Play Store mainly works for Android devices, from where Android users can download various apps as per their needs on their phones That is, it acts as an application store. Mainly here the apps are free to download on their phones. As various developers are publishing their apps on Google Play Store on one hand and users are using them on the other hand, From which a financial side of the developers is also getting prosperous. Google arranges app rating for users which basically allows users to tell how they feel about an app after using it but it is completely personal.
## PROJECT DESCRIPTION
This project contains
1 colab notebook,
1 technical documentation
1 presentation
## INTRODUCTION
Currently there are at least 25 lakh apps on play store. Today we will show how we analyzed the apps obtained from the dataset through the Python library on this project. The data set has 13 columns and 10841 rows. After cleaning the data, we analyze which apps are most popular and why? Which apps are the least popular and why? What is the problem with the apps that are least popular and what should be done to bring them back to popularity.



## PROBLEM STATEMENT
1.How many apps are free or paid?
2.Which apps are at the top of their popularity?
3.Which apps category have been downloaded the most?
4.  The most popular category among the categories that appear on the Play Store dataset?
5.What percentage of apps are free?
6.The name of the most downloaded apps among the paid apps?
7.How many free apps have been downloaded over a million?
8.Which apps received the most positive and the least negative reviews?
## DESCRIPTION OF DATASET
It had 10841 rows and 13 columns.  so  let's analyze it .
This dataset holding following  columns:
App: This section contains the name of  apps.
Category:  The category indicates which type the app is. It is seen here that there are 33 unique values
Rating: This column shows the average calculations of users by taking feedback from them. The value of opinion is between zero and five.
Review: This column carries out how many users voted on that particular app.
Size : How much Android device space a user needs to install the app is the work of the size column.
Installs : It keeps track of how many people have downloaded the apps. However, this is not exact data.
Type : This column tells you whether you have to pay to download this app or it can be used for free.
Price : The prize column indicates how much money to pay to download this app if the type column tells you it's not free If free, its value is zero.
Content Rating : This section indicates that which audience or age group's people this app targeted.
Genres : The column of the genre indicates which sub-category the app belongs to
Last Updated : This column indicates when was last updated for users to use it better after it was published on a PlayStore.
Current Ver : Here is a description of which version this app can currently run on.
Android Ver : This column determines how much the user's Android version needs to be to use the app.
## STEPS
#DATA CLEANING AND PREPARATION: STAGE 1 - We have run df.head() & df .tail() for getting data how it look is. We also run df.collumn() & df.shape() to get full columns data & get how many row & collumns present here.
We have pass a code df.info() [df=play store dataset] which shows us full information about columns.
We also check duplicate data & found it,so we have drop it from dataset & check the shape of dataset.we also trying to find out missing value in column , fill it ‘FREE’ to use it as usable & drop unusable columns(android ver & cureent ver). Then we have showing plot distribution.

STAGE 2- We have Columns like Reviews, Size, Installs, Price are of object type so we can change their data type to integer/float.We can see the size of column, which should be numeric , is of the data type ‘object’, it also has characters ‘k’ (kilobyte) and ‘M’ (megabyte) in the values.So we have removing M and replacing  K with e-3. Some values also found ‘+’ , ‘,’ ‘$’ sign in them, which will be removed.after we looked at the ’last updated’ column it contains the date on which the app is updated/launched last time. It is of object type so we have to convert date in the date-time format. Now we have got final dataset to explore it.

## WHAT WE HAVE DONE IN THIS PROJECT
1.Which category app present most & which category app install most
2.FREE  APP v PAID APP
3.PAID CATEGORY SECTION
4.CORRELATION  HEATMAP
5.INFLUENCE OF PRICE ON RATING
6.UPDATE YEAR &  DETAILS
7.SIZE v INSTALLS
8.LOG INSTALLS & SCATTER PLOT SIZE
AND A LOT OF THINGS
## CONCLUSION
Through the analysis of exploratory data, we have tried to observe that which apps appear on the Play Store have attracted people more and which apps have attracted the crowd the most. The project also shows the reasons for the apps that could not attract the crowd. We can explore more:
a)First of all we can say that 91.9% apps are free & 8.1% apps are paid.
b)Most apps are available in Family category.
c)Most favorite category of users is Game.
d)The most disliked category by users is medical.
e)Personalization is the most popular category among paid apps.
f)Free apps have an average rating of 4.18
g)Paid apps have an average rating of 4.26
h)The number of free apps downloaded more than 1 billion is 20.
i)People prefer small size apps more.
j)Most of the paid apps cost less than $100
k)User mostly liked updated apps.

## REFERANCE
Kaggle
Towards Data Science (TDS)
Pew Research Center
GreeksforGreeks
Python Libraries
GitHub
## IMPORTANT LINK
COLAB_LINK:https://colab.research.google.com/drive/1nnwuizGKKdAKV9bBHeLMV03CDeD88r6-?usp=share_link
PRESENTION_LINK: https://drive.google.com/file/d/1ReutFi-_m3V2IjKxhqgrWyjEilD_qcg5/view?usp=sharing
TECHNICAL_DOUCUMENTION: https://drive.google.com/file/d/15RouD40cIIjzt3bUqiaFeVcOv0KAWgnW/view?usp=sharing
