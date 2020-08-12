# NLP
Repository for Text, Web and Social media Analytics lab homework

## Text Preprocessing

Very first step of NLP.  It includes:
* Getting rid of whole lines that are not conveying any usefull information
* Removing Punctuation, Numbers, extra spaces and any other unuseful characters
* Transforming everything into lower case, to decrease the number of potential features for later application in a model
* Removing stop words
* Removing short words (< 3 characters)
* Stemming /  Lemmatization

## Text Representation
Tranforming unstructured textual data into structured (i.e. vectors). Different approaches tested.

### Bag of words (BoW)
Uses a vector where each feature represents one word of the dictionary. Feature importance can be derived with different methods

#### One-hot encoding
Binary representation depending on the appearance of the word in the document

#### Absolute frequency
Value is the number of appearances of a word => more common words are more important

#### Relative frequency 
Absolute text frequency/ length of document

#### TF-IDF frequency
Considers the occurence among all documents => Artificially increases importance of rare words and decreases importance of very common words

### N-Grams
Uses combinations of consecutive words

### Embeddings 
Represent words in a continuous vector space such that similar words are closer together 

#### Word2Vec
Created by Google. Based on a two layer neural network. Words that appear in similar contexts must have a similar embedding representation

#### Contextual Embeddings
* Embedding for Language Models (ELMo)
* Bidirectional Encoder Representations from Transformers (BERT)

## Classification 
Supervised learning. Requires annotated corpus. Comparison with two different models
* Naive Bayes
* Random Forest

## Clustering
Unsupervised learning. Unannotated corpus. Two types were explored:
* K-means
* LDA Topic Modelling

## Text Analytics in Social Media
Sentiment analysis done with different packages 

## Mining Social Graphs
Building graphs from Twitter dataset, degree-centrality calculation

## Web Analytics
Visualization of main metrics
* Bounce Rate
* Exit Rate
* Page Value
* etc..
