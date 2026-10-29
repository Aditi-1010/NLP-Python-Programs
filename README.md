# NLP Practicals 📚

This repository contains a collection of **32 Natural Language Processing (NLP) practicals** implemented using Python and popular NLP and machine learning libraries.

The practicals cover a wide range of concepts, from basic text preprocessing and numerical representation to word embeddings, text classification, sentiment analysis, topic modeling, transformer models, information extraction, and document processing.

---

## 🎯 Objectives

The main objectives of these practicals are:

- To understand the fundamentals of Natural Language Processing.
- To perform sentence and word tokenization.
- To apply stemming, lemmatization, and stop-word removal.
- To perform Part-of-Speech (POS) tagging, parsing, and chunking.
- To identify named entities and resolve coreferences.
- To represent text using Bag of Words (BoW), TF-IDF, and N-grams.
- To understand word embeddings using Word2Vec and GloVe.
- To calculate text similarity using cosine similarity and Word Mover's Distance.
- To perform text classification using Naïve Bayes and SVM.
- To perform sentiment analysis and opinion mining.
- To discover hidden topics using LDA and LSA.
- To understand RNN, LSTM, and attention mechanisms.
- To apply transformer models such as BERT, GPT-2, BART, and T5.
- To perform machine translation and text summarization.
- To develop a basic chatbot using a pre-trained transformer.
- To perform document classification, separation, and boundary detection.

---

## 🛠️ Technologies Used

| Technology / Library | Purpose |
|---|---|
| Python 3.x | Main programming language |
| NLTK | Tokenization, stemming, lemmatization, POS tagging, and n-grams |
| spaCy | Parsing, chunking, NER, and information extraction |
| Regular Expressions | Pattern matching and rule-based processing |
| Scikit-learn | BoW, TF-IDF, classification, cosine similarity, and LSA |
| Gensim | Word2Vec, topic modeling, and WMD support |
| GloVe | Pre-trained word embeddings |
| TextBlob | Sentiment analysis and polarity detection |
| VADER | Rule-based sentiment analysis |
| PyTorch / TensorFlow | Neural network implementations, where required |
| Hugging Face Transformers | BERT, GPT-2, BART, T5, MarianMT, and other transformer models |

The exact libraries required depend on the practical being executed.

---

## 📂 Repository Structure

The following is a suggested naming convention for organizing all 32 practicals.

```text
NLP-Python-Programs/
│
├── 01_Tokenization.py
├── 02_Stemming_Lemmatization.py
├── 03_Stopword_Removal.py
├── 04_POS_Tagging.py
├── 05_Parsing_Chunking.py
├── 06_NER_spaCy.py
├── 07_Coreference_Resolution.py
├── 08_Bag_of_Words.py
├── 09_TF_IDF_vs_BoW.py
├── 10_N_Grams.py
├── 11_Cosine_Similarity.py
├── 12_Word2Vec_Embeddings.py
├── 13_GloVe_Word_Embeddings.py
├── 14_WMD_Text_Similarity.py
├── 15_Text_Classification_TFIDF.py
├── 16_Sentiment_Analysis.py
├── 17_LDA_Topic_Modeling.py
├── 18_LSA_Topic_Modeling.py
├── 19_Opinion_Mining.py
├── 20_Information_Extraction.py
├── 21_Information_Retrieval_TFIDF.py
├── 22_RNN_LSTM_Sequence_Classification.py
├── 23_Attention_Mechanism.py
├── 24_BERT_Text_Classification.py
├── 25_BERT_GPT2_Sentence_Embeddings.py
├── 26_GPT2_Text_Generation.py
├── 27_Transformer_NER.py
├── 28_Machine_Translation_MarianMT_T5.py
├── 29_Text_Summarization_BART_T5.py
├── 30_Transformer_Chatbot.py
├── 31_Document_Classification_Separation.py
├── 32_Hybrid_Probabilistic_FSM_Boundary_Detection.py
│
└── README.md
```

**Note:** These filenames are suggested names. They should be adjusted to match the actual files in the repository.

---

## 📘 List of All 32 Practicals

