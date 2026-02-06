# **Digital Method of the Month: Text Analysis**

An introduction to text analysis tools, formats and considerations

9 February 2026

Edinburgh Futures Institute 

Alex Crest. Archaeology PhD Researcher


## **Schedule**

12:00 Housekeeping and Introductions

12:05 Overview of this text analysis session (5 minutes)

12:10 Text analysis (45 minutes)

12:55 Wrap up (5 minutes)


## **What is quantitative text analysis?**

The computational exploration of language and linguistic features in textual data.

This can include assigning numerical values to texts that gauge sentiment, to understanding common words and phrases and bundling these into topics, to detecting associated terms that occur alongside a common key term to see how meaning changes in different contexts.


## **Why would I use text analysis?**

To answer specific research questions

These can be data orientated:
1. What themes occur in customer reviews associated with the Samsung Series 5/8 Washing Machine?
2. What issues do politicians emphasise at Prime Ministers Questions?
3. What concerns appear most often in patient feedback?

Also broader, where the data is analysed for more detailed work:
1. What are the heritage values of the Antonine Wall in different social, spatial and digital contexts?
Sub research questions:
    What attachments do different communities have with different places? 
		How are these expressed? (As a Google Maps Local Guide, on Social          Media?)
		What are the mechanisms through which values develop?

To summarize HUGE amounts of text 

To study the evolution of an author&#39;s vocabulary throughout their publication history

To study the differences in vocabulary or concepts in different groups of texts

To understand how positively/neutrally/negatively people are writing book reviews or discussing certain topics

To identify places or organizations named in a dataset or _corpus_ (collection of texts)

To extract certain types of information from a dataset

To examine patterns in a text or corpus

To target more in-depth analysis

Datasets can be _structured_ or _unstructured_:

-Structured data contains an observable organisational pattern (e.g. could be stored in a spreadsheet or database: multiple choice survey results, library metadata, census data)

-Unstructured data does not (digitised novels by Jane Austen, transcribed interviews, open-ended survey results)


## **Some common text analysis methods:**

