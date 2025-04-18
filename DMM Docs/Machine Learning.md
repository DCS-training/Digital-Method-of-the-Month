# Digital Method of the Month 
## Machine Learning

**Date**: 7th April 2025

**Hosted By**: Chris Oldnall

## Today's Schedule

**13:00&ndash;13:05**: Housekeeping.

**13:05&ndash;13:10**: Brief introduction to machine learning and how we are going to structure the session.

**13:10&ndash;13:25**: Attendee introductions &ndash; what is your interest in and experience with machine learning?

**13:25&ndash;13:50**: Machine learning in practice.

**13:50&ndash;14:00**: Signposting to available resources and wrapping up.

## Introduction

What is machine learning?
Machine learning is the process of using data to "train" a model to perform based on the patterns found in the data. There are various different types of methods used for model training, and the methods used differ if you are doing supervised or unsupervised learning (defined below). Machine learning is popular as a method these days because it is more efficient and less expensive to train and maintain machine learning models than it is to maintain rule-based systems. The use of machine learning has also enabled people to learn patterns that they would not have otherwise seen in the data, enabling insights from application areas that previously were not as well understood. These methods have been popularized by the increasing availability of data.

## Key concepts

### Supervised Learning
When we have a set of data, we typically have a very clear idea of what we want to use it for. Typically this is either understanding the relationship between two variables, or to use it to determine the output of some outcome when given a load of new data without the outcome. For supervised learning we need complete sets of data (with both predictors and outcome) and can do one of two things:
- Regression --> typically involves predicting a value
- Classification --> typically involves putting things into set categories
  
Process:
- Find your data and prepare it so that it is in the right format for models.
- Split data into training data and testing data. Some people might say train, test, and evaluation split is needed. The sets of data used for evaluation/testing should be kept separate - in a "lockbox" so to speak. Important to avoid "leakage".
- Select your model. Many different methods are used for supervised learning, including simpler models such as decision trees, logistic regression and more complex models such as neural networks. Some "ensemble" methods combine multiple model types to improve model performance.
- Evaluate model performance, based on a set of standard metrics, including accuracy (%of correct predictions). Other evaluation metrics include precision (# of true positives/total # of positives), and recall (true positives/true positives + false negatives). Good to also evaluate on the impact on certain subgroups of the population, to ensure that the model is not worse at predicting certain groups than others.

### Unsupervised Learning
Looking for patterns in the data, without an idea of what we are looking for yet. Clustering methods are popular here.

### Limitations of Machine Learning
- The things "learned" by models could be based on completely spurious correlations. It is sometimes difficult to figure out which features were used by the model. Methods like feature importance exist but are imperfect.
- The datasets used for machine learning are often flawed and not representative of the whole population. Many contain errors as well, which if not caught, could lead to very misleading results!
- Supervised learning depends on having labeled data for the training process. This is not always easy to come by. Many people in the computer vision community use pretrained models for this reason. But the models are often trained on completely different data/images than the context we are interested in. This can lead to so-so results.
- Ethical problems arise if machine learning decisions are used as a justification for arrest, or other consequential actions. Particularly if model accuracy is worse for certain groups.

## The way forward 

### CDCS Courses:
- [Introduction to Machine Learning](https://www.cdcs.ed.ac.uk/events/introduction-machine-learning25))
- [Advanced Uses of LLMs](https://www.cdcs.ed.ac.uk/events/advanced-uses-llm)


### Books:

- AIQ: How artificial intelligence works and how we can harness its power for a better world, James Scott and Nicholas Polson.
- Artificial Intelligence: A Modern Approach, Stuart Russell and Peter Norvig
- Life 3.0: Being Human in the Age of Artificial Intelligence, Max Tegmark

### Academic papers:
- [1] Timnit Gebru, Jamie Morgenstern, Briana Vecchione, Jennifer Wortman Vaughan, Hanna Wallach, Hal Daumé III, and Kate Crawford. 2021. Datasheets for Datasets. DOI:https://doi.org/10.48550/arXiv.1803.09010
- [2] Margaret Mitchell, Simone Wu, Andrew Zaldivar, Parker Barnes, Lucy Vasserman, Ben Hutchinson, Elena Spitzer, Inioluwa Deborah Raji, and Timnit Gebru. 2019. Model Cards for Model Reporting. In Proceedings of the Conference on Fairness, Accountability, and Transparency, 220–229. DOI:https://doi.org/10.1145/3287560.3287596
- [3] Inioluwa Deborah Raji, Emily M. Bender, Amandalynne Paullada, Emily Denton, and Alex Hanna. 2021. AI and the Everything in the Whole Wide World Benchmark. Retrieved February 7, 2023 from http://arxiv.org/abs/2111.15366
- [4] Michael A. Lones. 2022. How to avoid machine learning pitfalls: a guide for academic researchers. DOI:https://doi.org/10.48550/arXiv.2108.02497

### Newspaper articles:

- In general any query in Google News &quot;machine learning \&lt;\&lt;your topic of interest\&gt;\&gt; would likely return an interesting reading.

- [The Economist explains - How machine learning works | The Economist explains | The Economist](https://www.economist.com/the-economist-explains/2015/05/13/how-machine-learning-works)
- [Unshackled algorithms - Machine-learning promises to shake up large swathes of finance | Finance &amp; economics | The Economist](https://www.economist.com/finance-and-economics/2017/05/25/machine-learning-promises-to-shake-up-large-swathes-of-finance)
- [Machine learning - Of prediction and policy | Finance &amp; economics | The Economist](https://www.economist.com/finance-and-economics/2016/08/20/of-prediction-and-policy)
- [The shape of things to come - How do proteins fold? | Science &amp; technology | The Economist](https://www.economist.com/science-and-technology/2020/11/30/how-do-proteins-fold)
- [Daily chart - A study finds nearly half of jobs are vulnerable to automation | Graphic detail | The Economist](https://www.economist.com/graphic-detail/2018/04/24/a-study-finds-nearly-half-of-jobs-are-vulnerable-to-automation)

### Videos:

- [Barack Obama: Intro to Deep Learning | MIT 6.S191 - YouTube](https://www.youtube.com/watch?v=l82PxsKHxYc)
- [AlphaGo - The Movie | Full Documentary - YouTube](https://www.youtube.com/watch?v=WXuK6gekU1Y)
- [DeepMind StarCraft II Demonstration - YouTube](https://www.youtube.com/watch?v=cUTMhmVh1qs)

### Courses:

- [Machine Learning with Python: A Practical Introduction | edX](https://www.edx.org/course/machine-learning-with-python-a-practical-introduct)
- [Machine Learning for Everyone | DataCamp](https://learn.datacamp.com/courses/introduction-to-machine-learning-with-r)

[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)

## Author List
### Latest Author: Christopher A Oldnall
### Previous Contributors: E. Martorell Toledano, Bhargavi Ganesh

