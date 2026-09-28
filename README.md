# NLP Practicals 📚

This repository contains a collection of basic **Natural Language Processing (NLP)** practical programs implemented using **Python, NLTK, spaCy, Regular Expressions (RegEx), and Scikit-learn**.

The practicals cover important NLP concepts such as:

- Tokenization
- Stemming
- Lemmatization
- Stop-word Removal
- Part-of-Speech (POS) Tagging
- Parsing
- Chunking
- Named Entity Recognition (NER)
- Bag of Words (BoW)
- TF-IDF
- N-Grams

These programs are designed to provide a basic understanding of how computers process, analyze, and represent human language.

---

# 🎯 Objectives

The main objectives of these practicals are:

- To understand the fundamentals of Natural Language Processing.
- To perform sentence and word tokenization.
- To understand stemming and lemmatization.
- To remove unnecessary stop words from text.
- To perform Part-of-Speech (POS) tagging.
- To understand parsing and chunking.
- To identify important entities from text using Named Entity Recognition.
- To understand Bag of Words representation.
- To convert text into numerical vectors.
- To understand Term Frequency and Inverse Document Frequency.
- To apply TF-IDF to text documents.
- To generate unigrams, bigrams, and trigrams.
- To gain practical experience with NLTK, spaCy, RegEx, and Scikit-learn.

---

# 🛠️ Technologies Used

### Python 3.x
Programming language used to implement all practicals.

### NLTK
Used for:

- Tokenization
- Stemming
- Lemmatization
- Stop-word removal
- POS tagging
- Chunking
- N-Grams

### spaCy
Used for:

- Tokenization
- POS tagging
- Chunking
- Named Entity Recognition

### Regular Expressions (RegEx)
Used for:

- Pattern-based parsing
- Chunking
- Text pattern matching

### Scikit-learn
Used for:

- Bag of Words
- TF-IDF
- Numerical representation of text

---

# 📂 Repository Structure

