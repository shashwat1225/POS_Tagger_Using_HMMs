# POS_Tagger_Using_HMMs

This code is a Part-of-Speech (POS) Tagger using Hidden Markov Models (HMM) and Viterbi decoding. The POS Tagger is trained on the Penn Treebank dataset and evaluated against the default NLTK POS tagger.

## Requirements

* NLTK
* Scikit-learn
* NumPy
* Tqdm
* Pandas
* Matplotlib

## How to use

To use the POS Tagger, first download the necessary NLTK data:

`import nltk`

`nltk.download('averaged_perceptron_tagger')`

Then, run the `main()` function. This will load the train, dev, and test sets from the Penn Treebank dataset, and evaluate the performance of the NLTK POS tagger on the test set.

The main function also includes several utility functions for processing and tokenizing text and tags, as well as evaluating the performance of the POS Tagger.

To use the HMM POS Tagger, you can modify the main function to train and evaluate the HMM model on the train and test sets, using the provided utility functions.

The HMM model uses the Viterbi decoding algorithm to find the most likely POS tags for a given sequence of words. The HMM model is trained on the Penn Treebank dataset, using the maximum likelihood estimates of the transition and emission probabilities.

## Evaluation

The performance of the HMM POS Tagger is evaluated using the classification report from scikit-learn, which includes precision, recall, and f1-score for each class. The Confusion Matrix from NLTK can also be used to visualize the performance of the POS Tagger.
