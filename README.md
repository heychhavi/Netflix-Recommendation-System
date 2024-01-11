# Netflix-Recommendation-System

Build an explicit feedback recommender system: that is, a model that takes into account explicit feedback signals (like ratings) to recommend new content. 

### First Approach: Matrix Factorization

<img src='https://storage.googleapis.com/gweb-cloudblog-publish/images/f1-collab_filtering.max-900x900.png?raw=true' width=50% />

This project demonstrates the implementation of a deep learning-based collaborative filtering model for predicting movie ratings. Using the MovieLens 1M dataset, the model provides personalized movie recommendations based on user preferences.

# Overview
The project includes two primary components:

Building a Deep Learning Model: Utilizing PyTorch, we construct a model to predict movie ratings based on user-item interactions.

Analysis of Predicted Ratings: We analyze the model's performance and estimate movie valuation using the predicted ratings.

Getting Started
# Prerequisites
Python 3.x
PyTorch
Pandas
Matplotlib
NumPy
Scikit-Learn
Model Architecture
The model uses a matrix factorization approach, representing both users and items as high-dimensional vectors. The dot product of these vectors aims to approximate the original user-item ratings.

# Features
Custom Embeddings: User and item embeddings, along with bias embeddings, are used for predictions.

Dataset and DataLoader: Efficient data handling and batching with PyTorch.

Training Loop: Includes validation and test phases with loss computation and optimization.

Analysis Tools: Functions for analyzing top-rated and valued movies, along with PCA visualization of movie embeddings.

# Results
The model demonstrates effective learning of user preferences and item characteristics, with results comparable to benchmark models. Detailed analysis includes top-rated movies, user activity histograms, and movie valuation based on predicted ratings.
