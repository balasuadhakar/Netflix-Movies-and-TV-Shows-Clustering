# Netflix-Movies-and-TV-Shows-Clustering

# **Project Summary -**

The main aim of this project is to utilize NLP techniques to analyze the Netflix Dataset containing movies and TV shows .The major objective is to categorize the content into meaningful clusters, enabling the development of an improved recommendation system. Additionally, the dataset will be thoroughly examined to reveal valuable insights and identify emerging trends in the rapidly expanding domain of streaming entertainment.
Steps followed in this project are:
1.	Importing the necessary libraries, mounting drive and storing data in variables for deriving meaningful insights.
2.	Checking for Null/Missing/Infinite values in our data. followed Binning process where respective feature(Rating) converted into miningful categories.
3.	Exploratory data analysis (EDA) was performed on various attributes and gained insightful findings that will be valuable in preventing subscriber churn.
4.	The hypothesis tests was conducted to gain deeper insights into the relationships between variables in our dataset.
5.	The process of handling the outliers, dropping unnecessary columns and creating appropriate functions are done in Feature Engineering step.
6.	The cluster was created using following attributes: director, cast, country, genre, rating and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.
7.	By using PCA  dimensionality reduction was carried out . 
8.	Finally the  clustering was done using different algorithms, such as K-Means, Agglomerative Hierarchical Clustering, DBSCAN, ElbowCurve,  Dendogram etc.
9.	The content-based recommender system was developed using the cosine similarity matrix. This system analyzes the type of show a user has watched and generates personalized recommendations for the user, which is expected to improve user experience and reduce subscriber churn for Netflix.

# **Problem Statement**

This dataset containing of movies and TV shows existing on Netflix as of 2019. The Flixable search engine was used to collect the dataset. 
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. 
The streaming service's number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. 
It will be interesting to explore what all other insights can be obtained from the same dataset. 
Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

### Variables Description 

The variable description of the Netflix Movies and TV Shows Clustering Dataset is as follows:

1. **show_id:** Unique identifier for each movie/show.

2. **type:** Indicates whether the entry is a movie or a TV show.

3. **title:** Name of the movie or TV show.

4. **director:** Name of the director(s) of the movie or TV show.

5. **cast:** Names of the actors and actresses featured in the movie or TV show.

6. **country:** Country or countries where the movie or TV show was produced.

7. **date_added:** Date when the movie or TV show was added to Netflix.

8. **release_year:** Year when the movie or TV show was released.

9. **rating:** TV rating or movie rating of the movie or TV show.

10. **duration:** Length of the movie or TV show in minutes or seasons.

11. **listed_in:** Categories or genres of the movie or TV show.

12. **description:** Brief synopsis or summary of the movie or TV show.

# **Conclusion**

**From EDA**


*   Netflix contains 69% movies and 31% TV shows.Top 10 trending directors of movies and TV shows have been identified. The adding of movies and TV shows are more in 10th and 12th months and very low in 2nd month.

*   Top 10 actors in movies and TV shows have been identified. USA and India are in top two places for launching the movies. Documentary type movies and Kids TV shows are more. USA and India are the top 2 countries for creating new contents. 
*  Adult content movies and TV shows have the more ratings.Family and friends contents less ratings. Most of the movies and Tv shows added in first day of the month and middle of the months. The movies and TV shows released on 2018 and 2019 are more. Older movies are not available more.  
*  Netflix have more movies and TV shows on Adult content and less on Family-Friendly content. More movies and TV shows from USA and more movies and less TV shows from india.Most of the movie duration are between 80 to 120 minutes.The most of the TV shows are in season 1.
*   It was found that most of the countries produces content related to Adult and Teen. Most adult contents produced by Spain, Maxico and France. Egypt, India produces most of the Teen content. Canada produces Children and Family content in better ratio in compaired with other countries, along with Adult and teen content. India has less Adult content with respect to other top countries. Teen and Adult contents duration are more Family-Friend content duration are less.

**From ML Model**



*   The following models were implemented for clustering such as K-means clustering, Agglomerative Hierarchical Clustering, DBSCAN (Density-Based Spatial Clustering of Applications with Noise) and Recommendation System.

*   The optimal number of clusters got from K-means is 4 and from Agglomerative Hierarchical Clustering the optimal number of clusters are found out to be 3.
*   The silhouette Score was choosen used the  evaluation metric over distortion score because it provides a more intuitive and interpretable result. Also Silhouette score is less sensitive to the shape of the clusters.
*   DBSCAN algorithm is not able to differentiate clusters and hence not helped in Project.
*   Built a Recommendation system that can help Netflix improve user experience and reduce subscriber churn by providing personalized recommendations to users based on their similarity scores.

























