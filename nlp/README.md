# Natural Language Processing

## Index
1. [Text Processing Pipeline](#text-processing-pipeline)
1. [Part Of Speech Tagging](#part-of-speech-tagging)

---

## Text Processing Pipeline

The typical text processing pipeline converts a dirty natural language text into a sequence of normalized tokens which can be used for further analysis. The process has the following steps:
- **Capturing text**: from files, webs, data bases,...
- **Cleaning**: the target of this step is to obtain plain text (removing HTML tags, etc)
- **Normalization**:
  + Case normalization: change all letters to lowercase
  + Punctuation removal: remove all punctuation
- **Tokenization**: split the text in tokens. Typically words, but could be sentences, letters,...
- **Stop word removal**: remove very common words with low quantity of information. Stop words are project dependent!
- **Part Of Speech (POS) tagging**: tag each word with its part of speech (noun, verb,...). This may help in the process of understanding the text, point out the relationship between words, disambiguate sentences and recognize cross references.
- **Named Entity Recognition**: recognizing entities (persons, organizations, countries,...) in our text to gain understanding about what is being said.
- **Stemming and Lemmatization**: useful to further normalize our tokens, so that different variations and modifications of words with similar meaning are considered the same. Usually, lemmatization is done before stemming, as it is more "intelligent" and its results can be used as input for the stemming process.

**Implementation**  
A Python implementation of this complete (basic) process can be found in [this notebook](https://github.com/josealberto-arcos-sanchez/data-science-knowledge/blob/master/NLP/text_processing.ipynb).

---

## Part Of Speech Tagging
TODO
