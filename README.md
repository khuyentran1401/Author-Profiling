# Task

Identity gender and language variety in Twitter in English. In specific, we want to classify between **male** and **female** and their locations including **Australia, Canada, Great Britain, Ireland, New Zealand, United States**

# Dataset

Dataset is provided by [Pan 2017](https://pan.webis.de/clef17/pan17-web/author-profiling.html)

# Methods
* Get data from .xml files
* Preprocessing with NLTK
  * Filter stopwords, punctuations, and lowercase
  * Tokenize
  * Stem words
* Visualization
  * Visualization with TSNE (a tool to visualize high-dimensional data)
* Model training
  * Support Vector Machine with variety of embeddings, including:
    *  Bag of words from scratch
    * Tf-Idf Vectorizer
    * Word2Vec
    * Combination of Tf-Idf and Word2Vec
    * BERT
   * Neural Network with BERT and PyTorch