| S. No. | Practical Name | CO |
|---:|---|:---:|
| 1 | Tokenization of Sentences and Words using NLTK and spaCy | CO1 |
| 2 | Stemming and Lemmatization on Sample Text | CO1 |
| 3 | Stop-word Removal from a Document | CO1 |
| 4 | Part-of-Speech (POS) Tagging of a Given Sentence | CO1 |
| 5 | Parsing and Chunking using Regex and spaCy | CO1 |
| 6 | Named Entity Recognition (NER) using spaCy | CO1 |
| 7 | Coreference Resolution using neuralcoref or a Similar Tool | CO2 |
| 8 | Bag-of-Words Vectorization and Representation | CO2 |
| 9 | TF-IDF Implementation and Comparison with BoW | CO2 |
| 10 | N-Gram Model: Unigrams, Bigrams, and Trigrams | CO2 |
| 11 | Cosine Similarity between Text Documents | CO2 |
| 12 | Word2Vec Embeddings using Gensim on a Custom Corpus | CO2 |
| 13 | GloVe Embeddings and Vector Representation | CO2 |
| 14 | Text Similarity using Word Mover's Distance (WMD) | CO2 |
| 15 | Text Classification using Naïve Bayes / SVM with TF-IDF | CO2 |
| 16 | Sentiment Analysis using TextBlob and VADER | CO2 |
| 17 | Topic Modeling using Latent Dirichlet Allocation (LDA) | CO2 |
| 18 | Topic Modeling using Latent Semantic Analysis (LSA) | CO2 |
| 19 | Opinion Mining on Product / Service Reviews Dataset | CO2 |
| 20 | Information Extraction from Structured / Unstructured Documents | CO2 |
| 21 | Information Retrieval with Ranking using TF-IDF | CO2 |
| 22 | Sequence Classification using RNN / LSTM | CO2 |
| 23 | Implementation of Attention Mechanism | CO2 |
| 24 | Fine-tuning BERT for Text Classification | CO3 |
| 25 | Sentence Embeddings using BERT and GPT-2 | CO3 |
| 26 | Text Generation using GPT-2 | CO3 |
| 27 | Named Entity Recognition using Transformers / BERT | CO3 |
| 28 | Machine Translation using MarianMT or T5 | CO3 |
| 29 | Text Summarization using BART or T5 | CO3 |
| 30 | Chatbot Development using a Pre-trained Transformer | CO3 |
| 31 | Automatic Document Classification and Separation using ML | CO3 |
| 32 | Hybrid Probabilistic and FSM-Based Sequence Modeling for Document Boundary Detection | — |

*The CO mapping for Practical 32 was not specified in the available practical details.*

---

## 🔍 Practical-Wise Overview

### Practicals 1–6: Text Preprocessing and Linguistic Analysis

These practicals introduce the basic operations required to process natural language text.

- **Tokenization:** Divides text into sentences and individual words.
- **Stemming:** Reduces words to their root-like forms.
- **Lemmatization:** Converts words into their meaningful dictionary base forms.
- **Stop-word Removal:** Removes selected common words that may not contribute useful information to a task.
- **POS Tagging:** Identifies grammatical categories such as nouns, verbs, and adjectives.
- **Parsing and Chunking:** Identifies grammatical structures and groups related words into phrases.
- **Named Entity Recognition:** Identifies entities such as people, organizations, and locations.

### Practicals 7–14: Text Representation and Similarity

These practicals focus on representing text numerically and comparing its content.

- **Coreference Resolution:** Identifies expressions that refer to the same entity.
- **Bag of Words:** Represents documents using word occurrence counts.
- **TF-IDF:** Assigns weights to words based on their importance within documents.
- **N-Grams:** Represents sequences of one or more consecutive words.
- **Cosine Similarity:** Measures the similarity between numerical vectors.
- **Word2Vec:** Learns word embeddings from a corpus.
- **GloVe:** Uses global word co-occurrence statistics to learn word vectors.
- **Word Mover's Distance:** Estimates semantic distance between documents using word embeddings.

### Practicals 15–21: Core NLP Applications

These practicals demonstrate how NLP techniques can solve real-world text-processing problems.

- **Text Classification:** Assigns predefined categories to text using machine learning.
- **Sentiment Analysis:** Determines whether text expresses positive, negative, or neutral sentiment.
- **LDA Topic Modeling:** Discovers hidden topics in a collection of documents.
- **LSA Topic Modeling:** Uses matrix factorization, commonly SVD, to identify latent semantic structures.
- **Opinion Mining:** Analyzes customer reviews and opinions.
- **Information Extraction:** Extracts useful structured information from text.
- **Information Retrieval:** Finds and ranks relevant documents based on a user query.

### Practicals 22–30: Neural Networks and Transformers

These practicals introduce neural approaches and pre-trained language models.

- **RNN and LSTM:** Process sequential data and learn relationships between sequence elements.
- **Attention Mechanism:** Assigns different importance to different input elements.
- **BERT:** Provides contextual language representations and supports classification and other NLP tasks.
- **GPT-2:** Generates text autoregressively.
- **Transformer-based NER:** Identifies named entities using transformer models.
- **Machine Translation:** Translates text between languages using sequence-to-sequence models.
- **Text Summarization:** Generates concise summaries of longer text.
- **Chatbot:** Generates conversational responses using a pre-trained model.

### Practicals 31–32: Document Processing

- **Document Classification and Separation:** Assigns documents to categories and organizes them according to predicted labels.
- **Hybrid Probabilistic and FSM-Based Boundary Detection:** Combines probabilistic decisions with a finite-state machine to identify document boundaries.

