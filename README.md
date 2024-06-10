# Music Recommender System using Collaborative Filtering

This project implements a music recommender system using collaborative filtering with the k-nearest neighbors (kNN) algorithm. It predicts songs that a user may like based on the preferences of similar users.

### Types of Recommender Systems
There are two main types of recommender systems:
- Content-based filters
- Collaborative filters

This project focuses on collaborative filtering, specifically user-item collaborative filtering with the kNN algorithm.

### Steps:
1. **Importing Required Libraries:** 
   - Pandas for data manipulation
   - NumPy for numerical operations
   - Matplotlib and Seaborn for data visualization
   - `csr_matrix` from Scipy for sparse matrix representation
   - `Recommender` class from `knn_recommender` module

2. **Reading the Files:**
   - Utilizing the Million Song Dataset containing user-song interactions and metadata.
   
3. **Exploring the Data:**
   - Identifying unique songs, artists, and users
   - Analyzing song and artist popularity
   - Investigating user-song interaction patterns

4. **Prepare the Data:**
   - Filtering the dataset to include users with a minimum number of song listens
   - Converting the data into a sparse matrix format to handle sparsity efficiently

5. **Model and Recommendations:**
   - Building the recommender system using kNN algorithm
   - Making song recommendations for given input songs

### Usage:
1. Clone the repository.
2. Install the required libraries listed in `requirements.txt`.
3. Run the provided Python scripts in the specified order.

### Example:
```python
from recommeders.knn_recommender import Recommender

# Initialize Recommender object
model = Recommender(data=mat_songs_features, decode_id_song=decode_id_song)

# Get recommendations for a song
recommendations = model.make_recommendation("I believe in miracles")

print("Recommendations:")
print(recommendations)

License:
This project is licensed under the Amrutha


Feel free to customize it according to your project's specifics.