Word/n-gram frequencies 
- more information [here](https://medium.com/the-data-nudge/nlp-basics-what-are-n-grams-e60cb125a758)
- Google Books [ngram viewer](https://books.google.com/ngrams/)
- N-Gram = common word coocurences e.g. a trigram "Walk the dog"

Sentence segmentation : seperating indivudal sentences

Collacates – words that occur in close proximity to one another
- more information [here](https://books.google.com/ngrams/)

Information extraction

Part-of-speech tagging
- some info [here](https://nlp.stanford.edu/software/tagger.shtml)
- try it [here](https://parts-of-speech.info/)

Named entity recognition – to find people, places, organizations, etc.
- read more [here](https://www.turing.com/kb/a-comprehensive-guide-to-named-entity-recognition)

Relation extraction – to find relationships among entities

Event extraction – to find events that entities participate in

Key word extraction

Classification

Sentiment analysis – to estimate positivity or negativity. 
- There are many different types e.g. lexicon-based, rule based etc.

Topic modelling
- video introduction/examples [here](https://www.youtube.com/watch?v=IUAHUEy1V0Q)

Clustering

<img width="925" height="602" alt="image" src="https://github.com/user-attachments/assets/38d6ecd1-7e16-4b2b-9f3e-e62295ceaefd" />
(Sievert and Shirley, 2014, 69)

Word embeddings – to study meanings, how meanings change over time

Large language model (LLM) and generative AI (GenAI) approaches

Crucially: Research your methods, learn their technicity (their operating function) and critically apply them to match your data and questions.


## **How can I do text analysis?**

3 main steps: 

(1) data preparation

(2) standardisation

(3) analysis

2 main approaches: 

(A) use out-of-the-box tools

(B) customise existing tools for your needs

Before beginning, it is important to familiarise yourself with the vocabulary, including:

**Tokens** : words, numbers, punctuation that are tokenised (they become represented by a number or digited in a matrix)

**Stopwords** : commonly appearing words often considered to be 'filler' or irrelevant (e.g. 'it', 'an', 'the', 'he', 'she'), that are removed before text analysis occurs to reduce 'noise'

**Concordances** : lists of a particular word in its usage contexts across a corpus ( I ran **home** from work ; **home** is where the heart is ; We built our **home** together).

**Stems** : root form of a word that may not be a word itself (**read** reader, reading, unread; **dict** predict, dictionary, verdict)

**Lemmas** : root form of a word that is itself a word: The dictionary version.

Decide how much time you need or can spend cleaning your text (data)


**What are important considerations when doing text analysis?**

Keep in mind that you may need to format your text in different ways for the different questions you&#39;re investigating.

For example: lowercasing (or &quot;casefolding&quot;) all words is useful when calculating word frequencies, but not when tagging parts of speech

If your text has been digitized using OCR (optical character recognition) or HRT (handwriting recognition technology), it WILL NOT be a perfect copy of the physical text, unless someone has manually reviewed and corrected the digitized text.

If your text is in multiple languages, you may need different models for each of them (ie. different lemmatizers, different NER models)

If your text has been scraped from the internet, in particular social media, you may have web-specific features to deal with, such as URLs, DOIs, hashtags, emojis, images, and references to other users. You should consider whether these have value for your research project and how they should be treated.

Figure out the optimal method to answer your research questions or meet the objectives of your project, and what you’re trying to measure. Are you focused on words, entities, topics, etc.?

Figure out how to present the results of your data. 

Common preprocessing pipelines include cleaning, stopword removal (often using a standard list), stemming and/or lemmatizing. However, depending upon your research question, some (or all) of these preprocessing steps might not be suitable. 




## **A note on LLMs/GenAI**

The emergence of LLMs/GenAI has opened more opportunities for researchers to employ text analysis methods in their research. However, these technologies can introduce a variety of ethical and legal risks and are typically more costly – computationally, environmentally, and financially – than other text analysis methods. Additionally, because these technologies are so new, there are limited 'real-world' examples of humanities and social science projects employing LLMs and GenAI-based methods.

Three common appraoches to analysing text using LLMs/GenAI include:

a) creating a retrieval augmented generation (RAG) system to query a datast

b) exploring a dataset by interacting with LLMs through chatbot interfaces or the command line

c) adjusting LLMs through fine tuning to improve their ability to perform a specific type of analysis or interpret a specific type of dataset

While we won't be discussing LLMs and GenAI in detail today, we have linked some resources at the end of this file if you're interested in learning more.




## **Tools and resources**

[**Voyant Tools**](https://voyant-tools.org/) - a beginner-friendly online platform for basic visualisations 

[**AntConc**](http://www.laurenceanthony.net/software/antconc/)- a user interface for text analysis that doesn&#39;t require any coding (with many of the capabilities you&#39;ll find in RegEx and Python NLTK), also open source

James Baker, Rossitza Atanassova, Andrew Salway (2020). Computational Analysis of Catalogue Data (Version v2021.01.21). [https://cataloguelegacies.github.io/antconc.github.io/](https://cataloguelegacies.github.io/antconc.github.io/)

[**LancsBox**](https://lancsbox.lancs.ac.uk/) - software platform for text analysis developed by Lancaster University

[**Gale Digital Scholar Lab**](https://library.ed.ac.uk/finding-resources/library-databases/database-includes/includes-g/gale-digital-scholar-lab) - platform for text analysis of Gale's primary sources

Tools from media labs, such as the [Digital Methods Initiative, University of Amsterdam](https://wiki.digitalmethods.net/Dmi/ToolDatabase) or the [SciencesPo MediaLab]( https://medialab.sciencespo.fr/outils/) 

**Python**, **R***, and Regular Expressions ( **RegEx** ) for simple queries (word counts, dataset size)

[Pythex](https://pythex.org/) - a web platform for testing regular expressions 

[The Programming Historian tutorials](https://programminghistorian.org/en/lessons/?topic=python)

Python&#39;s Natural Language Toolkit (**NLTK**) is a popular text analysis library with many online resources, and it&#39;s open source (free!) There are also libraries like spaCy and Gensim which are usable alongside NLTK for many advanced text processing operations, such as topic modelling and NER.

R&#39;s **QUANTEDA** (Quantitative Analysis of Textual Data) is a popular text analysis package for R users, which has a variety of models and sample corpora built in for text analysis.

Alex, Beatrice and Llewellyn, Clare. (2020) _Library Carpentry: Text &amp; Data Mining_. Centre for Data, Culture &amp; Society, University of Edinburgh. [http://librarycarpentry.org/lc-tdm/](http://librarycarpentry.org/lc-tdm/).8

You can write Python and R code using...

**Jupyter Notebooks** – becoming popular among digital humanists and in the GLAM sector

[NLS Data Foundry Tools: Jupyter Notebooks](https://data.nls.uk/tools/jupyter-notebooks/) – introductions to NLTK in Jupyter Notebooks using text from the National Library of Scotland&#39;s digitized collections

[GLAM Workbench](https://glam-workbench.github.io/) – introductions to using Python Jupyter Notebooks with data from galleries, libraries, archives, and museums

**IDEs** (Integrated Development Environments) – for example, Atom, RStudio (for R), PyCharm (for Python), Anaconda

See [The Programming Historian tutorials to get started](https://programminghistorian.org/en/lessons/?search=integrated+development+environment)

The University of Edinburgh also runs [Notaeble](https://noteable.edina.ac.uk/), allowing students and staff members to run code in Jupyter notebooks and R studio.

[**Visual Studio Code**](https://code.visualstudio.com/) - an open-source code editor for a variety of languages including Python, JavaScript, and C++

[**Anaconda**](https://www.anaconda.com/) - an open-scource set of libraries in R and Python; suitable for advanced text analysis using AI and machine learning

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

Törnberg, Petter. (2024). [_How to use LLMs for Text Analysis_](https://arxiv.org/abs/2307.13106). arXiv (preprint)

Nielbo, Kristoffer L., et al. (2024). [_Quantiative text analysis_](https://doi.org/10.1038/s43586-024-00302-w). 

Bonacchi, C., et al. (2024). [Political uses of the ancient past on social media are predominantly negative and extreme](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0308919).

Goodale, Ian. (2024). [_Analyzing Multilingual French and Russian Text using NLTK, spaCy, and Stanza._](https://programminghistorian.org/en/lessons/analyzing-multilingual-text-nltk-spacy-stanza) The Programming Historian.

Rebora, Simone. (2023). [Sentiment Analysis in Literary Studies. A Critical Survey.](https://www.digitalhumanities.org/dhq/vol/17/2/000691/000691.html)

Havens, Lucy. (2020). [_Exploring Collections as Data with Jupyter Notebooks_](https://data.nls.uk/projects/exploring-collections-as-data-with-jupyter-notebooks/). National Library of Scotland Data Foundry.

Tweedie, Brett. [_We Are What We Steal_](https://theconversation.com/we-are-what-we-steal-the-new-south-wales-police-gazette-and-charting-histories-of-crime-131140). The State Library of New South Wales and DX Lab.

Bird, Steven and Klein, Ewan and Loper, Edward. (2019). [_Natural Language Processing with Python – Analyzing Text with the Natural Language Toolkit._](https://www.nltk.org/book/](https://www.nltk.org/book/).

Alex, Beatrice. (2020). [_Geoparsing English Language Text with the Edinburgh Geoparser_](https://programminghistorian.org/en/lessons/geoparsing-text-with-edinburgh). The Programming Historian.

Silge, Julia and Robinson, David. [_Tidy Text Mining with R._](https://www.tidytextmining.com/index.html)

Sievert, C., & Shirley, K. (2014, June). LDAvis: A method for visualizing and interpreting topics. In Proceedings of the workshop on interactive language learning, visualization, and interfaces (pp. 63-70).


## **upcoming training**
- Keep up with our training programme for 2025/2026 [here](https://www.cdcs.ed.ac.uk/training)



## **CDCS past training resources**
- [Python intermediate Courses (2020)](https://github.com/DCS-training/python-interm)
- [CDCS Summer School (2021)](https://github.com/DCS-training/CDCS-Summer-School) Notebooks on Text analysis and Neteworking Analysis 
- [Introduction to text analysis](https://github.com/DCS-training/IntroToTextAnalysis)
- [Further Text analysis](https://github.com/DCS-training/FurtherTextAnalysis)
- [Edina Introduction to sentiment analysis ](https://learn.edina.ac.uk/sentiment/)
- [Webscraping News sites](https://github.com/DCS-training/WebscrapingNewsitesWithPython)

## Authors: Alex Crest (Alex.Hiscock@ed.ac.uk), Lucy Havens (lucy.havens@ed.ac.uk), James Besse (James.Besse@ed.ac.uk), Jessica Witte (jessica.wite@ed.ac.uk)  

Any questions? Thank you for joining today! Please let us know how you found the session [here](https://forms.office.com/r/pfqHFYqvfS)!


[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)