```text
NLP-Python-Programs/
│
├── 01_Tokenization.py
├── 02_Stemming_Lemmatization.py
├── 03_Stopword_Removal.py
├── 04_POS_Tagging.py
├── 05_Parsing_Chunking.py
├── 06_NER.py
├── 07_Bag_of_Words.py
├── 08_TF_IDF.py
├── 09_N_Grams.py
│
└── README.md

1️⃣ Tokenization of Sentences and Words
File:
01_Tokenization.py

🔹 What is Tokenization?
Tokenization is the process of breaking a piece of text into smaller units called tokens.

Tokens can be:

Sentences

Words

Punctuation marks

For example:

NLP is interesting. It is used in AI.

Sentence tokenization produces:

NLP is interesting.
It is used in AI.

Word tokenization produces individual words such as:

NLP
is
interesting
It
is
used
in
AI

🔹 What does the program do?
This practical demonstrates:

Sentence tokenization using NLTK.

Word tokenization using NLTK.

Sentence and word tokenization using spaCy.

🔹 Important Functions/Concepts
sent_tokenize() – Splits text into sentences.

word_tokenize() – Splits text into words and punctuation.

spacy.load() – Loads a spaCy language model.

doc.sents – Provides sentences identified by spaCy.

doc – Contains processed tokens from the input text.

🔹 Example
Input:

Natural Language Processing is a part of AI. It helps computers understand human language.

Output:

Sentence Tokenization:
Natural Language Processing is a part of AI.
It helps computers understand human language.

Word Tokenization:
Natural
Language
Processing
is
a
part
of
AI
...

💡 Key Learning
Tokenization is generally one of the first steps of NLP preprocessing because later NLP operations often work on individual sentences and words.

2️⃣ Stemming and Lemmatization
File:
02_Stemming_Lemmatization.py

🔹 What is Stemming?
Stemming reduces a word to its root-like form by removing prefixes or suffixes.

Examples:

playing  → play
played   → play
studies  → studi

The result produced by stemming may not always be a valid English word.

🔹 What is Lemmatization?
Lemmatization converts a word into its meaningful base or dictionary form, called a lemma.

Examples:

running  → run
better   → good
studies  → study

Unlike stemming, lemmatization generally produces a meaningful word.

🔹 What does the program do?
The practical:

Takes words or a sentence as input.

Applies a stemming algorithm.

Applies lemmatization.

Displays the results for comparison.

🔹 Important Functions/Concepts
PorterStemmer() – Performs Porter stemming.

WordNetLemmatizer() – Performs lemmatization using WordNet.

stem() – Returns the stemmed form.

lemmatize() – Returns the lemma/base form.

🔹 Example
Word	Stemming	Lemmatization
playing	play	playing/play*
studies	studi	study
running	run	running/run*

*The exact lemmatized result can depend on the Part-of-Speech information supplied to the lemmatizer.

💡 Key Learning
Both techniques reduce variations of words to a common form, which can help NLP systems process similar words more effectively.

3️⃣ Stop-word Removal
File:
03_Stopword_Removal.py

🔹 What are Stop Words?
Stop words are commonly occurring words that often provide limited information for certain NLP tasks.

Examples include:

the
is
a
an
of
and
in
to

🔹 What does the program do?
The practical:

Takes a sentence or document as input.

Tokenizes the text into words.

Identifies commonly used stop words.

Removes those words.

Displays the filtered text.

🔹 Example
Input:

This is a simple example of Natural Language Processing.

After Stop-word Removal:

simple example Natural Language Processing

🔹 Important Functions/Concepts
stopwords.words() – Provides a list of stop words.

word_tokenize() – Converts text into individual tokens.

List comprehension – Used to filter unwanted words.

💡 Key Learning
Stop-word removal can reduce the amount of unnecessary text and may improve efficiency in some NLP applications.

Note: Stop words should not always be removed. Their importance depends on the NLP task. For example, the word "not" can be important for sentiment analysis.

4️⃣ Part-of-Speech (POS) Tagging
File:
04_POS_Tagging.py

🔹 What is POS Tagging?
Part-of-Speech tagging assigns a grammatical category to each word in a sentence.

Common POS categories include:

POS	Meaning	Example
Noun	Person, place, thing, etc.	book
Verb	Action/state	run
Adjective	Describes a noun	beautiful
Adverb	Describes a verb/adjective	quickly
Pronoun	Replaces a noun	he
Preposition	Shows relationship	in

🔹 What does the program do?
The practical:

Takes a sentence as input.

Tokenizes it into words.

Assigns a POS tag to each word.

Displays each word along with its grammatical tag.

🔹 Example
Input:

The student reads a book.

Possible output:

The      DT
student  NN
reads    VBZ
a        DT
book     NN

The exact tags depend on the tagger and sentence context.

🔹 Important Functions/Concepts
word_tokenize() – Performs word tokenization.

pos_tag() – Assigns POS tags to tokens.

POS tag set – Defines the grammatical meaning of each tag.

💡 Key Learning
POS tagging helps NLP systems understand the grammatical role of words within a sentence.

5️⃣ Parsing and Chunking
File:
05_Parsing_Chunking.py

This practical demonstrates how words can be grouped into meaningful phrases.

🔹 What is Parsing?
Parsing is the process of analyzing the grammatical structure of a sentence.

It helps identify relationships between words and phrases.

For example:

The student reads a book.

can be divided into structures such as:

Noun Phrase (NP) → The student
Verb Phrase (VP) → reads a book

🔹 What is Chunking?
Chunking groups related words into phrases based on their POS tags.

For example:

The intelligent student

can be identified as a Noun Phrase (NP).

🔹 What does the program do?
The practical demonstrates:

POS tagging of words.

Defining grammatical patterns using RegEx grammar.

Extracting phrases using NLTK chunking.

Performing phrase/chunk identification using spaCy.

🔹 Example RegEx Grammar
NP: {<DT>?<JJ>*<NN>}

This pattern can identify a noun phrase containing:

Optional determiner (DT)

Zero or more adjectives (JJ)

A noun (NN)

🔹 Important Functions/Concepts
RegexpParser() – Creates a chunk parser using grammar rules.

parse() – Applies the grammar to tagged words.

noun_chunks – spaCy feature used to identify noun phrases.

💡 Key Learning
Parsing and chunking help an NLP system understand the structure and relationships between words instead of treating every word independently.

6️⃣ Named Entity Recognition (NER)
File:
06_NER.py

🔹 What is Named Entity Recognition?
Named Entity Recognition (NER) is the process of identifying important entities in text and assigning them categories.

Common entities include:

Label	Meaning
PERSON	Person's name
ORG	Organization
GPE	Geopolitical entity/place
DATE	Date
MONEY	Monetary value
LOC	Location

🔹 What does the program do?
The practical:

Loads a pre-trained spaCy English model.

Processes the input text.

Identifies named entities.

Displays the entity text and its corresponding label.

🔹 Example
Input:

Aditi visited Microsoft in Noida on Monday.

Possible output:

Aditi     → PERSON
Microsoft → ORG
Noida     → GPE
Monday    → DATE

The exact entities recognized depend on the spaCy model and context.

🔹 Important Functions/Concepts
spacy.load() – Loads the trained NLP model.

nlp() – Processes the input text.

doc.ents – Returns recognized entities.

ent.text – Gives the entity text.

ent.label_ – Gives the entity category.

💡 Key Learning
NER is useful for extracting important information from unstructured text and is widely used in applications such as information extraction, search engines, chatbots, and document analysis.

7️⃣ Bag of Words (BoW)
File:
07_Bag_of_Words.py

🔹 What is Bag of Words?
Bag of Words (BoW) is a text representation technique that converts text documents into numerical vectors based on the occurrence of words.

It creates a vocabulary of unique words from the given documents and represents each document using the frequency of those words.

For example:

Document 1: I like NLP
Document 2: I like Python

The vocabulary can be:

I
like
NLP
Python

The documents can then be represented numerically based on word occurrence.

🔹 What does the program do?
The practical:

Takes one or more text documents as input.

Creates a vocabulary of words.

Calculates word frequencies.

Converts text into numerical vectors.

Displays the Bag of Words representation.

🔹 Important Concepts
Vocabulary

Word frequency

Document-term matrix

Numerical vector representation

💡 Key Learning
Bag of Words converts textual data into numerical form so that machine learning algorithms can process text.

8️⃣ TF-IDF
File:
08_TF_IDF.py

🔹 What is TF-IDF?
TF-IDF stands for Term Frequency–Inverse Document Frequency.

It is a text representation technique that assigns importance to words based on:

How frequently they occur in a document.

How rare they are across a collection of documents.

TF-IDF consists of two main components.

Term Frequency (TF)
Measures how frequently a word occurs in a document.

Inverse Document Frequency (IDF)
Measures how important a word is by reducing the weight of words that occur in many documents.

The TF and IDF values are combined to produce a TF-IDF score.

🔹 What does the program do?
The practical:

Takes multiple text documents.

Calculates TF-IDF values.

Converts documents into numerical vectors.

Displays the resulting TF-IDF matrix.

🔹 Important Concepts
Term Frequency

Inverse Document Frequency

TF-IDF score

TF-IDF matrix

Numerical text representation

💡 Key Learning
TF-IDF gives higher importance to words that are frequent in a particular document but less common across the entire collection.

9️⃣ N-Grams
File:
09_N_Grams.py

🔹 What are N-Grams?
An N-gram is a sequence of N consecutive words or tokens in a text.

Unigram
A unigram contains one word.

Example:

Natural
Language
Processing

Bigram
A bigram contains two consecutive words.

Example:

Natural Language
Language Processing

Trigram
A trigram contains three consecutive words.

Example:

Natural Language Processing

🔹 What does the program do?
The practical demonstrates:

Unigram generation.

Bigram generation.

Trigram generation.

Extraction of consecutive word sequences from text.

🔹 Important Concepts
Unigram

Bigram

Trigram

N-gram language representation

💡 Key Learning
N-grams help capture relationships between consecutive words and are useful in applications such as:

Language modeling

Text prediction

Autocomplete

Text analysis

Natural language generation

🔄 Overall NLP Workflow
The practicals collectively demonstrate a basic NLP workflow:

                    Input Text
                        │
                        ▼
                  Tokenization
                        │
                        ▼
        ┌───────────────┴───────────────┐
        │                               │
        ▼                               ▼
 Stemming /                     Stop-word Removal
 Lemmatization
        │                               │
        └───────────────┬───────────────┘
                        ▼
                   POS Tagging
                        │
                        ▼
                Parsing / Chunking
                        │
                        ▼
                       NER
                        │
                        ▼
              Text Representation
                        │
              ┌─────────┼─────────┐
              ▼         ▼         ▼
             BoW      TF-IDF    N-Grams

These steps do not have to be applied in exactly this order for every NLP application. The preprocessing and representation pipeline depends on the problem being solved.

⚙️ Installation and Setup
1. Install Python
Make sure Python 3.x is installed on your system.

Check the installation using:

python --version

2. Install Required Libraries
Open the terminal in the project directory and run:

pip install nltk spacy scikit-learn

3. Download Required NLTK Resources
Open Python and run:

import nltk

nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')

Depending on your NLTK version, additional resources may be required. If NLTK displays an error asking for another resource, download the resource indicated in the error message.

4. Install spaCy English Model
Run:

python -m spacy download en_core_web_sm

This model is used for practicals involving spaCy-based NLP processing.

▶️ How to Run
Open a terminal in the repository folder and run any practical using:

python 01_Tokenization.py

Similarly:

python 02_Stemming_Lemmatization.py
python 03_Stopword_Removal.py
python 04_POS_Tagging.py
python 05_Parsing_Chunking.py
python 06_NER.py
python 07_Bag_of_Words.py
python 08_TF_IDF.py
python 09_N_Grams.py

🧪 Sample Input
The following text can be used for testing several practicals:

Natural Language Processing is a part of Artificial Intelligence.
It helps computers understand and process human language.

Another sample:

Aditi is studying Computer Science and Artificial Intelligence.
She is learning Natural Language Processing using Python.

📖 Concepts Covered
Practical	Concept	Library / Tool
01	Tokenization	NLTK, spaCy
02	Stemming & Lemmatization	NLTK
03	Stop-word Removal	NLTK
04	POS Tagging	NLTK
05	Parsing & Chunking	NLTK, RegEx, spaCy
06	Named Entity Recognition	spaCy
07	Bag of Words	Scikit-learn
08	TF-IDF	Scikit-learn
09	N-Grams	NLTK

🎓 Learning Outcomes
After completing these practicals, the learner will be able to:

Understand the basic concepts of NLP.

Tokenize text into sentences and words.

Apply stemming and lemmatization.

Remove stop words from text.

Perform Part-of-Speech tagging.

Understand basic parsing and chunking.

Extract noun phrases from text.

Identify named entities using spaCy.

Understand Bag of Words representation.

Convert text into numerical vectors.

Calculate TF-IDF representations.

Generate unigrams, bigrams, and trigrams.

Understand basic NLP preprocessing and text representation.

Work with NLP libraries such as NLTK and spaCy.

Use Scikit-learn for basic text vectorization.

🚀 Applications of NLP
The concepts covered in these practicals are used in real-world applications such as:

Chatbots and virtual assistants

Search engines

Sentiment analysis

Text classification

Machine translation

Information extraction

Spam detection

Question-answering systems

Resume and document analysis

Text summarization

Autocomplete and text prediction

Document similarity

Text mining

🔑 Key NLP Concepts
This repository provides practical implementation of the following major NLP concepts:

Tokenization
     ↓
Stemming
     ↓
Lemmatization
     ↓
Stop-word Removal
     ↓
POS Tagging
     ↓
Parsing
     ↓
Chunking
     ↓
Named Entity Recognition
     ↓
Bag of Words
     ↓
TF-IDF
     ↓
N-Grams

📌 Notes
NLP preprocessing techniques should be selected according to the task.

Stop-word removal is not appropriate for every NLP application.

Stemming may produce words that are not valid dictionary words.

Lemmatization generally produces meaningful base forms but may require correct POS information for better results.

NER results depend on the trained spaCy model and the context of the input.

TF-IDF values depend on the collection of documents being analyzed.

Bag of Words does not capture word order.

N-Grams can capture limited word-order information.

👩‍💻 Author
Aditi Panwar

B.Tech CSE (AI)

**
