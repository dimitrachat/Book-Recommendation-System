# Book-Recommendation-System
## Overview
This project aims to build a book recommendation system using the Book-Crossing dataset. The dataset includes information about users, books, and ratings. The goal is to recommend books to users based on their reading preferences and ratings. The project explores various recommendation algorithms, including:

- **Collaborative Filtering**
- **K-Nearest Neighbors (KNN)**
- **Singular Value Decomposition (SVD)**
- **Non-Negative Matrix Factorization (NMF)**

## Dataset
The dataset consists of three main files:
1. **Users**: Contains user IDs, locations, and ages.
2. **Books**: Contains book details such as ISBN, title, author, publisher, and image URLs.
3. **Ratings**: Contains user IDs, book ISBNs, and ratings.

## Data Cleaning
Before building the recommendation system, the dataset was cleaned to remove outliers, filter users with fewer than 150 ratings, and books with fewer than 100 ratings. Additionally, only users from the USA were considered, and the age range was limited to 12-85 years to ensure valid ratings.

## Methods
1. **Collaborative Filtering**: A user-based recommendation system that suggests books based on the preferences of similar users.
2. **K-Nearest Neighbors (KNN)**: A method that finds the most similar users based on their book ratings and recommends books accordingly.
3. **Singular Value Decomposition (SVD)**: A matrix factorization technique used to reduce the dimensionality of the dataset and improve recommendations.
4. **Non-Negative Matrix Factorization (NMF)**: Another matrix factorization technique that decomposes the user-item matrix into lower-dimensional matrices to make recommendations.

## Evaluation
The recommendation system was evaluated using metrics such as:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **Precision**
- **Recall**
- **F1-Score**

The best results were achieved using the KNN algorithm after removing zero ratings and focusing on highly rated books.

## Results
- **KNN Algorithm**: Achieved the lowest RMSE and improved precision and recall after data cleaning.
- **SVD and NMF**: Performed worse compared to KNN in terms of RMSE.

## Future Work
- Explore more advanced recommendation algorithms like deep learning-based models.
- Include more data and additional years to improve model accuracy.
- Consider external factors like book genres and user demographics.
