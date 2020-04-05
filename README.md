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
   
# Result 
Using Tf-Idf achieves the highes f1-score. The result is shown in the table below:

**Gender**: _female_: 0, _male_: 1

. | precision | recall | f1-score | support
------------ | ------------- | ------------- | ------------- | -------------
0 | 0.79 | 0.82 | 0.80 | 1200
1 | 0.81 | 0.78 | 0.79 | 1200
accuracy | _ | _ | 0.80 | 2400
macro avg | 0.80 | 0.80 | 0.80 | 2400
weighted avg | 0.80 | 0.80 | 0.80 | 2400

**Language Variety**: _australia_: 0, _canada_: 1, _great britain_: 2, _ireland_: 3, _new zealand_: 4, _United States_: 5

. | precision | recall | f1-score | support
------------ | ------------- | ------------- | ------------- | -------------
0 | 0.85 | 0.83 | 0.84 | 400
1 | 0.78 | 0.85 | 0.81 | 400
2 | 0.85 | 0.81 | 0.83 | 400
3 | 0.87 | 0.85 | 0.86 | 400
4 | 0.91 | 0.90 | 0.90 | 400
5 | 0.82 | 0.82 | 0.82 | 400
accuracy | _ | _ | 0.84 | 2400
macro avg | 0.85 | 0.84 | 0.84 | 2400
weighted avg | 0.85 | 0.84 | 0.84 | 2400




