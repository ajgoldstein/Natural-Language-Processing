# Natural-Language-Processing
The four projects below were all part of the University of Michigan's EECS 595: Intro to Natural Language Processing. The course syllabus can be found above, along with a PDF describing each of the assignments.

## Assignments Overview

All the assignments were in written in Python, but in most cases the use of libraries like scikit-learn and NLTK were restricted and it was <b>required to implement complex functions from scratch</b>.

For each assignment, I've organized my code into <b>well-commented and easily-readable Jupyter notebooks</b>. Additionally, all the relevant files (including datasets used, .py Python scripts, and .txt result summaries) can be downloaded through each project's .zip file.

## Assignment #1
### 1) Sentence Boundary Detection
* <b>Major Task</b>: write a Python program SBD.py that detects sentence boundaries in text.

* <b>Result</b></u>: built a program that predicts if a period (.) is the end of a sentence or not with 99.2% accuracy.

### 2) Collocation Identification
* <b>Major Task</b>: write a Python program Collocations.py that identifies collocations in text.

* <b>Result</b>: built a program that implements the chi-square and the pointwise mutual information (PMI) measures of association for the identification of bigram collocations.

## Assignment #2
### 1) Language Identification Using Neural Networks
* <b>Major Task</b>: build a neural network from total scratch (no libraries allowed!) that identifies written language as English, French, or Italian.

* <b>Result</b>: designed a neural network that takes a five character text sequence and predicts the correct language with 97% accuracy.

Short explanation of my NN building process:

I started with pre-processing the train and dev data by running through their contents and storing sentences, five character sequences, and their corresponding language labels into several dictionaries. Then, using the alphabet (of length c) that I just generated, I one-hot-encoded the five character sequences into vectors (of length 5c). From here, I randomly initialized the neural network weights and proceeded forward propagate through the network layers (input —> hidden —> output). Here, I was careful to shuffle the training data so as to not overfit to any particular language. Then, after each run-through, I updated the weights through backpropogation and gradient descent. Finally, after 3 epochs I used the updated weights to make language predictions on the test data.

### 2) Hyperparameter Optimization
* <b>Major Task</b>: using at least five different sets of values for the hyperparameters  d  and  η , train the network on the training data, and see which set of hyperparameters performs best on the dev data.

* <b>Result</b>: found and evaluated the optimal hyperparameters on the test data, performing with 98% accuracy.

## Assignment #3
### 1) Part of Speech Tagging
* <b>Major Task</b>: write a Python program  Viterbi.py  that implements the Viterbi algorithm for part-of-speech tagging.
* <b>Result</b>: built a program that uses the Treebank dataset to assign words their Penn Treebank tag with 86% accuracy.

## Assignment #4
### 1) 
### List of Topics Covered
- Brief overview of English linguistics
- Text preprocessing
- Language models
- Word embeddings
- Part of speech tagging
- Syntactic parsing
- Lexical semantics
- Word sense disambiguation
- Subjectivity and sentiment analysis
- Information extraction
 - Automatic summarization
 - Question answering
 - Machine translation
 - Natural language processing for social sciences
 - Other special topics
