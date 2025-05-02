MOVIE RECOMMENDATION
This project is a simple content-based movie recommendation system that uses genre similarity to recommend movies
It is built using Python and pandas, and computes cosine similarity between one-hot encoded genre vectors to find movies similar to a user's input.
📁 Workflow Summary
1. Load Dataset
Import a local CSV file of movies that includes genre labels.
2. Preprocessing
Replace any occurrences of '(no genres listed)' with an empty string.
Split genre strings (e.g., "Action|Adventure") into lists.
One-hot encode the genres into binary vectors for each genre.
3. Build Similarity Matrix
Use cosine similarity to compare one-hot encoded genre vectors.
Create a similarity matrix where each movie is compared with all others.
4. User Input
Accept a movie title from the user (year is optional).
Clean the input by removing any year suffix.
Match the cleaned title against entries in the dataset.
5. Recommendations
Find similar movies using the similarity matrix.
Filter by a similarity threshold.
Return the top N most similar movies based on genre.
