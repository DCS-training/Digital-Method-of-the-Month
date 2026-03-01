# Digital Method of the Month 
## Machine Learning
**Date**: 04/03/2026
### Author: Somya Iqbal

Schedule & itinerary:
> - Brief introduction
> - Feedback from attendees on goals and directions
> - Talk covering the main branches of ML and related use cases
> - Demonstration of simulated neural network and functions for classification task.
> - Q & A

## Introduction

In in the 1940s Alan Turing suggested that machines could ***learn***. Developing algorithms to implement this form of learning was not introduced until the 1950s with experiments training programms to learn and play games like chess. The process for developing these learning instances were further advanced and applied Backgammon & GO. One of the functional everyday applications of ML is the categorisation of emails spam/not spam using classification algorithms.

Early development of artificial neural networks from foundational neuroscience research surrounding how neurons in the brain operate were introduced to the computing fields. The idea was to add layered inputs and outputs to simulate learning, via the connections between inputs in the artificial neurons, for what the output should be and adding weights to these neural connections. These models would then represent simple functions for learning. The algorithms for tuning parameters like weights, and connections then led to considerations for building upon these linear functions to multi-layered networks, thereby increasing number of neurons, learning rates, and minimising error and loss. 

The history and development of machine learning from early statistical inference frameworks for higher level representations of learning, training features, through symbolic representations to rule based inductions give a lot of weight to the advanced methodologies available under the AI umbrella today.

### Vocabulary & key terms

[Tom Mitchell - Glossary of ML terms - hyperlink to pdf](https://link.springer.com/content/pdf/10.1023/A:1017181826899.pdf)

- Features
- Output/target
- Recall
- Precision

There are overlaps and also differences in terminology between statistical domains and ML.

> ## Task (T), Performance (P) & Evaluation (E)

## Supervised ML - Labelled data

Here we have a dataset we use for input, but have desired output category, this is where labels come in. We would like our model to learn the mappings from data and be able to categorise by class/group and predict. Labels are therefore the target outcomes you want the model to predict with new data (categorical or numerical).

#### **Regression**
> Predicting continuous values
- Linear regression, Random forest, Decision tree (regression), k-nearest neighbours, neural networks, Bayesian networks.
#### **Classification** 
> predicting a category or class
- Logistic regression, Decision trees, Random forest, support vector machines, KNN, neural networks.

Typically the way a supervised ML workflow would be applied would include (Example):
1. Define research question
2. Data collection
3. Annotation (labels)
4. Feature representation
5. TRain/Test split
6. Model selection
7. Evaluation
8. Interpretation & secondary validations from domain

## Unsupervised ML - Non labelled data

A notable difference in unsupervised methods is no label on the input data. The goal is to find latent structures. Finding relationships in data structures without a measured output can be useful for identifying clusters, dimensions, trajectories and components.

- **Clustering**
-- grouping similar items
-> PCA (Principal Component Analysis), K-means, DBSCAN, hierarchical clustering
- **Dimension reduction** -- reducing the number of features
- **Association learning** -- discovering rules in the data
- **Visualisation** -- UMAP, t-sne

## Reinforcement Learning

Learning through mediums such as reward - another neuroscience foundation.

## Use cases

Discussion: When do you need ML as opposed to traditional statistical methods?
- Hypothesis testing
- Classification of groups
- Feature generation/extraction
- Dataset alignment
- Match scoring

## Limitations and quandaries

- Overfitting
- Underfitting
- Training & test data
- Small datasets & high variances

### A lens on neural networks

-  Demo: [Neural Playground - visual environment](https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.36040&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false)

### Unsupervised methods - A simulated view
Simulated PCA, UMAP, T-SNE 
- Demo: [Embedding projector- visual environment](https://projector.tensorflow.org/)

## Further applied learning
>- [Keras workbook via Tensorflow - classification task](https://www.tensorflow.org/tutorials/keras/classification)
>- [Scikit-learn examples and guide](https://scikit-learn.org/stable/index.html)


## Further reading 
- Hastie, Tibshirani, Friedman, "The Elements of Statistical Learning", Springer, 2001.
>Reinforcement learning
- Reinforcement Learning: Theory & Algorithms by Agarwal, Jiang, Kakade & Sun
- Reinforcement Learning: An Introduction by Sutton & Barto
> Feature selection
- H. Liu, H. Motoda (2008). Computational Methods of Feature Selection.Chapman
and Hall/CRC
-  H. Liu, H. Motoda (1998). Feature Selection for Knowledge Discovery and
Data Mining. Kluwer Academic Publishers.
- Y. Saeys, I. Inza, P. Larrañaga (2007). A review of feature selection techniques
in bioinformatics. Bioinformatics, 23(19), 2507-2517.
> Bayesian networks
 - Neapolitan, R.E. (2004) Learning Bayesian Networks. Prentice Hall.
-  Castillo, E., Gutiérrez, J.M., Hadi, A.S. (1997) Expert Systems and
Probabilistic Network Models. Springer.
-  Koller, D., Friedman, N. (2009) Probabilistic Graphical Models. Principles and
Techniques. MIT Press.
- F. Jensen, T. Nielsen (2007) Bayesian Networks and Decision Graphs.
Springer.
- Sucar, E. (2015) Probabilistic Graphical Models. Principles and Applications.
Springer.



[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)