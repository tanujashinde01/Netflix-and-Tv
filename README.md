# Netflix-and-Tv


This project is an exploratory data analysis (EDA) and clustering analysis of Netflix content data. The objective was to gain insights into the distribution, genres, and characteristics of Netflix content while applying machine learning techniques, particularly clustering, to uncover hidden patterns.

The initial phase of the project involves exploratory data analysis (EDA) to understand the structure and insights hidden in the dataset. This includes identifying the types of content available (TV Shows vs Movies), their distribution across countries, release years, ratings, and genres (listed_in). The dataset comprises 7787 entries with 12 columns, including metadata such as title, cast, country, director, date added, release year, and description. While there were missing values in columns like director, cast, and country, the data was clean from duplicate entries.

A TF-IDF vectorization technique was applied to convert the text-based 'description' and 'listed_in' feature into numerical format suitable for clustering. The text preprocessing steps included tokenization, stop word removal, lemmatization, and vectorization using TfidfVectorizer. The dimensionality of this data was then reduced using Principal Component Analysis (PCA) to make it easier to visualize and interpret.

With the vectorized and reduced features, K-Means clustering was implemented to group similar content. The optimal number of clusters was determined using the Elbow Method and Silhouette Scores, which helped understand the internal cohesion and separation of the clusters.

Hierarchical Clustering was also performed in the final steps of the project to validate and compare results obtained from K-Means clustering. Hierarchical clustering was visualized using a dendrogram, providing a different perspective on content similarity based on text-based features.