---

## ⚙️ Installation and Setup

### 1. Install Python

Install Python 3.x and verify the installation:

```bash
python --version
```

### 2. Install Common Libraries

Run the following command in your terminal:

```bash
pip install nltk spacy scikit-learn gensim textblob vaderSentiment transformers torch sentencepiece
```

Some practicals may require additional libraries depending on their implementation.

### 3. Download NLTK Resources

Run the following Python code:

```python
import nltk

nltk.download("punkt")
nltk.download("stopwords")
nltk.download("wordnet")
nltk.download("averaged_perceptron_tagger")
```

Depending on the NLTK version, additional resources may be required.

### 4. Install the spaCy English Model

Run:

```bash
python -m spacy download en_core_web_sm
```

### 5. Transformer Model Downloads

Pre-trained models such as BERT, GPT-2, BART, T5, and MarianMT may download automatically when first loaded.

An internet connection is generally required for the initial download unless the model is already available locally. Large models may require substantial RAM or GPU memory.

---

## ▶️ How to Run

Open a terminal in the repository directory and execute the required Python file.

For example:

```bash
python 01_Tokenization.py
```

Other examples:

```bash
python 09_TF_IDF_vs_BoW.py
python 15_Text_Classification_TFIDF.py
python 24_BERT_Text_Classification.py
python 29_Text_Summarization_BART_T5.py
```

Run each practical separately. The filenames used in the commands must match the actual files in the repository.

For Google Colab, install the necessary libraries in a notebook cell and execute the practical cells in order.

---

## 🧠 Concepts Covered

The 32 practicals cover the following major NLP concepts:

- **Text Preprocessing:** Tokenization, stemming, lemmatization, stop-word removal.
- **Linguistic Analysis:** POS tagging, parsing, chunking, NER, and coreference resolution.
- **Text Representation:** Bag of Words, TF-IDF, N-grams, Word2Vec, GloVe, and sentence embeddings.
- **Text Similarity:** Cosine similarity and Word Mover's Distance.
- **Machine Learning:** Naïve Bayes, SVM, text classification, and evaluation.
- **Sentiment Analysis:** TextBlob, VADER, and opinion mining.
- **Topic Modeling:** LDA and LSA.
- **Deep Learning:** RNN, LSTM, and attention mechanisms.
- **Transformers:** BERT, GPT-2, BART, T5, and MarianMT.
- **Advanced Applications:** Text generation, translation, summarization, chatbots, and transformer-based NER.
- **Document Processing:** Information extraction, classification, separation, and boundary detection.
- **Information Retrieval:** TF-IDF-based document ranking.

---

## 🎓 Learning Outcomes

After completing these practicals, learners should be able to:

- Understand the fundamentals of Natural Language Processing.
- Preprocess text using common NLP techniques.
- Analyze grammatical structures and identify named entities.
- Convert text into sparse and dense numerical representations.
- Compare documents using vector similarity and semantic distance.
- Build basic text-classification and sentiment-analysis workflows.
- Discover topics from collections of documents.
- Extract useful information from unstructured text.
- Retrieve and rank documents according to relevance.
- Understand the basic roles of RNN, LSTM, attention, and transformer models.
- Apply pre-trained models to classification, text generation, translation, summarization, and chatbot tasks.
- Understand document classification and boundary-detection workflows.

---

## 🌍 Applications of NLP

The concepts covered in these practicals are useful in applications such as:

- Chatbots and virtual assistants
- Search engines and information retrieval
- Spam detection and text classification
- Sentiment analysis of customer reviews
- Machine translation
- Automatic text summarization
- Resume and document analysis
- Question-answering systems
- Topic discovery and document organization
- Text generation and autocomplete
- Information extraction
- Document boundary detection

---

## 📌 Important Notes

- The README describes the intended coverage of 32 practicals. Ensure that the corresponding program files are present before claiming that every practical has been implemented.
- The exact implementation and dependencies may differ between practicals.
- Older packages such as `neuralcoref` may not support current spaCy versions. A compatible coreference-resolution implementation may be necessary.
- Stop-word removal is not suitable for every NLP task.
- Stemming may produce forms that are not valid dictionary words, whereas lemmatization aims to produce meaningful base forms.
- Bag of Words and TF-IDF do not inherently capture complete word order or semantic meaning.
- Word2Vec and GloVe provide word embeddings, while BERT provides contextual representations.
- Higher cosine similarity generally indicates greater vector similarity; lower WMD indicates a smaller semantic distance.
- LDA and LSA use different approaches to discover latent topics.
- Transformer models can require significant computational resources and download time.
- Never upload API keys, passwords, or other sensitive credentials to a public repository.

---

## 👩‍💻 Author

**Aditi Panwar**

B.Tech CSE (AI)

---

⭐ If you find this repository useful, consider giving it a star!
