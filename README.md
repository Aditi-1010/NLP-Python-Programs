# NLP Practicals

## Description

This repository contains basic **Natural Language Processing (NLP)** practical programs implemented using **Python, NLTK, spaCy, and Regular Expressions**. These programs cover fundamental NLP techniques such as tokenization, stemming, lemmatization, stop-word removal, POS tagging, parsing, chunking, and named entity recognition.

## Objectives

* Understand the basics of Natural Language Processing.
* Perform sentence and word tokenization.
* Apply stemming and lemmatization on text.
* Remove stop words from documents.
* Perform Part-of-Speech (POS) tagging.
* Perform parsing and chunking using RegEx and spaCy.
* Identify named entities using spaCy.

## Technologies Used

* Python 3.x
* NLTK
* spaCy
* Regular Expressions (RegEx)

## Repository Structure

```text
NLP-Practicals/
│
├── 01_Tokenization.py
├── 02_Stemming_Lemmatization.py
├── 03_Stopword_Removal.py
├── 04_POS_Tagging.py
├── 05_Parsing_Chunking.py
├── 06_NER.py
│
└── README.md
```

## Programs Included

### 1. Tokenization of Sentences and Words

Demonstrates sentence and word tokenization using **NLTK and spaCy**.

### 2. Stemming and Lemmatization

Demonstrates the process of reducing words to their root or base forms using **stemming and lemmatization**.

### 3. Stop-word Removal

Removes commonly occurring words such as `the`, `is`, `a`, `and`, etc. from a document using NLTK.

### 4. Part-of-Speech (POS) Tagging

Assigns grammatical tags such as noun, verb, adjective, and adverb to words in a sentence.

### 5. Parsing and Chunking

Demonstrates phrase extraction and chunking using **Regular Expressions and spaCy**.

### 6. Named Entity Recognition (NER)

Identifies named entities such as **Person, Organization, Location, Date**, etc. from a given text using spaCy.

## How to Run

1. Install **Python 3.x**.
2. Download or clone this repository.
3. Open a terminal in the project folder.
4. Install the required libraries:

```bash
pip install nltk spacy
```

5. Download the spaCy English language model:

```bash
python -m spacy download en_core_web_sm
```

6. Run any program, for example:

```bash
python 01_Tokenization.py
```

## Sample Input

```text
Natural Language Processing is a part of AI. It helps computers understand human language.
```

## Sample Output

```text
Sentence Tokenization:
['Natural Language Processing is a part of AI.',
 'It helps computers understand human language.']

Word Tokenization:
['Natural', 'Language', 'Processing', 'is', 'a', 'part', 'of', 'AI', ...]
```

## Learning Outcomes

After completing these practicals, the learner will be able to:

* Understand basic NLP preprocessing techniques.
* Tokenize text into sentences and words.
* Perform stemming and lemmatization.
* Remove stop words from text.
* Perform POS tagging.
* Extract phrases using chunking.
* Identify named entities using NER.

## Author

**Your Name**

B.Tech CSE (AI)
