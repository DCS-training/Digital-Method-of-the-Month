# **Digital Method of the Month: Text Analysis**

04 December 2023

## Authors: Lucy Havens (lucy.havens@ed.ac.uk), James Besse (James.Besse@ed.ac.uk) 


## **Schedule**

12:00 Housekeeping (5 minutes)

12:05 Overview of this text analysis session (5 minutes)

12:10 Round of introductions (10-15 minutes)

12:20/25 Text Analysis

12:55 Wrap up (5 minutes)



## **What is text analysis?**

Word/n-gram frequencies

Sentence segmentation

Collacates – words that occur in close proximity to one another

Information extraction

Part-of-speech tagging

Named entity recognition – to find people, places, organizations, etc.

Relation extraction – to find relationships among entities

Event extraction – to find events that entities participate in

Classification

Sentiment analysis

Topic modelling

Word embeddings – to study meanings, how meanings change over time

## **Why would I use text analysis?**

To summarize HUGE amounts of text – &quot;distant reading&quot;

To study the evolution of an author&#39;s vocabulary throughout their publication history

To study the differences in vocabulary or concepts in different groups of texts

To understand how positively/neutrally/negatively people are writing book reviews or discussing certain topics

To identify places or organizations named in a text or _corpus_ (collection of texts)

## **How can I do text analysis?**

3 main steps: (1) data preparation, (2) standardization, (3) analysis

2 main approaches: (A) use out-of-the-box tools, (B) customize existing tools to your needs

