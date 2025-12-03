# Movie Recommendation System Using Hybrid Similarity

**Course:** 02807 Computational Tools for Data Science  
**Institution:** Technical University of Denmark (DTU)  
**Semester:** Autumn 2025

---

## Team Members
- [Member 1 Name] - Student ID
- [Member 2 Name] - Student ID
- [Member 3 Name] - Student ID
- [Member 4 Name] - Student ID

---

## Project Summary

This project implements a **hybrid movie recommendation system** that combines multiple similarity dimensions to find movies similar to a given query. Using the Rotten Tomatoes dataset, we demonstrate:

1. **Course Topic 1 - Similar Items:** We compute pairwise similarity across movies using six distinct feature types, combined through weighted averaging.

2. **Course Topic 2 - Clustering:** K-Means clustering is applied to group movies by genre characteristics, with evaluation using Davies-Bouldin index and silhouette scores.

3. **Outside Topic - Topic Modeling (LDA):** We use Latent Dirichlet Allocation to discover latent topics from critic reviews, enabling automatic genre label generation based on review content rather than predefined categories.

The system produces recommendations by computing a hybrid similarity score:

$$
S_{hybrid} = \alpha \cdot S_{info} + \beta \cdot S_{rating} + \gamma \cdot S_{genre} + \delta \cdot S_{year} + \epsilon \cdot S_{style} + \zeta \cdot S_{type}
$$

---

## Data Requirements
Place the following files in the `datasets/` folder:

- `rotten_tomatoes_movies.csv`
- `rotten_tomatoes_critic_reviews.csv`

**Dataset Source:**  
[Rotten Tomatoes Movies and Critic Reviews Dataset on Kaggle](https://www.kaggle.com/datasets/stefanoleone992/rotten-tomatoes-movies-and-critic-reviews-dataset/data?select=rotten_tomatoes_movies.csv)

---

## Dependencies
All required Python packages are listed in `requirements.txt`. Install them using:

```bash
pip install -r requirements.txt
