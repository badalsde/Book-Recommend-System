# Book-Recommend-System
This is a Book Recommender System developed using both Popularity Based Recommendation System and Collaborative Filtering technique, which suggests books to the user based on their past ratings and other similar users.
## Popularity Based Recommendation System
The Popularity Based Recommendation System suggests books based on their popularity. It recommends the top 50 most popular books based on the ratings and number of reviews.

## Collaborative Filtering Recommender System
The Collaborative Filtering Recommender System uses the ratings given by the users to find other users with similar interests, and recommends books that those similar users have liked. The system uses cosine_similarity `Cosine similarity is a measure of similarity between two non-zero vectors of an inner product space.it is commonly used as a distance metric to measure the similarity between two feature vectors` algorithm to find the similarity between books. These cosine similarity are then used to predict the ratings for the books that the user has not yet rated.

Table of Contents
- Installation
- Usage
- Dataset
- Model Training
- Web Application
## 1. Installation
To run this project, you will need to have Python 3 installed on your system, along with the following libraries:
- pandas
- numpy
- scikit-learn
- flask
## 2. Usage
To use this project, you can simply clone this repository and run the app.py script using the following command:

run app.py

This will launch the web application in your default browser. You can then enter the book name, based on your book name the model will recommend five books name with poster.

## 3. Dataset
The dataset used in this project is sourced from kaggle.com, and includes some popular books and publishers. The dataset includes the following features:

You can find the dataset 1. [book](https://github.com/badalsde/Book-Recommend-System/blob/main/Books.csv) 2. [user](https://github.com/badalsde/Book-Recommend-System/blob/main/Users.csv) 3. [rating](https://github.com/badalsde/Book-Recommend-System/blob/main/Ratings.csv)

- ISBN
- Book-Rating
- Book-Title	
- Book-Author
- Year-Of-Publication
- Publisher

The dataset has been preprocessed to handle missing values and categorical variables.

## 4. Model Training
The machine learning model used the ratings given by the users to find other users with similar interests, and recommends books that those similar users have liked. The system uses cosine_similarity, trained using the scikit-learn library. The model has been trained on the book, user and rating dataset, and achieves a mean absolute error as less as possible.

The model has been saved as a books.pkl file, which is loaded by the app.py script.

## 5. Web Application
The web application is built using the Flask framework, and allows users to enter the sbook name and get 5 recommend book name. The application includes a simple user interface with input fields for enter movie name, as well as an output field for recommend 5 books name.

To run the web application, simply run the app.py script using the following command:

run app.py

## Contributing
If you find any issues or have any suggestions for this project, feel free to create a pull request or submit an issue.