[**AntConc**](http://www.laurenceanthony.net/software/antconc/)- a user interface for text analysis that doesn&#39;t require any coding (with many of the capabilities you&#39;ll find in RegEx and Python NLTK), also open source

James Baker, Rossitza Atanassova, Andrew Salway (2020). Computational Analysis of Catalogue Data (Version v2021.01.21). [https://cataloguelegacies.github.io/antconc.github.io/](https://cataloguelegacies.github.io/antconc.github.io/)

Tools from media labs, such as the [Digital Methods Initiative, University of Amsterdam](https://wiki.digitalmethods.net/Dmi/ToolDatabase) or the [SciencesPo MediaLab]( https://medialab.sciencespo.fr/outils/) 

**Python**, **R***, and Regular Expressions ( **RegEx** ) for simple queries (word counts, dataset size)

[Pythex](https://pythex.org/)

[The Programming Historian tutorials](https://programminghistorian.org/en/lessons/?topic=python)

Python&#39;s **NLTK** is a popular text analysis library with many online resources, and it&#39;s open source (free!) There are also libraries like spaCy and Gensim which are usable alongside NLTK for many advanced text processing operations, such as topic modelling and NER.

R&#39;s **QUANTEDA** (Quantitative Analysis of Textual Data) is a popular text analysis package for R users, which has a variety of models and sample corpora built in for text analysis.

Alex, Beatrice and Llewellyn, Clare. (2020) _Library Carpentry: Text &amp; Data Mining_. Centre for Data, Culture &amp; Society, University of Edinburgh. [http://librarycarpentry.org/lc-tdm/](http://librarycarpentry.org/lc-tdm/).8

You can write Python and R code using...

**Jupyter Notebooks** – becoming popular among digital humanists and in the GLAM sector

[NLS Data Foundry Tools: Jupyter Notebooks](https://data.nls.uk/tools/jupyter-notebooks/) – introductions to NLTK in Jupyter Notebooks using text from the National Library of Scotland&#39;s digitized collections

[GLAM Workbench](https://glam-workbench.github.io/) – introductions to using Python Jupyter Notebooks with data from galleries, libraries, archives, and museums

**IDEs** (Integrated Development Environments) – for example, Atom, R studio (for R)

See [The Programming Historian tutorials to get started](https://programminghistorian.org/en/lessons/?search=integrated+development+environment)

The University of Edinburgh also runs [Notaeble](https://noteable.edina.ac.uk/), allowing students and staff members to run code in Jupyter notebooks and R studio.


**What are important considerations when doing text analysis?**

Familiarize yourself with the vocabulary, including:

**Tokens** : words, numbers, punctuation

**Concordances** : list of a particular word in its usage contexts across a corpus

**Stems** : root form of a word that may not be a word itself

**Lemmas** : root form of a word that is itself a word

Decide how much time you need or can spend cleaning your text (data)

Keep in mind that you may need to format your text in different ways for the different questions you&#39;re investigating.

For example: lowercasing (or &quot;casefolding&quot;) all words is useful when calculating word frequencies, but not when tagging parts of speech

If your text has been digitized using OCR (optical character recognition) or HRT (handwriting recognition technology), it WILL NOT be a perfect copy of the physical text, unless someone has manually reviewed and corrected the digitized text.

If your text is in multiple languages, you may need different models for each of them (ie. different lemmatizers, different NER models)

If your text has been scraped from the internet, in particular social media, you may have web-specific features to deal with, such as URLs, DOIs, hashtags, emojis, images, and references to other users. You should consider whether these have value for your research project and how they should be treated.

Figure out the optimal method to answer your research questions or meet the objectives of your project, and what you’re trying to measure. Are you focused on words, entities, topics, etc.?

Figure out how to present the results of your data. 


## **Additional Resources**

LinkedIn Learning - available to all University staff and students from MyEd portal

[W3Schools Tutorials](https://www.w3schools.com/)

[Stack Overflow](https://stackoverflow.com/)

[R Bloggers](https://www.r-bloggers.com/)

[Digital Methods Initiative, University of Amsterdam](https://wiki.digitalmethods.net/Dmi/ToolDatabase)

[SciencesPo MediaLab]( https://medialab.sciencespo.fr/outils/) 

[Why R?](https://whyr.pl/foundation/)

[Language Technology and Data Anylysis Laboratory](https://ladal.edu.au/tutorials.html)

[Stanford Natural Language Processing Group](https://nlp.stanford.edu/)

## **Reading**

Havens, Lucy. (2020) [_Exploring Collections as Data with Jupyter Notebooks_](https://data.nls.uk/projects/exploring-collections-as-data-with-jupyter-notebooks/). National Library of Scotland Data Foundry.

Lang, Anouk. [_Word Embeddings: A Very Short Introduction_](https://aelang.github.io/word-embeddings). Digital textualities | semantic cartographies | networked geographies.

Tweedie, Brett. [_We Are What We Steal_](https://dxlab.sl.nsw.gov.au/we-are-what-we-steal/). The State Library of New South Wales and DX Lab.

Bird, Steven and Klein, Ewan and Loper, Edward. (2019) _Natural Language Processing with Python – Analyzing Text with the Natural Language Toolkit_. O&#39;Reilly Media. 978-0-596-51649-9. [https://www.nltk.org/book/](https://www.nltk.org/book/).

Alex, Beatrice. (2020)[_Geoparsing English Language Text with the Edinburgh Geoparser_](https://programminghistorian.org/en/lessons/geoparsing-text-with-edinburgh). The Programming Historian.

Silge, Julia and Robinson, David. [_Tidy Text Mining with R_](https://www.tidytextmining.com/index.html)


## **CDCS Upcoming training**
- [Advanced Text Analysis. Topic Modelling with Python](https://www.cdcs.ed.ac.uk/events/intro-topic-modelling)14/04, 21/04, 24/04
- [Silent Disco. Sentiment Analysis with Python](https://www.cdcs.ed.ac.uk/events/silent-disco-sentiment-analysis-with-python) 20/04
- [Silent Disco: Interrogating a National Narrative with GPT-2 (large-scale corpus)](https://www.cdcs.ed.ac.uk/events/silent-disco-interrogating-a-national-narrative)



## **CDCS Past training Resources**
- [Python intermediate Courses (2020)](https://github.com/DCS-training/python-interm)
- [CDCS Summer School (2021)](https://github.com/DCS-training/CDCS-Summer-School) Notebooks on Text analysis and Neteworking Analysis 
- [Introduction to text analysis](https://github.com/DCS-training/IntroToTextAnalysis)
- [Further Text analysis](https://github.com/DCS-training/FurtherTextAnalysis)
- [Edina Introduction to sentiment analysis ](https://learn.edina.ac.uk/sentiment/)
- [Webscraping News sites](https://github.com/DCS-training/WebscrapingNewsitesWithPython)



Any questions? Thank you for joining today! Please let us know how you found the session [here](https://forms.office.com/r/pfqHFYqvfS)!


[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)
