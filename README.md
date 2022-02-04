# Arabic-Sentiment-Analysis-Python-AJGT

# Description:
1) The dataset we used is "AJGT" it introduces an Arabic Jordanian General Tweets (AJGT) Corpus consisted of 1,800 tweets annotated as positive and negative.

2) First step we loaded the dataset file with xlsx format but Pandas blocks this format for security reasons so we used 'openpyxl' engine to load the data.

3) Then we used nltk.download() To download stoping words from NLTK.

4) 1- In preprocessing the data we subjected the data to preprocessing, we removed both arabic and english punctuation and Normalized different letter variants with one common letter.

    2- We made a list of arabic and english punctiations that we wand to remove from our text then we loaded the Arabic stop words with NLTK.

    3- Then we defined a list with Arabic diacritics "Tashkeel" to remove them .

    4- We removed the punctiations and diacritics "Tashkeel" and converted the longation characters like {إ,أ,آ,ا,ي,ؤ,ئ,ة} to {ا,ه,ي,ء}.

    5- Then we splitted the data to train and test with test size 20%.

5) Then we make a pipeline for each model to use TfidfVectorizer() "TF-IDF function is term frequency-inverse document frequency", indicates what the importance of the word is in order to understand the document or dataset.

6) We used grid search to choose the best hyperparameters values.

7) We made 4 models and the accuracy of each of them are

    1- LogisticRegression: 83%

    2- MultinomialNB: 83%

    3- RandomForestClassifier:82%

    4- SVC: 85%
