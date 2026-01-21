# Digital Method of the Month

## Descriptive and inferential statistics

## 23-01-26

### Today's schedule

-   10:00-10:05 Housekeeping

-   10:05-10:10 Brief introduction to the method and how we are going to structure the session

-   10:10-10:25 Round of Presentation of the attendees and brief intro of those who said they would be happy to talk

-   10:25-10:50 discussion using this document

-   10:50-11:00 discuss available resources, way forwards and wrapping up

## Introduction

**Statistics** is the discipline that concerns the collection, organization, analysis, interpretation, and presentation of data. Statistics is widely used in scientific disciplines and more and more often in Humanities and Social sciences. However, the difference in the datasets and questions typically part of the latter research calls for some additional caution on using it. Broadly statistics can be divided into two main branches **Descriptive Statistics** and **Inferential Statistics.**

### Key Concepts for today

-   [Descriptive Statistics](https://www.investopedia.com/terms/d/descriptive_statistics.asp)

    -   Descriptive statistics are used to summarize a given data set. This can either be a representation of the entire population or a sample of a population.

    -   Descriptive statistics are broken down into measures of central tendency and measures of variability (spread). Measures of central tendency include the mean, median, and mode.

    -   Measures of variability include standard deviation, variance, minimum and maximum variables, [kurtosis](https://www.investopedia.com/terms/k/kurtosis.asp), and [skewness](https://www.investopedia.com/terms/s/skewness.asp).

-   [Inferential Statistics](https://conjointly.com/kb/inferential-statistics/)

    -   *Inferential statistics* is used to suggest explanations for a situation or phenomenon.

    -   It allows for conclusions based on extrapolations, and so is fundamentally different from descriptive statistics.

    -   Note that inferential statistics usually suggest but cannot absolutely prove an explanation or cause-and-effect relationship.

    -   Often inferential statistics help to draw conclusions about an entire population by looking at only a sample of the population.

    -   Inferential statistics often involves estimation and hypothesis testing.

## Time

-   How much will it take to learn?
-   Is it possible to self-learn?

## Easy Pitfalls

-   Not knowing your dataset well
-   Making sure your data is tidy and easy to use (https://vita.had.co.nz/papers/tidy-data.pdf).
-   [Know your sample size expectations](https://quantitudepod.org/s4e13-power/) - Do you have the power?
-   [What to do with a small sample - Is it always a problem?](https://quantitudepod.org/s2e25-options-for-small-samples/)
-   [What to do with missing data?](https://quantitudepod.org/s4e08-craig-enders/). The [Naniar](https://naniar.njtierney.com/) R package is an amazing tool for visualising and understanding the potential implications of missing data.
-   Not having a pre-set of questions - beware of accidental p-hacking/cherry picking.
-   [Know the limitations of p values](https://www.youtube.com/watch?v=42QuXLucH3Q) 
-   Statistical significance vs meaningful significance.
-   Not knowing the limitation of the method/dataset, e.g. many tests works on normally distributed, independent samples.
-   Working with Likert measures.
-   [Reporting conventions](https://apastyle.apa.org/style-grammar-guidelines/tables-figures).
-   [Correlation is not always causation](https://www.tylervigen.com/spurious-correlations) (But it can be sometimes!)
-   Beware the Simpon's paradox! When looking at correlations with population groups, we can sometimes find that the correlation can simulataenously be positive and negative. Both are correct, we just need to make sure the analysis aligns with the research question. (https://en.wikipedia.org/wiki/Simpson%27s_paradox).
-   Always visualise your analysis - numbers alone do not tell us the full story. The [datasaurus visualisation](https://jumpingrivers.github.io/datasauRus/) nicely demonstrates 12 very different datasets which happen to have identical means, standard deviations, and correlation coefficients.
-   Getting overwhelmed on whether I need a t-test, ANOVA or regression... They are all forms of general linear models, and will give the same output from a different perspectives (<https://lindeloev.github.io/tests-as-linear/>). 

## Software

Depending on the type of analysis you are going to conduct, there are different software you can use to facilitate it

-   Excel (not a good idea, but if you need to calculate summarising stats quickly, it will be easy to use)
-   [SPSS](https://en.wikipedia.org/wiki/SPSS) (Easier interface - but will misspecify categorical variables as numeric for regression analyses)
-   [JASP](https://jasp-stats.org/) An open source graphic user interface for conducting statistics. Think of SPSS, but free, and with greater access to contemporary analyses, and less annoying to use.
-   [R and R Studio](https://bookdown.org/mikemahoney218/LectureBook/basic-statistics-using-r.html)
-   [Python and SciPy](https://en.wikipedia.org/wiki/SciPy)

## Training

-   [Data Analysis Workflow Design](https://www.cdcs.ed.ac.uk/events/data-analysis-workflow-design) 02 Feb 2026, 14:00-17:00
-   [Good Data Visualisation with R](https://www.cdcs.ed.ac.uk/events/good-data-visualisation-with-R) 06 Feb 2026, 10:00-12:00; 13 Feb 2026, 10:00-12:00
-   [Getting Started with Data Analaysis in Python](https://www.cdcs.ed.ac.uk/events/getting-started-with-data-analysis-in-python) 18 Feb 2026, 14:00-16:00, 25 Feb 2026, 14:00 - 16:00
-   [Digital Method of the Month: Machine Learning](https://www.cdcs.ed.ac.uk/events/DMM-machine-learning-2026) 04 Mar 2026, 15:00-16:00
-   [A Gentle Introduction to Causal Inference](https://www.cdcs.ed.ac.uk/events/a-gentle-introduction-to-causal-inference) 5 Mar 2026, 14:00–16:00; 12 Mar 2026, 14:00–16:00
-   [Foundations of Mahine Learning](https://www.cdcs.ed.ac.uk/events/foundations-of-machine-learning) 6 Mar 2026, 10:00–12:00; 13 Mar 2026, 10:00–12:00
-   [Digital Method of the Month: Organising Data via Databases](https://www.cdcs.ed.ac.uk/events/digital-method-month-organising-data-databases) 30 Mar 2026, 14:00–15:00
-   [Getting Started with Regression in R](https://www.cdcs.ed.ac.uk/events/getting-started-with-regression-in-R) 15 Apr 2026, 10:00–12:00; 22 Apr 2026, 10:00–12:00
-   [Getting Started with Bayesian Statistics](https://www.cdcs.ed.ac.uk/events/getting-started-with-bayesian-statistics) 21 Apr 2026, 14:00–16:00; 28 Apr 2026, 14:00–16:00
-   [Linear Mixed Effects Modelling](https://www.cdcs.ed.ac.uk/events/linear-mixed-effects-modelling) 29 Apr 2026, 10:00–12:00; 6 May 2026, 10:00–12:00; 13 May 2026, 10:00–12:00
-   [Explainable Machine Learning (XAI)](https://www.cdcs.ed.ac.uk/events/explainable-machine-learning-XAI) 1 May 2026, 10:00–12:00; 8 May 2026, 10:00–12:00

### Self-learning and External courses

Material and online courses on statistics are many. Here is a small selection to help you kick off.

-   <https://quantitudepod.org/> - My favourite geeky podcast. Full of gems on statistical analyses and navigating academic careers. The syllabus section is particularly helpfull, and each episode from season 2 onwards will contain a very useful reading list.
-   <https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw> - Stat Quest with John Starmer. Fantastic youtube channel that explains in an easy way complex statistical concepts)
-   <https://www.youtube.com/@very-normal> - Very Normal Statistics. Another fantastic youtube resource with provides both explainers and deep dives on statistics in an accesible and entertaining manner.
-   <https://hiss-r-resources.shinyapps.io/game/> An app Rhys Davies designed to help you understand regressions and interaction effects with interactive plots.
-   <https://www.linkedin.com/learning/r-statistics-essential-training> -  Linkedin R training to help you get started​​​​
-   <[http://www.sthda.com/english/wiki/descriptive-statistics-and-graphics](https://www.sthda.com/english/wiki/descriptive-statistics-and-graphics)>​​
-   <https://www.coursera.org/specializations/statistics>
-   <https://learningstatisticswithr.com/>
-   <https://online-learning.harvard.edu/course/statistics-and-r?delta=0>
-   <http://edinbr.org/>
-   <https://bookdown.org/mikemahoney218/LectureBook/basic-statistics-using-r.html>
-   <https://cran.r-project.org/doc/contrib/Verzani-SimpleR.pdf>
-   <https://daviddalpiaz.github.io/appliedstats/applied_statistics.pdf>

## Feedback

- <https://forms.office.com/r/YYNrqvuNr8>

## Additional Resources

R Studio will enable you to perform statistical analyses on your data. The following paragraphs and links will help you get an introductory overview of the main concepts and tools available for performing statistical analyses in R.

### Descriptive Statistics

**Central Tendency and Measure of Dispersions**

-   <http://statistics-help-for-students.com/What_are_measures_of_central_tendency_and_dispersion.htm#.Xsqyf2gzbIU>
-   <https://derangedphysiology.com/main/cicm-primary-exam/required-reading/research-methods-and-statistics/Chapter%203.0.2/variability-dispersion-and-central-tendency>
-   <https://us.sagepub.com/sites/default/files/upm-assets/43350_book_item_43350.pdf>
-   <https://rcompanion.org/handbook/C_02.html>
-   <https://towardsdatascience.com/descriptive-statistics-in-r-8e1cad20bf3a>
-   <http://www.sthda.com/english/wiki/descriptive-statistics-and-graphics>
-   <https://www.youtube.com/watch?v=BiLIcCtXmm0>
-   <https://www.youtube.com/watch?v=SzZ6GpcfoQY>

**Type of Distributions**

-   <https://en.wikipedia.org/wiki/List_of_probability_distributions>
-   <https://www.cyclismo.org/tutorial/R/probability.html>
-   <https://www.stat.umn.edu/geyer/old/5101/rlook.html>

**Correct your dataset Outliers and Skewed distribution**

-   <https://www.linkedin.com/learning/r-statistics-essential-training/transforming-variables?autoplay=true&u=50251009>

### Inferential Statistics

An open-source and fully-reproducible electronic textbook for teaching statistical inference using tidyverse data science tools. <https://moderndive.com/>

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

Corrections

**Bonferroni**

-   <https://www.statisticssolutions.com/bonferroni-correction/>
-   <https://rcompanion.org/rcompanion/f_01.html>
-   <https://rviews.rstudio.com/2019/10/02/multiple-hypothesis-testing/>

**Tuckey**

-   <https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/TukeyHSD>
-   <https://rpubs.com/aaronsc32/post-hoc-analysis-tukey>
-   <https://www.r-bloggers.com/anova-and-tukeys-test-on-r/>

**Comparison**

-   <https://www.researchgate.net/post/Which_post_hoc_test_is_better_Tukey_HSD_or_Bonfferoni>

**Student T test**

-   <http://www.sthda.com/english/wiki/one-sample-t-test-in-r>

-   <https://statistics.berkeley.edu/computing/r-t-tests>

-   <https://www.statmethods.net/stats/ttest.html>

-   <https://www.youtube.com/watch?v=pTmLQvMM-1M>

-   <https://www.youtube.com/watch?v=NF5_btOaCig>

-   <https://www.linkedin.com/learning/r-statistics-essential-training/comparing-means-with-the-t-test?autoplay=true&u=50251009>

**Anova Test**

-   <http://www.sthda.com/english/wiki/one-way-anova-test-in-r>

-   <https://www.datanovia.com/en/lessons/anova-in-r/>

-   <https://www.r-bloggers.com/performing-anova-test-in-r-results-and-interpretation/>

-   <https://www.scribbr.com/statistics/anova-in-r/>

-   <https://www.youtube.com/watch?v=NF5_btOaCig>

-   <https://www.youtube.com/watch?v=fT2No3Io72g>

-   <https://www.linkedin.com/learning/r-statistics-essential-training/comparing-means-with-a-two-factor-anova?autoplay=true&u=50251009>

**Chi Squared Test**

-   <http://www.sthda.com/english/wiki/chi-square-test-of-independence-in-r>

-   <https://www.r-bloggers.com/chi-squared-test/>

-   <https://towardsdatascience.com/chi-square-test-of-independence-in-r-c109947ca73a>

-   <https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/chisq.test>

**Kolmogorov-Smirnof test**

-   <https://stat.ethz.ch/R-manual/R-devel/library/stats/html/ks.test.html>
-   <https://stats.stackexchange.com/questions/222294/understanding-kolmogorov-smirnov-test-in-r>
-   <https://en.wikipedia.org/wiki/Kolmogorov%E2%80%93Smirnov_test>

**Correlation**

-   <https://www.statmethods.net/stats/correlations.html>

-   <https://en.wikipedia.org/wiki/Correlation_and_dependence>

-   If you want to have some fun learning how to eyeballing the correlation between 2 variables here is a nice website to play with [http://guessthecorrelation.com/](https://www.datanovia.com/en/blog/cluster-analysis-in-r-practical-guide/)

-   <https://www.linkedin.com/learning/r-statistics-essential-training/calculating-correlation?autoplay=true&u=50251009>

**Linear Regression**

-   <https://www.youtube.com/watch?v=66z_MRwtFJM>

-   <http://r-statistics.co/Linear-Regression.html>

-   [Simple linear regression](http://www.sthda.com/english/articles/40-regression-analysis/167-simple-linear-regression-in-r/)

**Other Type of Regressions**

-   [Bivariate regression](https://www.linkedin.com/learning/r-statistics-essential-training/computing-a-bivariate-regression?autoplay=true&u=50251009)

-   [Multiple regression](https://www.linkedin.com/learning/r-statistics-essential-training/computing-a-multiple-regression?autoplay=true&u=50251009)

-   [Poisson regression](https://www.dataquest.io/blog/tutorial-poisson-regression-in-r/)

-   [SEM](http://lavaan.ugent.be/tutorial/tutorial.pdf)

**PCA**

-   <http://www.sthda.com/english/articles/31-principal-component-methods-in-r-practical-guide/118-principal-component-analysis-in-r-prcomp-vs-princomp/>
-   <https://cran.r-project.org/web/packages/ggfortify/vignettes/plot_pca.html>
-   <https://towardsdatascience.com/principal-component-analysis-pca-101-using-r-361f4c53a9ff>
-   <https://www.linkedin.com/learning/r-statistics-essential-training/conducting-a-principal-components-factor-analysis?autoplay=true&u=50251009>
-   <https://www.youtube.com/watch?v=FgakZw6K1QQ&t=985s>
-   <https://www.youtube.com/watch?v=0Jp4gsfOLMs>

**Cluster Analysis**

-   <https://en.wikipedia.org/wiki/Cluster_analysis>

-   <https://www.statmethods.net/advstats/cluster.html>

-   <https://www.datanovia.com/en/blog/cluster-analysis-in-r-practical-guide/>

-   <https://www.datanovia.com/en/blog/types-of-clustering-methods-overview-and-quick-start-r-code>

-   <http://girke.bioinformatics.ucr.edu/GEN242/pages/mydoc/Rclustering.html>

-   <https://www.linkedin.com/learning/r-statistics-essential-training/conducting-a-cluster-analysis?autoplay=true&u=50251009>

**K-Means**

-   <https://www.youtube.com/watch?v=4b5d3muPQmA>
-   <https://www.youtube.com/watch?v=tkAJT8gWBSY>
-   <https://www.datanovia.com/en/lessons/k-means-clustering-in-r-algorith-and-practical-examples/>
-   <https://www.datacamp.com/community/tutorials/k-means-clustering-r>
-   <https://uc-r.github.io/kmeans_clustering>

**Hierarchical clustering**

-   <https://cran.r-project.org/web/packages/dendextend/vignettes/Cluster_Analysis.html>
-   <https://rpubs.com/markloessi/499252>
-   <https://www.datacamp.com/community/tutorials/hierarchical-clustering-R>
-   <https://www.youtube.com/watch?v=7xHsRkOdVwo>
-   <https://www.youtube.com/watch?v=tkAJT8gWBSY>

**Discriminant analysis**

-   <http://www.sthda.com/english/articles/36-classification-methods-essentials/146-discriminant-analysis-essentials-in-r/>

-   <https://www.r-bloggers.com/discriminant-analysis-statistics-all-the-way/>

-   <https://www.statmethods.net/advstats/discriminant.html>

-   <https://rpubs.com/Nolan/298913>

-   <https://www.youtube.com/watch?v=r-AQxb1_BKA>


