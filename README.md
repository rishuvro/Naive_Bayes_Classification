# Naive_Bayes_Classification
# **NB Classifier for Text Classification**

Let's now give an example of text classification using the Naive Bayes method. Although this method is a two-class problem, the same approaches are applicable to multi-class settings. Let's Say we have a set of reviews (document) and its classes:

| Document | Text | Class |
| --- | --- | --- |
| 1 | I loved Crow | + |
| 2 | I hated Crow | - |
| 3 | Crow is a good bird. | + |
| 4 | It's black and Dirty | - |
| 5 | Black is a Good Color. | + |

Prior to fitting the model and using a machine learning algorithm for training, we need to think about how to best represent a text document as a feature vector. A commonly used model in Natural Language Processing (NLP) is a so-called bag of words model.

The idea behind this model is really simple. The first step is the creation of the vocabulary - the collection of all different words that occur in the training set. For our example, vocabulary, which consists of 10 unique words could be written as:

\< I, loved, crow, hated, a, great, poor, dirty, good, color \>

Using tokenization, which is general process of breaking down a text corpus into individual elements that serve as input for various NLP methods, Usually, tokenization is accompanied by other optional processing steps such as removal of stop words and punctuation characters, stemming or lemmetizing and construction of n-grams.

Using Python, let's convert the documents into feature sets, where the attributes are possible words and the values are number of times a word occurs in the given document
