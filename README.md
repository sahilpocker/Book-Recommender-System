# Book Recommender System Using Keras
***
This is a Book Recommendation system using keras, made using the [goodbooks-10k](https://www.kaggle.com/zygmunt/goodbooks-10k "goodbooks-10k") dataset

We will use a technique called collaborative filtering using the keras framework, even-though this doesnt qualify as a deep-learning problem.

The Dataset has been saved in the local directory, and the notebook file can be found [here](https://github.com/sahilpocker/Book-Recommender-System/blob/master/book-recommender-system.ipynb "book-recommender-system")

___

Our task is to predict the rating for a user/book pair, with the idea that if we had a model that’s good at this task then we could predict how a user would rate books they haven’t read yet and recommend books with the highest predicted rating.

### Data cleaning and tranformation
* Duplicate entries have been removed 
* The _user_id_ and _book_id_ has to be converted to sequential integers first, starting from zero. This is because these fields are currently non-sequential integers with a unique ID.

___

The model performed reasonably well with 5 epochs, without overfitting much.

![Trainind-Test-Curve](https://i.imgur.com/qptDlEC.png)