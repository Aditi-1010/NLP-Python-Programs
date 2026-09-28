# NLP Practicals 📚

This repository contains a collection of **Natural Language Processing (NLP)** practical programs implemented using **Python, NLTK, spaCy, Regular Expressions (RegEx), GloVe, Gensim, TextBlob, VADER, and Scikit-learn**.

The practicals cover important NLP concepts ranging from basic text preprocessing and representation to **word embeddings, text similarity, text classification, sentiment analysis, topic modeling, opinion mining, information extraction, and information retrieval**.

---

# 🎯 Objectives

The main objectives of these practicals are:

* To understand the fundamentals of Natural Language Processing.
* To perform sentence and word tokenization.
* To understand stemming and lemmatization.
* To remove unnecessary stop words from text.
* To perform Part-of-Speech (POS) tagging.
* To understand parsing and chunking.
* To identify important entities using Named Entity Recognition.
* To understand Bag of Words representation.
* To convert text into numerical vectors.
* To understand Term Frequency and Inverse Document Frequency.
* To apply TF-IDF to text documents.
* To generate unigrams, bigrams, and trigrams.
* To understand word embeddings using GloVe.
* To calculate text similarity using Word Mover's Distance.
* To perform text classification using Naïve Bayes and SVM.
* To perform sentiment analysis using TextBlob and VADER.
* To perform topic modeling using LDA and LSA.
* To perform opinion mining on product/service reviews.
* To extract information from structured and unstructured text.
* To build a basic information retrieval system using TF-IDF and cosine similarity.

---

# 🛠️ Technologies Used

### Python 3.x

Programming language used to implement all practicals.

### NLTK

Used for:

* Tokenization
* Stemming
* Lemmatization
* Stop-word removal
* POS tagging
* Chunking
* N-Grams
* Text preprocessing

### spaCy

Used for:

* Tokenization
* POS tagging
* Chunking
* Named Entity Recognition
* Information Extraction

### Regular Expressions (RegEx)

Used for:

* Pattern-based parsing
* Chunking
* Text pattern matching

### Scikit-learn

Used for:

* Bag of Words
* TF-IDF
* Text classification
* Naïve Bayes
* SVM
* Cosine similarity
* LSA using SVD
* Numerical representation of text

### GloVe

Used for:

* Word embeddings
* Semantic representation of words
* Word similarity
* Vector-based NLP operations

### Gensim

Used for:

* Word embeddings
* Word Mover's Distance
* Topic modeling
* LDA

### TextBlob

Used for:

* Sentiment analysis
* Polarity detection
* Subjectivity detection

### VADER

Used for:

