# Named Entity Recognition

Named Entity Recognition (NER) is the task of locating named entity mentions in unstructured text and classifying them into pre-defined categories, such as person names, organizations, locations, etc.; but does not identify which specific entity it is.

Different Natural Language Processing libraries in Python to apply NER models to texts are considered, and also different online tools.

## Flair
[Flair](https://github.com/zalandoresearch/flair) is a powerful Natural Language Processing library developed by Zalando Research that allows to apply different NLP models to text, in particular NER models.

There is one model that was trained over the English CoNLL-03 dataset, and it can recognize 4 different entity types:
1.	Person (PER)
2.	Localization (LOC)
3.	Organization (ORG)
4.	Miscellaneous (MISC)

These labels count with some prefixes: Single (S), Begin (B), End (E) and Inside (I), which appears depending on if single word entities or compound words entities are found.


There is another model trained over the Ontonotes dataset, and it can recognize 16 different entity types:
1.	Person (PERSON)
2.	Organization (ORG)
3.	Countries, cities, states (GPE)
4.	Other locations not included in the previous type (LOC)
5.	Facilities (FAC)
6.	Cardinal numbers (CARDINAL)
7.	Titles of books, songs, etc (WORK_OF_ART)
8.	Dates or periods (DATE)
9.	Vehicles, foods, etc. (PRODUCT)
10.	Any named language (LANGUAGE)
11.	Nationalities or religious or political groups (NORP)
12.	Sport events, wars, etc. (EVENT)
13.	Ordinal numbers (ORDINAL)
14.	Named documents made into laws (LAW)
15.	Measurements, as of weight or distance (QUANTITY)
16.	Times smaller than a day (TIME)


## spaCy

[spaCy](https://spacy.io/) is a free open-source library for Natural Language Processing in Python. It features NER, among others.
We applied two different models. Both are an English multi-task CNN trained on OntoNotes, but the second one with GloVe vectors trained on Common Crawl.
