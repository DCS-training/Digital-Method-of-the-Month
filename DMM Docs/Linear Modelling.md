# Digital Method of the Month

## Linear Modelling

## 21-01-25

### Today's schedule

-   12:00-12:05 Housekeeping

-   12:05-12:10 Brief introduction to the method and how we are going to structure the session

-   12:10-12:25 Round of Presentation of the attendees and brief intro of those who said they would be happy to talk

-   12:25-12:50 discussion using this document

-   12:50-13:00 discuss available resources, way forwards and wrapping up

## Introduction

**Linear modelling** is a statistical term to any model that assumes linearity of the data. This is commonly conducted through linear regressions, but other analysis methods such correlation analysis, mixed models, and SEM can also be used to analyse linear data.

Linear model is usually described by two parameters: the *slope* and the *y*-intercept. This can be summarised mathematically by y = the *slope*, multiplied by *x*, plus the *y-intercept*, i.e., *y = mx + b* .

These linear models can be used for a variety of reasons in analyses:

-    To test hypotheses.

-   To explore causal relationships between variables.

-   To suggest explanations for situations/phenomenons.

-   To help draw conclusions about an entire population by looking at a sample of the population.

To get an overview of linear regression and other related regression models, you may find this guide helpful: ["Regression analysis: The ultimate guide"](https://www.qualtrics.com/uk/experience-management/research/regression-analysis/).
For more in-depth understanding, check out this book: ["Analysing Data using Linear Models"](https://bookdown.org/pingapang9/linear_models_bookdown/). 


## Time

-   How much will it take to learn?
-   Is it possible to self-learn?

## Easy Pitfalls

#### Theory

-   Is your analysis reflective of the hypothesis?
-   Measurement reliability - How consistent is the measure?
-   Measurement validity - Being aware and critical of what constructs are actually being evaluated.
-   Have you accounted for the effects of confounding variables, covariates, and potential interaction terms? (i.e., beware the [Simpson's paradox](https://en.wikipedia.org/wiki/Simpson%27s_paradox)).
-   [Are you conducting a linear analysis? A mediation analysis? A moderation analysis? A moderated mediation? A moderated moderation? A mediated moderated moderation?!!!](https://afhayes.com/introduction-to-mediation-moderation-and-conditional-process-analysis.html)
-   Is your analysis theoretically and empirically justifiable?
-   Are your covariates appropriate? Beware of "collider" variables - materials on [Directed Aclyctic Graphs (DAGS)](https://pmc.ncbi.nlm.nih.gov/articles/PMC8821727/) are useful for anticipating potential theoretical issues from covariates.
-   Do you need to consider expanding on the linear model, and adopt a [structural equation modelling (SEM)](https://www.taylorfrancis.com/reader/read-online/dd855ba2-d7df-464d-b8e6-14885231a4f8/chapter/pdf?context=ubx) approach? 

#### Interpreting analyses

-   [Have you plotted your data?](https://en.wikipedia.org/wiki/Anscombe%27s_quartet)
-   [Know your sample size expectations](https://quantitudepod.org/s4e13-power/) - Do you have the power?
-   Is your analysis under powered? Is your analysis "over" powered?
-   [What to do with a small sample - Is it always a problem?](https://quantitudepod.org/s2e25-options-for-small-samples/)
-   What to do with missing data? Removing missing entries may bias your analyses under some circumstances.
-   Not having a pre-set of questions - beware of accidental p-hacking/cherry picking.
-   [Know the limitations of p values](https://www.youtube.com/watch?v=42QuXLucH3Q)
-   Statistical significance vs meaningful significance.
-   Not knowing the limitation of the method/dataset, e.g. many tests works on normally distributed, independent samples.
-   Working with Likert measures.
-   [Reporting conventions](https://apastyle.apa.org/style-grammar-guidelines/tables-figures).
-   [Correlation is not causation](https://www.tylervigen.com/spurious-correlations) (But it can be sometimes!)
-   Are your variables correctly specified? (This is a scarier issue for SPSS, as it can ignore your data labelling when using regression analysis).
-   Interpreting categorical variables and model intercepts - how to spot the ["reference"](https://www.statology.org/dummy-variables-regression/) variable, and interpret what it means. You may also need to specify your ["contrast coding"](https://stats.oarc.ucla.edu/spss/faq/coding-systems-for-categorical-variables-in-regression-analysis-2/) using a different approach.

#### Model assumptions 

-   Checking your ["model assumptions"](https://bookdown.org/pingapang9/linear_models_bookdown/chap-assumptions.html; https://people.duke.edu/~rnau/testing.html), and understanding what these mean for the interpretation of your analysis.
-   Be cautious of using statistical tests for assumptions (they are very sensitive to being either underpowered or overpowered, and so type 1 and type 2 errors will be common). Better to use visual methods of checking plots. Useful paper on the subject by [Shatz, 2023](https://link.springer.com/article/10.3758/s13428-023-02072-x).
-   I find it useful to explore why the assumption exists to understand it's implications. For example, if a t-test is used to compare the mean value of two groups, why are we assuming the data is normally distributed?
-   Main assumptions to check for in linear models:
    - Linearity of relationships 
    - Independence of residuals 
    - Normality of residuals
    - Equal variances for residuals
-    If needed, consider using a [generalised linear model](https://bookdown.org/roback/bookdown-BeyondMLR/) to address your analysis. It may help solve some issues of violated assumption.

#### Repreated measures and Linear Mixed-effects Models 

-    If you have repeated meatures, this would mean that your data are not independent. This then violates the independence of residuals assumption of simple linear regression, and as such it is inappropriate to use this method to anlayse such data. In this case, what you can do is to use linear mixed effects models.
  
-    Suppose, you want to study the effectiveness of a new drug on 5 groups of patients recruited from 5 different wards in a particular hospital over 10 weeks. You measure the effect of this drug on every individual patient every Friday, and you do this for ten weeks. Now, the data points you collect are not independent because they either come from the very same participant, or from the same ward (beling looked after by the same medics team). In other words, the data are clusterd/grouped by participants and by wards. Now you can hopefully see that such by-particiapnt individual difference and by-ward difference would have unstrcutured effects on your outcome variable (i.e., the effectiveness of the drug). You cannot ignore such grouping/clustering effects. A good way to deal with them is to include them as random effects using linear mixed effects models. Your predictor variables are included in the model as fixed effects just as how you do it when building a simple linear regression.

-   An accesible book that explains all you need to know about linear mixed effects modelling (R code provided)
     Vasishth et al. (2022) Linear Mixed Models in Linguistics and Psychology: A Comprehensive Introduction.
    (https://vasishth.github.io/Freq_CogSci/)

## Software

Depending on the type of analysis you are going to conduct, there are different software you can use to facilitate it

-   [SPSS](https://en.wikipedia.org/wiki/SPSS) (Easy interface - but will misspecify categorical variables as numeric for regression analyses)
-   [R and R Studio](https://r-statistics.co/Linear-Regression.html?utm_content=cmp-true)
-   [Python and SciPy](https://en.wikipedia.org/wiki/SciPy).
-   [AMOS](https://www.ibm.com/products/structural-equation-modeling-sem)
-   [STATA](https://www.stata.com/).

## Training

-   [Digital Method of the Month: Focus on Statistical Methods Part 3 - Simulation](https://www.cdcs.ed.ac.uk/events/digital-method-of-the-month-statistical-methods-simulation) 07 Feb 2024 12:00-13:00

-   [From SPSS to R: How to Make Your Statistical Analysis Reproducible](https://www.cdcs.ed.ac.uk/events/spss-to-r) 19 -26 Feb 2024 10:00-12:00

-   [A Gentle Introduction to Causal Inference](https://www.cdcs.ed.ac.uk/events/causal-inference) 6 Mar 2024 14:00 - 16:00.

-   [Digital Method of the Month: Machine Learning](https://www.cdcs.ed.ac.uk/events/digital-method-month-machine-learning) 05 Apr 12:00-13:00

-   [Introduction to Machine Learning with Python](https://www.cdcs.ed.ac.uk/events/intro-machine-learning-python) 08-15 Apr 14:00-16:00

-   [Interactive Analysis Reports with R Markdown](https://www.cdcs.ed.ac.uk/events/interactive-analysis-reports-r-markdown) 11 Apr 10:00-12:00

-   [Introduction to Bayesian Statistics](https://www.cdcs.ed.ac.uk/events/intro-bayesian-statistics) 17-24 Apr 14:00-16:00

-   [Null Hypothesis Testing in R](https://www.cdcs.ed.ac.uk/events/null-hypothesis-testing-r) 18-25 Apr 10:00-12:00

-   [Regression and Mixed Effects Modelling](https://www.cdcs.ed.ac.uk/events/regression-mixed-effects-modelling) 29 Apr -13 May 14:00-16:00

### Self-learning and External courses

Material and online courses on statistics are many. Here is a small selection to help you kick off.

-   <https://quantitudepod.org/> - My favourite geeky podcast. Full of gems on statistical analyses and navigating academic careers..
-   <https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw>(Fantastic youtube channel that explains in an easy way complex statistical concepts)
-   <https://www.linkedin.com/learning/r-statistics-essential-training>​
-   <https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw> ​
-   <https://rcompanion.org/handbook/C_02.html>​
-   <https://towardsdatascience.com/descriptive-statistics-in-r-8e1cad20bf3a>​
-   <http://www.sthda.com/english/wiki/descriptive-statistics-and-graphics>​
-   <https://www.youtube.com/watch?v=BiLIcCtXmm0>​
-   <https://www.youtube.com/watch?v=SzZ6GpcfoQY>​
-   <https://www.coursera.org/specializations/statistics>
-   <https://learningstatisticswithr.com/>
-   <https://online-learning.harvard.edu/course/statistics-and-r?delta=0>
-   <http://edinbr.org/>
-   <https://bookdown.org/mikemahoney218/LectureBook/basic-statistics-using-r.html>
-   <https://cran.r-project.org/doc/contrib/Verzani-SimpleR.pdf>
-   <https://daviddalpiaz.github.io/appliedstats/applied_statistics.pdf>
-   <https://bookdown.org/roback/bookdown-BeyondMLR/>
## Feedback

-   <https://forms.office.com/r/YYNrqvuNr8>

## Additional Resources

R Studio will enable you to perform statistical analyses on your data. The following paragraphs and links will help you get an introductory overview of the main concepts and tools available for performing statistical analyses in R.

**Sample, Population and Bias**

-   <https://stattrek.com/sampling/populations-and-samples.aspx>

-   <https://www.statisticssolutions.com/what-is-the-difference-between-population-and-sample/>

-   <https://www.youtube.com/watch?v=eIZD1BFfw8E>

-   <https://towardsdatascience.com/what-is-statistical-bias-and-why-is-it-so-important-in-data-science-80e02bf7a88d>

-   <https://www.dummies.com/education/math/statistics/how-to-identify-statistical-bias/>

-   <https://data36.com/statistical-bias-types-explained/>

-   <https://www.statisticshowto.com/what-is-bias/>

**Null-hypothesis significance test**

-   <https://en.wikipedia.org/wiki/Statistical_hypothesis_testing>
-   <https://data-flair.training/blogs/hypothesis-testing-in-r/>
-   <https://rcompanion.org/handbook/D_01.html>
-   <https://www.andrew.cmu.edu/user/achoulde/94842/lectures/lecture07/lecture07-94842.html>

**P-VALUE**

-   <https://www.youtube.com/watch?v=5Z9OIYA8He8>
-   <https://www.youtube.com/watch?v=vemZtEM63GY>
-   <https://www.youtube.com/watch?v=KEofcJ1tfkI>

**Correlation**

-   <https://www.statmethods.net/stats/correlations.html>

-   <https://en.wikipedia.org/wiki/Correlation_and_dependence>

-   If you want to have some fun learning how to eyeballing the correlation between 2 variables here is a nice website to play with [http://guessthecorrelation.com/](http://guessthecorrelation.com/).

-   <https://www.linkedin.com/learning/r-statistics-essential-training/calculating-correlation?autoplay=true&u=50251009>

**Linear Regression**

-   <https://www.youtube.com/watch?v=66z_MRwtFJM>

-   <http://r-statistics.co/Linear-Regression.html>

-   [Simple linear regression](http://www.sthda.com/english/articles/40-regression-analysis/167-simple-linear-regression-in-r/)

**Linear Mixed Regression**
 - <https://vasishth.github.io/Freq_CogSci/> 
 
**Other Type of Regressions**

-   [Bivariate regression](https://www.linkedin.com/learning/r-statistics-essential-training/computing-a-bivariate-regression?autoplay=true&u=50251009)

-   [Multiple regression](https://www.linkedin.com/learning/r-statistics-essential-training/computing-a-multiple-regression?autoplay=true&u=50251009)

-   [Poisson regression](https://www.dataquest.io/blog/tutorial-poisson-regression-in-r/)

-   [SEM](http://lavaan.ugent.be/tutorial/tutorial.pdf)