* Sentiment analysis
* Sentiment scoring
* Positive, negative, and neutral classification

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
├── 10_GloVe_Word_Embeddings.py
│
├── 14_WMD_Text_Similarity.py
├── 15_Text_Classification_TFIDF.py
├── 16_Sentiment_Analysis.py
├── 17_LDA_Topic_Modeling.py
├── 18_LSA_Topic_Modeling.py
├── 19_Opinion_Mining.py
├── 20_Information_Extraction.py
├── 21_Information_Retrieval_TFIDF.py
│
└── README.md
```

---

# 🔟 GloVe Word Embeddings

File:

`10_GloVe_Word_Embeddings.py`

## 🔹 What is GloVe?

**GloVe (Global Vectors for Word Representation)** is a word embedding technique that represents words as numerical vectors.

It captures semantic relationships between words based on their co-occurrence statistics in a large text corpus.

For example, semantically related words such as:

```text
king
queen
man
woman
```

are represented using vectors that capture relationships between them.

## 🔹 What does the program do?

The practical:

* Loads pre-trained GloVe word vectors.
* Represents words using numerical vectors.
* Finds similar words.
* Calculates similarity between words.
* Demonstrates semantic relationships using word embeddings.

## 🔹 Important Concepts

* Word Embeddings
* Vector Representation
* Semantic Similarity
* Pre-trained Word Vectors
* GloVe

## 💡 Key Learning

GloVe converts words into dense numerical vectors that capture semantic relationships between words.

---

# 1️⃣4️⃣ Text Similarity using Word Mover's Distance (WMD)

File:

`14_WMD_Text_Similarity.py`

## 🔹 What is Word Mover's Distance?

**Word Mover's Distance (WMD)** measures the semantic distance between two documents or sentences using word embeddings.

Instead of simply comparing whether the same words occur, WMD considers the distance between the meanings of words in the embedding space.

### Important Point

```text
Lower WMD → More Similar
Higher WMD → Less Similar
```

## 🔹 What does the program do?

The practical:

* Takes two text sentences.
* Tokenizes the sentences.
* Represents words using word embeddings.
* Calculates Word Mover's Distance.
* Determines the similarity between the texts.

## 🔹 Important Concepts

* Word Embeddings
* Semantic Similarity
* Word Mover's Distance
* Vector Space
* Document Similarity

## 💡 Key Learning

WMD can measure semantic similarity even when two texts do not contain exactly the same words.

---

# 1️⃣5️⃣ Text Classification using Naïve Bayes / SVM with TF-IDF

File:

`15_Text_Classification_TFIDF.py`

## 🔹 What is Text Classification?

Text classification is the process of assigning predefined categories or labels to text.

Examples include:

* Spam / Not Spam
* Positive / Negative
* Sports / Technology
* News categories

## 🔹 TF-IDF

TF-IDF converts text into numerical vectors by assigning importance to words based on their frequency in documents.

## 🔹 Naïve Bayes

Naïve Bayes is a probabilistic machine learning algorithm commonly used for text classification.

## 🔹 SVM

Support Vector Machine (SVM) is a supervised learning algorithm that finds a decision boundary between different classes.

## 🔹 What does the program do?

The practical:

* Takes text documents and labels.
* Converts text into TF-IDF vectors.
* Splits the dataset into training and testing data.
* Trains a Naïve Bayes or SVM classifier.
* Predicts the class of test documents.
* Calculates classification accuracy.

## 🔹 Important Concepts

* TF-IDF
* Training Data
* Testing Data
* Naïve Bayes
* SVM
* Classification
* Accuracy

## 💡 Key Learning

TF-IDF provides numerical features that can be used by machine learning algorithms for text classification.

---

# 1️⃣6️⃣ Sentiment Analysis using TextBlob and VADER

File:

`16_Sentiment_Analysis.py`

## 🔹 What is Sentiment Analysis?

Sentiment analysis determines the emotional or opinion-based nature of text.

A text can generally be classified as:

```text
Positive
Negative
Neutral
```

## 🔹 TextBlob

TextBlob provides a simple way to calculate:

* Polarity
* Subjectivity

Polarity indicates whether the text is positive or negative.

Subjectivity indicates how opinion-based the text is.

## 🔹 VADER

**VADER (Valence Aware Dictionary and sEntiment Reasoner)** is a rule-based sentiment analysis tool designed particularly for text containing informal language.

It produces sentiment scores including:

* Positive
* Negative
* Neutral
* Compound

## 🔹 What does the program do?

The practical:

* Takes a text sentence as input.
* Performs sentiment analysis using TextBlob.
* Performs sentiment analysis using VADER.
* Displays sentiment scores.
* Classifies the text as positive, negative, or neutral.

## 💡 Key Learning

Sentiment analysis is widely used for analyzing opinions, reviews, feedback, and social media text.

---

# 1️⃣7️⃣ Topic Modeling using Latent Dirichlet Allocation (LDA)

File:

`17_LDA_Topic_Modeling.py`

## 🔹 What is LDA?

**Latent Dirichlet Allocation (LDA)** is an unsupervised machine learning technique used for discovering hidden topics in a collection of documents.

A document can contain multiple topics, and each topic is represented by a group of related words.

## 🔹 What does the program do?

The practical:

* Takes a collection of documents.
* Performs basic text preprocessing.
* Creates a dictionary of words.
* Creates a Bag of Words representation.
* Applies the LDA algorithm.
* Extracts hidden topics.
* Displays important words associated with each topic.

## 🔹 Important Concepts

* Topic Modeling
* Latent Topics
* Bag of Words
* Document-Topic Distribution
* Topic-Word Distribution
* LDA

## 💡 Key Learning

LDA automatically discovers hidden thematic structures within a collection of documents.

---

# 1️⃣8️⃣ Topic Modeling using Latent Semantic Analysis (LSA)

File:

`18_LSA_Topic_Modeling.py`

## 🔹 What is LSA?

**Latent Semantic Analysis (LSA)** is a technique used to discover hidden semantic relationships between terms and documents.

LSA commonly uses **Singular Value Decomposition (SVD)** to reduce the dimensionality of a document-term or TF-IDF matrix.

## 🔹 What does the program do?

The practical:

* Takes multiple documents.
* Converts documents into TF-IDF vectors.
* Applies SVD.
* Reduces the dimensionality of the text representation.
* Extracts important words associated with latent topics.

## 🔹 Important Concepts

* TF-IDF
* Singular Value Decomposition
* Dimensionality Reduction
* Latent Topics
* Semantic Relationships
* LSA

## 💡 Key Learning

LSA identifies hidden semantic structures by reducing the dimensionality of the text representation.

---

# 1️⃣9️⃣ Opinion Mining on Product/Service Reviews Dataset

File:

`19_Opinion_Mining.py`

## 🔹 What is Opinion Mining?

Opinion mining is the process of identifying opinions, attitudes, and sentiments expressed in text.

It is commonly applied to:

* Product reviews
* Customer feedback
* Service reviews
* Online comments

## 🔹 What does the program do?

The practical:

* Takes product or service reviews.
* Processes each review.
* Calculates sentiment polarity.
* Classifies reviews as positive, negative, or neutral.
* Displays the sentiment results.
* Provides a summary of sentiment distribution.

## 🔹 Example

```text
"The product is excellent"
        ↓
