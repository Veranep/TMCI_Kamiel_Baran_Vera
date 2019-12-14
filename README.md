# Text Mining and Collective Intelligence Project by Kamiel Fokkink, Baran Iscanli, and Vera Neplenbroek

## Building a translation model

## Abstract
The goal of this project is to create a functioning English-Dutch translation model. The data set contains English and Dutch translations of the same movie subtitles, which will be connected in the translation model to build the translator. The model consists of two Recurrent Neural Networks, an Encoder and a Decoder, which will transform the English input sentence to a tensor, and then to a Dutch output sentence. It is based on a PyTorch implementation, but extended by reversing the input sentences, and using different data formats. Evaluation will be done using the BLEU measure, giving each translated Dutch sentence/text a score out of 1, based on how much it corresponds to the target sentence/text.

## Research questions
-	How to preprocess our data in a meaningful and helpful way?
-	What is a suitable approach to making a translation model?
-	How can machine learning techniques be applied to train our model?
-	How to implement this approach into code that works with our data?
- 	How can we evaluate the performance of our model?

## Dataset
We used the [OpenSubtitles dataset](http://opus.nlpl.eu/OpenSubtitles-v2018.php) on translated movie subtitles. It consists of 3GB of English Dutch sentence pairs. But we did not use the whole dataset, due to the long training time. We filtered the sentence pairs to be no longer than 15 words, and the English sentence starting with [I, you, he, she, it, we, they] followed by [is, are, am, have, has, were, had] for less grammatical variance and more focused training. 20% of these filtered sentence pairs were reserved for training.

## A final list of milestones for the project
* Preprocessing
  * Chunk into bits and pickle the dataset as list objects (Baran)
  * Filtering on grammatical structure (Baran)
* Making the model
  * Research into which kind of models and approaches exist (Kamiel)
  * Implement the Sequence to Sequence Network code from [Pytorch]( https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html) (Kamiel)
  * Find a few ways to alter and enhance this standard model (Vera)
  * Training the model over our data (Baran and Vera)
* Evaluating
  * Find a suitable evaluation measure for translation (Vera)
  * Implement it in code (Vera)
* Writing the report
  * Introduction, the model, discussion, conclusion (Kamiel)
  * Preprocessing and dataset (Baran)
  * Tweaks to the model, evaluation (Vera)

## Documentation
Since the data file is too big to be uploaded to Git, it can be downloaded [here](http://opus.nlpl.eu/download.php?f=OpenSubtitles/v2018/tmx/en-nl.tmx.gz).
Our repository contains two ipython notebooks. One contains all the code to read in, preprocess and filter the data. The other contains the bulk of the code, with the basis code to create the translation model, the enhancements that we implemented, commands to perform the training, and evaluation.
