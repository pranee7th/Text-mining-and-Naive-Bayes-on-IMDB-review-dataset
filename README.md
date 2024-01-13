
 **Data Loading and Exploration:**
   - The project begins by importing necessary libraries and loading a subset of the IMDB movie review dataset using pandas. The dataset contains reviews (`X`) and corresponding sentiment labels (`classes`).

 **Text Preprocessing:**
   - Text data preprocessing is a crucial step in natural language processing (NLP). The reviews are cleaned and preprocessed in two parts:
      - **Part 1:** Involves removing special characters, single-letter words, and other noise from the text.
      - **Part 2:** Focuses on lemmatization, splitting words, and creating a clean representation of the reviews.

 **Vectorization:**
   - The text data is converted into a numerical format using the CountVectorizer from scikit-learn. This step involves creating a matrix (`texts`) that represents the frequency of each word in each review and a list (`vocab`) containing all unique words.

 **Data Splitting:**
   - The dataset is split into training and testing sets using the `train_test_split` function. 80% of the data is used for training and 20% for testing.

 **Naive Bayes Model Training:**
   - A Multinomial Naive Bayes classifier (`clf`) is imported from scikit-learn, fitted to the training data, and used to predict sentiment on the test data.

 **Model Evaluation:**
   - The accuracy of the model is evaluated on both the training and test sets using the `accuracy_score` function. Additionally, a classification report is generated, providing precision, recall, and F1-score for each sentiment class.

 **Results and Analysis:**
   - The project concludes with an analysis of the model's performance. The accuracy on the training set is high (92.15%), but there is a slight drop in accuracy on the test set (83.1%). This is expected as the model is tested on new, unseen data.
   - The classification report indicates good performance in terms of precision, recall, and F1-score for both positive and negative sentiments.

In summary, this project focuses on sentiment analysis using a Naive Bayes classifier on IMDB movie reviews. It involves data preprocessing, vectorization, model training, and evaluation, providing insights into the model's performance on both training and test datasets.