Positive

"The service was terrible"
        ↓
Negative
```

## 💡 Key Learning

Opinion mining helps organizations understand customer feedback and evaluate opinions about products or services.

---

# 2️⃣0️⃣ Information Extraction (IE) from Structured / Unstructured Documents

File:

`20_Information_Extraction.py`

## 🔹 What is Information Extraction?

**Information Extraction (IE)** is the process of automatically extracting useful and structured information from text.

It can identify entities such as:

* People
* Organizations
* Locations
* Dates
* Money
* Products

## 🔹 Named Entity Recognition

NER is an important component of information extraction.

For example:

```text
Aditi visited Microsoft in Noida.
```

Possible entities:

```text
Aditi      → PERSON
Microsoft  → ORG
Noida      → GPE
```

## 🔹 What does the program do?

The practical:

* Loads a pre-trained spaCy model.
* Processes an unstructured document.
* Identifies named entities.
* Extracts entity text.
* Displays entity labels.

## 🔹 Important Functions

```text
spacy.load()
nlp()
doc.ents
ent.text
ent.label_
```

## 💡 Key Learning

Information Extraction converts unstructured text into useful structured information.

---

# 2️⃣1️⃣ Information Retrieval System with Ranking using TF-IDF

File:

`21_Information_Retrieval_TFIDF.py`

## 🔹 What is Information Retrieval?

Information Retrieval (IR) is the process of finding relevant information or documents from a collection based on a user's query.

Search engines are a common real-world example of information retrieval systems.

## 🔹 TF-IDF

TF-IDF represents documents and queries as numerical vectors.

## 🔹 Cosine Similarity

Cosine similarity measures the similarity between the query vector and document vectors.

```text
Higher Similarity → More Relevant
Lower Similarity  → Less Relevant
```

## 🔹 What does the program do?

The practical:

* Stores a collection of documents.
* Takes a user query.
* Converts documents and query into TF-IDF vectors.
* Calculates cosine similarity.
* Ranks documents according to similarity.
* Displays the most relevant documents first.

## 🔹 Example

Query:

```text
machine learning artificial intelligence
```

The system calculates similarity between the query and each document and produces a ranked list.

## 🔹 Important Concepts

* Information Retrieval
* TF-IDF
* Cosine Similarity
* Query Vector
* Document Vector
* Document Ranking

## 💡 Key Learning

TF-IDF combined with cosine similarity can be used to build a basic search and document ranking system.

---

# 🔄 Overall NLP Workflow

The practicals collectively demonstrate an NLP workflow from basic preprocessing to advanced NLP applications:

```text
                     Input Text
                         │
                         ▼
                   Tokenization
                         │
                         ▼
          ┌──────────────┴──────────────┐
          │                             │
          ▼                             ▼
   Stemming /                    Stop-word Removal
   Lemmatization
          │                             │
          └──────────────┬──────────────┘
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
             ┌───────────┼───────────┐
             ▼           ▼           ▼
            BoW        TF-IDF      N-Grams
                         │
                         ▼
                  Word Embeddings
                    (GloVe)
                         │
             ┌───────────┼───────────┐
             ▼           ▼           ▼
          Similarity   Classification  Sentiment
             │           │           │
             ▼           ▼           ▼
            WMD       NB / SVM     TextBlob/VADER
                         │
                         ▼
                  Topic Modeling
                   ┌─────┴─────┐
                   ▼           ▼
                  LDA         LSA
                   │           │
                   └─────┬─────┘
                         ▼
              Information Extraction
                         │
                         ▼
              Information Retrieval
                         │
                         ▼
                  Ranked Results
```

These steps do not have to be applied in exactly this order for every NLP application. The pipeline depends on the problem being solved.

---

# ⚙️ Installation and Setup

## 1. Install Python

Make sure Python 3.x is installed on your system.

Check the installation using:

```bash
python --version
```

## 2. Install Required Libraries

Run:

```bash
pip install nltk spacy scikit-learn gensim textblob vaderSentiment
```

## 3. Download Required NLTK Resources

Run:

```python
import nltk

nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')
```

Depending on your NLTK version, additional resources may be required.

## 4. Install spaCy English Model

Run:

```bash
python -m spacy download en_core_web_sm
```

---

# ▶️ How to Run

Open a terminal in the repository folder and run any practical using:

```bash
python 01_Tokenization.py
```

Similarly:

```bash
python 02_Stemming_Lemmatization.py
python 03_Stopword_Removal.py
python 04_POS_Tagging.py
python 05_Parsing_Chunking.py
python 06_NER.py
python 07_Bag_of_Words.py
python 08_TF_IDF.py
python 09_N_Grams.py
python 10_GloVe_Word_Embeddings.py
python 14_WMD_Text_Similarity.py
python 15_Text_Classification_TFIDF.py
python 16_Sentiment_Analysis.py
python 17_LDA_Topic_Modeling.py
python 18_LSA_Topic_Modeling.py
python 19_Opinion_Mining.py
python 20_Information_Extraction.py
python 21_Information_Retrieval_TFIDF.py
```

---

# 📖 Concepts Covered

| Practical | Concept                  | Library / Tool            |
| --------- | ------------------------ | ------------------------- |
| 01        | Tokenization             | NLTK, spaCy               |
| 02        | Stemming & Lemmatization | NLTK                      |
| 03        | Stop-word Removal        | NLTK                      |
| 04        | POS Tagging              | NLTK                      |
| 05        | Parsing & Chunking       | NLTK, RegEx, spaCy        |
| 06        | Named Entity Recognition | spaCy                     |
| 07        | Bag of Words             | Scikit-learn              |
| 08        | TF-IDF                   | Scikit-learn              |
| 09        | N-Grams                  | NLTK                      |
| 10        | GloVe Word Embeddings    | GloVe                     |
| 14        | Word Mover's Distance    | Gensim                    |
| 15        | Text Classification      | TF-IDF, Naïve Bayes, SVM  |
| 16        | Sentiment Analysis       | TextBlob, VADER           |
| 17        | Topic Modeling           | LDA, Gensim               |
| 18        | Topic Modeling           | LSA, SVD, Scikit-learn    |
| 19        | Opinion Mining           | TextBlob                  |
| 20        | Information Extraction   | spaCy, NER                |
| 21        | Information Retrieval    | TF-IDF, Cosine Similarity |

---

# 🎓 Learning Outcomes

After completing these practicals, the learner will be able to:

* Understand the basic concepts of NLP.
* Tokenize text into sentences and words.
* Apply stemming and lemmatization.
* Remove stop words from text.
* Perform Part-of-Speech tagging.
* Understand parsing and chunking.
* Extract noun phrases from text.
* Identify named entities using spaCy.
* Understand Bag of Words representation.
* Convert text into numerical vectors.
* Calculate TF-IDF representations.
* Generate unigrams, bigrams, and trigrams.
* Understand word embeddings using GloVe.
* Measure semantic similarity using WMD.
* Perform text classification using Naïve Bayes and SVM.
* Perform sentiment analysis using TextBlob and VADER.
* Discover hidden topics using LDA and LSA.
* Perform opinion mining on reviews.
* Extract useful information from unstructured documents.
* Build a basic information retrieval and ranking system.
* Apply NLP concepts to practical text-processing problems.

---

# 🚀 Applications of NLP

The concepts covered in these practicals are used in real-world applications such as:

* Chatbots and virtual assistants
* Search engines
* Sentiment analysis
* Text classification
* Machine translation
* Information extraction
* Spam detection
* Question-answering systems
* Resume and document analysis
* Text summarization
* Autocomplete and text prediction
* Document similarity
* Topic discovery
* Customer review analysis
* Information retrieval
* Text mining

---

# 🔑 Key NLP Concepts

This repository provides practical implementation of the following major NLP concepts:

```text
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
     ↓
GloVe Word Embeddings
     ↓
Word Mover's Distance
     ↓
Text Classification
     ↓
Sentiment Analysis
     ↓
Topic Modeling
     ↓
Opinion Mining
     ↓
Information Extraction
     ↓
Information Retrieval
```

---

# 📌 Notes

* NLP preprocessing techniques should be selected according to the task.
* Stop-word removal is not appropriate for every NLP application.
* Stemming may produce words that are not valid dictionary words.
* Lemmatization generally produces meaningful base forms but may require correct POS information for better results.
* NER results depend on the trained spaCy model and the context of the input.
* TF-IDF values depend on the collection of documents being analyzed.
* Bag of Words does not capture word order.
* N-Grams can capture limited word-order information.
* GloVe represents words as dense numerical vectors.
* WMD uses word embeddings to measure semantic distance between texts.
* Naïve Bayes and SVM can be used for supervised text classification.
* TextBlob and VADER provide different approaches to sentiment analysis.
* LDA is a probabilistic topic modeling technique.
* LSA commonly uses SVD to identify latent semantic structures.
* Information Extraction can convert unstructured text into structured information.
* Information Retrieval systems can rank documents based on their relevance to a query.

---

# 👩‍💻 Author

**Aditi Panwar**

**B.Tech CSE (AI)**

---

⭐ If you find this repository useful, consider giving it a **star**!
