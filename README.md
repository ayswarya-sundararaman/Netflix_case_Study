

# Netflix Recommendation System Case Study

## Dataset
- **Netflix Prize Dataset**: 
  - **User Ratings**: Anonymous movie ratings from users between 1999 and 2005.
  - **Data Files**: `combined_data_1.txt`, `combined_data_2.txt`, `combined_data_3.txt`, and `combined_data_4.txt`.
  - **Features**: Movie ID, User ID, Rating, Date.

## Problem Statement
- **Objective**: Predict the rating a user would give to a movie they haven’t rated yet.
- **Metrics**: Minimize RMSE (Root Mean Squared Error) and MAPE (Mean Absolute Percentage Error).
  
## Models Implemented
1. **Collaborative Filtering**:
   - Explored user-user and item-item similarity using **cosine similarity**.
   - Applied **Matrix Factorization** using **Truncated SVD** for dimensionality reduction and faster similarity computation.

2. **Content-Based Filtering**:
   - Integrated movie metadata like titles and release dates for content-based recommendations.
   - Used **TF-IDF** for text-based similarity on movie descriptions.

3. **Hybrid Approach**:
   - Combined collaborative and content-based filtering to improve recommendation accuracy.

## Results
- **Truncated SVD**: Reduced dimensionality of user-movie matrix, speeding up computations.
- **RMSE Improvement**: Models achieved significant reduction in RMSE over baseline Cinematch performance.

## Conclusion
The hybrid model using collaborative filtering with SVD-based dimensionality reduction, combined with content-based filtering, provided the best accuracy and efficiency in predicting movie ratings.

