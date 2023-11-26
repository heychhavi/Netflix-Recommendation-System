# Netflix-Recommendation-System

Build an explicit feedback recommender system: that is, a model that takes into account explicit feedback signals (like ratings) to recommend new content. 

### First Approach: Matrix Factorization
he basic idea is very simple:

Start with user-item-rating triplets, conveying the information that user i gave some item j rating r.
Represent both users and items as high-dimensional vectors of numbers. For example, a user could be represented by [0.3, -1.2, 0.5] and an item by [1.0, -0.3, -0.6].
The representations should be chosen so that, when we multiplied together (via dot products), we can recover the original ratings.
The utility of the model then is derived from the fact that if we multiply the user vector of a user with the item vector of some item they have not rated, we hope to obtain a predicition for the rating they would have given to it had they seen it.
<img src='https://storage.googleapis.com/gweb-cloudblog-publish/images/f1-collab_filtering.max-900x900.png?raw=true' width=50% />
