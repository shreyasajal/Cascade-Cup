# Cascade-Cup
Organizer:Consulting and Analytics Club IIT Guwahati
Team Name:DataFreaks
Competition link:https://dare2compete.com/o/cascade-cup-consulting-analytics-club-iit-guwahati-134091
Total participants:2,035
Round 1:
Data Science Quiz
Rank:88 
The top 500 participants were selected for the next rounds

Round 2
HACKATHON
Problem Statement:
Understanding the customers’ intentions can help to improve the journey, e.g., by taking shortcuts or giving recommendations to improve the overall experience is very important. With the extent of development in the field of machine learning research, personalization of services has become very common. Typically, a user’s intention on a Web site can be understood by looking at their past interactions. In concrete terms, this means that a user leaves a sequence of events about the history of his page views and interactions. An event can be that a user makes a search query, calls up an article page or receives an e-mail. This data forms the basis for working with the following techniques. Therefore, the first step is to collect or extract this data. This step has been done by Trell.

In this world of big data, Trell wants you to use the data to predict the age group of their users based on their activity on social media activities.  This will help them to divide their huge userbase and cater differently to each of them. Given this huge dataset, predict the age group of the users, the evaluation metric for the competition is the Weighted F1 score.


F1 score on private Leaderboard:79.9207
Rank:75th 
Hackathon link:https://dphi.tech/challenges/cascade-cup-data-science-hackathon/46/overview/about
Approach:
1.The training dataset consisted of 488877 rows and 27 columns.After importing the required modules,we headed to data preprocessing.
2.Data Preprocessing:We checked for outliers in data and skewness of the data through boxplots.After that,keeping max threshold of 99.9 percentile and min threshold of 0.01 percentile ,we removed the outliers from the numeric columns that did not fall in the range of min to max threshold
Depending on the skewedness as inferred from the distplots,we used log and sqrt transformation on the respective columns,whichever reduced the skewness better 
Removed the unimportant features from the dataset after extracting the feature scores through SelectKBest class from sklearn's feature selection module.
Finally we fitted different machine learning models on the training dataset,performed hyperparameter tuning using Randomized Search CV given the dataset's big size.
We tried models like:XGB Classifier,Catboost Classifer,K Neighbours,Random Forest Classifiers.The model that we chose for the final submission that fetched us the weighted F1 score=79.9207 was the one that gave us the highest cross validation score on our validation set using K fold cross validation.We made sure that we chose K in a way such that our validation set was similar to the test set used for scoring.

Round 3
EXPLORATORY DATA ANALYSIS ROUND
Problem statement:
Absenteeism is a habitual pattern of absence from a duty or obligation without good reason. Generally,
absenteeism is unplanned absences. If a workplace exhibits high degree of absenteeism there is a
problem. It has been viewed as an indicator of poor individual performance, as well as a breach of an
implicit contract between employee and employer.
This is a 740 x 22 tabular dataset, what each column represents is given in the data dictionary. Your task is
to prepare an extensive report by preforming analysis on the dataset. Provide as many meaningful
inferences and correlations using graphs as you can. Ensure that the report is not more than 10 pages
(including the introduction and thank you pages).
We prepared an extensive data analysis report using seaborn anmd matplotlib libraries in Python.
Overall competetion rank:75th
