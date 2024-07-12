# Clustering and Recommendation System for Netflix Shows

# Description
This project conducts exploratory data analysis (EDA) and clustering analysis on a Netflix content dataset. The goal is to uncover insights and patterns, clustering the content based on textual attributes to understand categorization and trends.

# Objective
The objective of this project is to analyze the Netflix dataset to identify patterns and trends in the platform's content. Additionally, it aims to perform clustering to group similar movies and TV shows based on their attributes, offering a clearer understanding of content distribution and characteristics.

# Attribute Information
- show_id : Unique ID for every Movie / Tv Show

- type : Identifier - A Movie or TV Show

- title : Title of the Movie / Tv Show

- director : Director of the Movie

- cast : Actors involved in the movie / show

- country : Country where the movie / show was produced

- date_added : Date it was added on Netflix

- release_year : Actual Releaseyear of the movie / show

- rating : TV Rating of the movie / show

- duration : Total Duration - in minutes or number of seasons

- listed_in : Genere

- description: The Summary description

# Conclusion

- **Key Findings from EDA:**
  Netflix hosts more movies than TV shows, with the total number of shows increasing significantly over time. Most shows are produced in the United States, primarily targeting adult and young adult audiences.
  
- **Clustering Approach:**
  We clustered the data based on attributes such as director, cast, country, genre, and description. These attributes were tokenized, preprocessed, and vectorized using a TFIDF vectorizer.

- **Feature Engineering:**
  We generated 20,000 attributes using TFIDF vectorization.

- **Dimensionality Reduction:**
  Principal Component Analysis (PCA) was applied to reduce dimensionality. We found that 4,000 components captured over 80% of the variance, so we limited the components to 4,000.
  
- **Clustering Algorithms:**
  The elbow method and Silhouette score analysis determined an optimal number of 6 clusters. -Agglomerative Clustering: Dendrogram visualization identified 12 optimal clusters.

- **Content-Based Recommender System:**
  A content-based recommender system was developed using cosine similarity. This system provides 10 recommendations based on the type of show a user has watched.

