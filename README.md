# Online-learning-Twitter-API-kafka-river
Group 14: Salma EZZINA and Chaima ELMESSAI
Project 8: (Social Network data) Collect tweets from Twitter API  in real-time and use a batch or 
online classification method to classify them for sentiment analysis.

This project was done using: Twitter API, Kafka, river, and sklearn.

Our tasks:
1. Sentiment analysis task, tackeled as a supervised multi-class classification.
2. Group community detection, tackeled as an unsupervised clustering task.

Each of these tasks' codes will be found in the corresponding folder, named as the name of the task.


Each folder contains 3 notebooks:
1. The first notebook named: TwitterApi_SendingAndSavingData
is to scrap twitter data using the twitter api and send it via kafka producer to the consumer, 
plus it saves the collected data locally.
REMARK1: The data will be generated after executing this notebook
Remark2: This notebook is almost the same for the two tasks
2. The second one: OnlineLearning_<TaskName> contains the online learning methods 
(the subscribed consumer will recieve the data and process it in real time),
with the needed NLP transformations on the data.
3. The third one named: BatchLearning_<TaskName> contains the batch tasks, with the data saved earlier.


Models used:
1. For the sentiment analysis task: 
	i. for online learning: 
			kNN, one Vs one logistic regression, and Hoeffding tree
	ii. for batch learning:
			kNN and one Vs one logistic regression

2. For community detection task: 
	i. for online learning: 
			Kmeans, STREAMKmeans and DBSTREAM
	ii. for batch learning: 
			Kmeans, DBSCAN, AgglomerativeClustering 
			
