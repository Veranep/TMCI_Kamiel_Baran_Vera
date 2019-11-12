# Text Mining and Collective Intelligence Project by Kamiel Fokkink, Baran Iscanli, and Vera Neplenbroek

## Title

## Abstract
A max 150-word description of the project question or idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The goal of this project is to create a functioning English-Dutch translation model. The model is trained on data from movie subtitles, by comparing both the English and the Dutch subtitle lines for the same movies. The exact approach with which we will build the translation model is still to be figured out, but it will probably require machine learning techniques such as neural networks. Ideally we want to create a model that can take any Dutch or English word as input, and gives a list of one or several words from the other language that are likely to mean the same. To evaluate the performance of our model, we will compare its output with other existing models that are proven to work.

## Research questions
A list of research questions you would like to address during the project.
- How to preprocess our data in a meaningful and helpful way?
- What is a suitable approach to making a translation model?
- How can machine learning techniques be applied to enhance our model?
- How to implement this approach into code that works with our data?
- How can we evaluate the performance of our model, in comparison to an existing translation model?

## Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show you've read the docs and are familiar with some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

## A tentative list of milestones for the project
Add here a sketch of your planning for the coming weeks. Please mention who does what.

## Documentation
This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.

## Brainstorm
Start with a pre-processing pipeline, create a base model that works without any extra grammar/language support, use grammar/language support for Dutch <-> English to improve the base model. Two models: one English-Dutch, one Dutch-English. End result: input: word in one language, output: sorted list of most likely translations in the another language.
