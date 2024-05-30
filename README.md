# Movie Classification and Sentiment Analysis

This project explores movie data from Rotten Tomatoes, performing sentiment analysis on movie reviews and classifying movies based on various features. The project is divided into two parts:

1. **Movie Classification**: Using a Random Forest Classifier to predict the tomatometer status of movies based on features such as runtime, ratings, and content rating.
2. **Sentiment Analysis**: Utilizing a pre-trained sentiment analysis model from Hugging Face Transformers to analyze critic reviews and predict the overall sentiment of a movie.

## Results

### Movie Classification

#### Decision Tree and Random Forest Classification

- **Accuracy**: The decision tree and random forest classifiers achieved accuracies of 99% and 99.26%, respectively, on the test data.
- **Confusion Matrix**: The confusion matrices below show the distribution of predicted and actual classes:

  ![Decision Tree Confusion Matrix](<img width="646" alt="decision_tree_cm" src="https://github.com/andrea-cas/rotten_tomatoes_movie_predictions/assets/155782270/7d174293-419e-423f-ae16-0127f455f819">)
  ![Random Forest Confusion Matrix](<img width="638" alt="random_forest_cm" src="https://github.com/andrea-cas/rotten_tomatoes_movie_predictions/assets/155782270/f4947c2f-7d56-4b6f-ae01-98149a77a239">)


### Sentiment Analysis

#### Hugging Face Transformers Sentiment Pipeline

- **Sentiment Prediction Accuracy**: The sentiment analysis pipeline achieved an accuracy of 81.3% on the test set.
- **Movie Status Predictions**: Out of 4 test cases, all predictions made by the `predict_sentiment` function were correct.
- **Example Predictions**: Here are some example predictions made by the sentiment analysis pipeline:

  - Review: "This action-packed fantasy adventure, based on Rick Riordan's hit Percy Jackson and the Olympians series of books, is great fun, and deserves to find an audience with teens now bereft of any Harry Potter magic." Predicted Sentiment: Positive
  - Review: "there's not one single thing in it that will appeal to a person who has ever seen a mythological origin story before, much less any other sort of adventure movie." Predicted Sentiment: Negative

### Interpretation

- The classification models demonstrate strong performance in predicting movie classifications based on various features.
- The sentiment analysis pipeline provides accurate predictions of sentiment for movie reviews, allowing for the determination of overall movie sentiment.

### Limitations and Future Work

- The models may exhibit biases or limitations inherent in the dataset used for training.
- Future work could involve fine-tuning the models, incorporating additional features, or experimenting with different algorithms to further improve performance.

## Datasets

The datasets used in this project are:

- **Rotten Tomatoes Movies Dataset**
- **Rotten Tomatoes Critic Reviews Dataset**

### Download from Hosting Service

Due to size constraints, the full dataset is hosted externally. You can download the datasets from the following link:

- [Rotten Tomatoes Movies and Critic Reviews Dataset](https://www.kaggle.com/datasets/stefanoleone992/rotten-tomatoes-movies-and-critic-reviews-dataset)
