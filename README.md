# Text Mining and Collective Intelligence Project by Kamiel Fokkink, Baran Iscanli, and Vera Neplenbroek

## Title

## Abstract
A max 150-word description of the project question or idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

## Research questions
A list of research questions you would like to address during the project. 

## Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show you've read the docs and are familiar with some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

## A tentative list of milestones for the project
* Preprocessing
  * Tokenize
  * PoS tagging
  * Lemmatize
  * Filter
  * Sample the dataset to theoritize
* Training the model
  * Decide on a couple of models to experiment with
  * Analyze the data
    * Frequency counts
    * N-grams
    * Choose the most suitable
* Evaluating
  * Compare the results of model with an existing gold standard
  * Analyze accuracy

## Documentation
This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.

## Brainstorm
Start with a pre-processing pipeline, create a base model that works without any extra grammar/language support, use grammar/language support for Dutch <-> English to improve the base model. Two models: one English-Dutch, one Dutch-English. End result: input: word in one language, output: sorted list of most likely translations in the another language.
