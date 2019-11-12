# Text Mining and Collective Intelligence Project by Kamiel Fokkink, Baran Iscanli, and Vera Neplenbroek

## Building a translation model

## Abstract
The goal of this project is to create a functioning English-Dutch translation model. The model is trained on data from movie subtitles, by comparing both the English and the Dutch subtitle lines for the same movies. The exact approach with which we will build the translation model is still to be figured out, but it will probably require machine learning techniques such as neural networks. Ideally we want to create a model that can take any Dutch or English word as input, and gives a list of one or several words from the other language that are likely to mean the same. To evaluate the performance of our model, we will compare its output with other existing models that are proven to work.

## Research questions
-	How to preprocess our data in a meaningful and helpful way?
-	What is a suitable approach to making a translation model?
-	How can machine learning techniques be applied to enhance our model?
-	How to implement this approach into code that works with our data?
- How can we evaluate the performance of our model, in comparison to an existing translation model?

## Dataset
We want to use the [OpenSubtitles dataset](http://opus.nlpl.eu/OpenSubtitles-v2018.php) on translated movie subtitles. We will first tokenize the dataset per sentence, then lemmatize the tokens and use part-of-speech tagging on them. We will possibly need to filter out punctuation and very unfrequent words, in both languages. We are planning on using the translation memory files (TMX), and to use the files in python the reader provided by the [translate-toolkit](https://github.com/translate/translate).

## A tentative list of milestones for the project
* Preprocessing
  * Tokenize
  * PoS tagging
  * Lemmatize
  * Filter
  * Sample the dataset to theoritize
* Training the model
  * Research into which kind of models and approaches exist
  * Decide on a couple of models to experiment with
  * Analyze the data
    * Frequency counts
    * N-grams
    * Choose the most suitable model
* Evaluating
  * Compare the results of model with an existing gold standard
  * Analyze accuracy

## Documentation
This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.

## Brainstorm
Start with a pre-processing pipeline, create a base model that works without any extra grammar/language support, use grammar/language support for Dutch <-> English to improve the base model. Two models: one English-Dutch, one Dutch-English. End result: input: word in one language, output: sorted list of most likely translations in the another language.
