# **Digital Method of the Month: Text Analysis**

28 January 2021

## Author: Lucy Havens (lucy.havens@ed.ac.uk)

## **Schedule**

12:00 Housekeeping (5 minutes)

12:05 Overview of this text analysis session (5 minutes)

12:10 Attendee introductions and presentations from those who volunteered (15 minutes)

12:25 Text Analysis (25 minutes)

12:50 Wrap up (10 minutes)

**\*\*\***

## **What is text analysis?**

Word frequencies

Sentence segmentation

Collacates – words that occur in close proximity to one another

Information extraction

Part-of-speech tagging

Named entity recognition – to find people, places, organizations, etc.

Relation extraction – to find relationships among entities

Event extraction – to find events that entities participate in

Classification

Sentiment analysis

Topic modeling

Word embeddings – to study meanings, how meanings change over time

##**Why would I use text analysis?**

To summarize HUGE amounts of text – &quot;distant reading&quot;

To study the evolution of an author&#39;s vocabulary throughout their publication history

To understand how positively/neutrally/negatively people are writing book reviews

To identify places named in a text or _corpus_ (collection of texts)

##**How can I do text analysis?**

3 main steps: (1) data preparation, (2) standardization, (3) analysis

2 main approaches: (A) use out-of-the-box tools, (B) customize existing tools to your needs

[**AntConc**](http://www.laurenceanthony.net/software/antconc/)- a user interface for text analysis that doesn&#39;t require any coding (with many of the capabilities you&#39;ll find in RegEx and Python NLTK), also open source

James Baker, Rossitza Atanassova, Andrew Salway (2020). Computational Analysis of Catalogue Data (Version v2021.01.21). [https://cataloguelegacies.github.io/antconc.github.io/](https://cataloguelegacies.github.io/antconc.github.io/)

**Python** and Regular Expressions ( **RegEx** ) for simple queries (word counts, dataset size)

[Pythex](https://pythex.org/)

[The Programming Historian tutorials](https://programminghistorian.org/en/lessons/?topic=python)

Python&#39;s **NLTK** is a popular text analysis library with many online resources, and it&#39;s open source (free!)

Alex, Beatrice and Llewellyn, Clare. (2020) _Library Carpentry: Text &amp; Data Mining_. Centre for Data, Culture &amp; Society, University of Edinburgh. [http://librarycarpentry.org/lc-tdm/](http://librarycarpentry.org/lc-tdm/).

You can write Python code using...

**Jupyter Notebooks** – becoming popular among digital humanists and in the GLAM sector

[NLS Data Foundry Tools: Jupyter Notebooks](https://data.nls.uk/tools/jupyter-notebooks/) – introductions to NLTK in Jupyter Notebooks using text from the National Library of Scotland&#39;s digitized collections

[GLAM Workbench](https://glam-workbench.github.io/) – introductions to using Python Jupyter Notebooks with data from galleries, libraries, archives, and museums

**IDEs** (Integrated Development Environments) – for example, Atom

See [The Programming Historian tutorials to get started](https://programminghistorian.org/en/lessons/?search=integrated+development+environment)

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

##**Additional Resources**

LinkedIn Learning - available to all University staff and students from MyEd portal

[W3Schools Tutorials](https://www.w3schools.com/)

[Stack Overflow](https://stackoverflow.com/)

##**Reading**

Havens, Lucy. (2020) [_Exploring Collections as Data with Jupyter Notebooks_](https://data.nls.uk/projects/exploring-collections-as-data-with-jupyter-notebooks/). National Library of Scotland Data Foundry.

Lang, Anouk. [_Word Embeddings: A Very Short Introduction_](https://aelang.github.io/word-embeddings). Digital textualities | semantic cartographies | networked geographies.

Tweedie, Brett. [_We Are What We Steal_](https://dxlab.sl.nsw.gov.au/we-are-what-we-steal/). The State Library of New South Wales and DX Lab.

Bird, Steven and Klein, Ewan and Loper, Edward. (2019) _Natural Language Processing with Python – Analyzing Text with the Natural Language Toolkit_. O&#39;Reilly Media. 978-0-596-51649-9. [https://www.nltk.org/book/](https://www.nltk.org/book/).

Alex, Beatrice. (2020)[_Geoparsing English Language Text with the Edinburgh Geoparser_](https://programminghistorian.org/en/lessons/geoparsing-text-with-edinburgh). The Programming Historian.

\*\*\*

Any questions? Thank you for joining today! Please let us know how you found the session [here](https://forms.office.com/Pages/ResponsePage.aspx?id=sAafLmkWiUWHiRCgaTTcYbJksOTKjv5Nsdenk5ny0NNUMFhOVkFOSE9IUkdUTjRTM0Q2RlJNSTFNTy4u)!
