## Github Copilot Tweets Analysis
In this project, I extracted tweets from Twitter using API and worked on it. Data is provided into (data)[https://github.com/Prasantkumar987/Natural_Language_Processing_using_Tensorflow/tree/main/Github_Copilot_Tweets_Analysis/data] folder of this repository. 

1. I preprocessed the tweets by applied Natural language techniques using **nltk**,**re**,""collection** libraries.
2. After preprocessing, ploted a **word Cloud** to get a glimpse of my preprocessed data.
3. I embedded, the preprocessed tweets using state of the art **BERT**, it took long to embed them.
4. I used elbow method to find preferred **Clusters** and got 2 clusters from it.
5. I trained, embedded vectors using **Kmeans** algorithm 
6. After that, I printed Silhouette Score and Graph to see the clusters in different color
7. At last, made a list of indexes of tweets falling in both clusters seperately. To check what is sentiment of people lying in different clusters. 
