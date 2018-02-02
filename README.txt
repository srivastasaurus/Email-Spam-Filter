Spam filtering is a document classification task which involves classifying an email as spam or non-spam mail.

Dependencies: 
   Scikit-learn dependencies : pip install scikit-learn
   Nltk: pip install nltk
   Pandas : pip install pandas
   numpy : pip install numpy

To build this application:
First extract equal number of spam and non-spam emails from Ling-spam Corpus. 
1. For preparing the text data, the data-set is split into a training set and a testing set. Then, we perform text cleaning where stop words like "and","the","of",etc are removed that are not meaningful.
    Another process to prerpare the dataset is lemmatization which is the process of grouping inflected words.

2. Creating a dictionary will help in counting the frequency of words in the data set.

3. After the dictionary is prepared, extrac the feature vectors, as per training mail and its labels.   

4. We'll be using scikit-learn ML librarry models- naive bayes classfier and SVM (to separate some of the training data from rest) for training classifiers. 
   
    Once the classifiers are trained, we can check the performance of the model.
    We extract word count vector of each mail in testing-set and predict its class(ham or spam) with the trained NB classifier and SVM model.
