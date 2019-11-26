# Text Mining and Collective Intelligence Project by Kamiel Fokkink, Baran Iscanli, and Vera Neplenbroek

## Building a translation model

## Abstract
The goal of this project is to create a functioning English-Dutch translation model. The model is trained on data from movie subtitles, by comparing both the English and the Dutch subtitle lines for the same movies. The exact approach with which we will build the translation model is still to be figured out. Ideally we want to create a model that can take any Dutch or English word as input, and gives a list of one or several words from the other language that are likely to mean the same. To evaluate the performance of our model, we will compare its output with other existing models that are proven to work.

## Research questions
-	How to preprocess our data in a meaningful and helpful way?
-	What is a suitable approach to making a translation model?
-	How can machine learning techniques be applied to enhance our model?
-	How to implement this approach into code that works with our data?
- How can we evaluate the performance of our model, in comparison to an existing translation model?

## Dataset
We want to use the [OpenSubtitles dataset](http://opus.nlpl.eu/OpenSubtitles-v2018.php) on translated movie subtitles. We will first divide the dataset for easier reading, then pickle it as objects. We will possibly need to filter out punctuation and very unfrequent words, in both languages. Rather than using the .tmx format, we just got the lines in the .pkl format because we don't need all the utilities offered by a .tmx extension

## A tentative list of milestones for the project
* Preprocessing
  * Chunk the dataset to smaller bits
  * Pickle as list objects
  * Filter
  * Sample the dataset
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
Since the data file is too big to be uploaded to Git, it should be downloaded [here](http://opus.nlpl.eu/download.php?f=OpenSubtitles/v2018/tmx/en-nl.tmx.gz) and put in the data folder, before running the .ipynb notebook. The notebook will assume the en-nl.tmx file is in the data folder.
