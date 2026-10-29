NLP Practicals 📚
A collection of 32 Natural Language Processing (NLP) practicals implemented using Python and popular NLP / machine-learning libraries. The practicals progress from text preprocessing and numerical representation to embeddings, classification, sentiment analysis, topic modeling, information extraction, transformer models, and document-processing applications.
Note: The filenames below are a suggested, consistent naming convention for the 32 practicals. Adjust any filename to match the actual file in your repository.

🎯 Objectives
- Learn core NLP concepts, from preprocessing to transformer-based applications.
- Represent text numerically using Bag of Words, TF-IDF, n-grams, and embeddings.
- Compare documents and measure semantic similarity.
- Build text-classification, sentiment-analysis, topic-modeling, and information-retrieval workflows.
- Explore RNN/LSTM, attention, BERT, GPT-2, and other transformer-based models.
- Apply NLP to translation, summarization, chatbots, and document organization.
🛠️ Technologies Used
Technology / Library	Purpose in the practicals
Python 3.x	Main programming language
NLTK	Tokenization, stemming, lemmatization, stop-word removal, POS tagging, n-grams
spaCy	Linguistic processing, parsing, named entity recognition, information extraction
Regular Expressions (re)	Pattern matching and rule-based chunking / boundary detection
Scikit-learn	BoW, TF-IDF, cosine similarity, classification, LSA/SVD, evaluation
Gensim	Word2Vec, topic modeling, and Word Mover's Distance support
GloVe vectors	Pre-trained word embeddings
TextBlob and VADER	Sentiment analysis
PyTorch / TensorFlow	Neural sequence models, where used
Hugging Face Transformers	BERT, GPT-2, MarianMT, BART, T5, and other transformer workflows


The exact dependencies depend on which practical you run. Some models also require downloads and may need a GPU for faster execution.
📂 Repository Structure
Use a numbered filename convention to keep all 32 practicals in order:
NLP-Python-Programs/
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
└── README.md
📘 All 32 Practicals
No.	Practical / Program	Main concepts	CO
01	Tokenization of Sentences and Words using NLTK and spaCy	Sentence and word tokenization	CO1
02	Stemming and Lemmatization on Sample Text	Stemming, lemmas, root/base forms	CO1
03	Stop-word Removal from a Document	Stop-word lists and preprocessing	CO1
04	Part-of-Speech (POS) Tagging of a Given Sentence	Grammatical categories and POS tags	CO1
05	Parsing and Chunking using Regex and spaCy	Phrase patterns, parsing, chunking	CO1
06	Named Entity Recognition (NER) using spaCy	Entity detection and entity labels	CO1
07	Coreference Resolution using neuralcoref or a Similar Tool	Linking mentions that refer to the same entity	CO2
08	Bag-of-Words (BoW) Vectorization and Representation	Vocabulary, document-term matrix, word counts	CO2
09	TF-IDF Implementation and Comparison with BoW	Term frequency, inverse document frequency, weighting	CO2
10	N-Gram Model (Unigrams, Bigrams, Trigrams) from a Corpus	N-gram generation and local word context	CO2
11	Cosine Similarity between Text Documents	Vector similarity and document comparison	CO2
12	Word2Vec Embeddings using Gensim on a Custom Corpus	CBOW / Skip-gram and dense word vectors	CO2
13	GloVe Embeddings Loading and Vector Representation	Pre-trained word vectors and semantic relationships	CO2
14	Text Similarity using Word Mover's Distance (WMD)	Embedding-based semantic distance	CO2
15	Text Classification using Naïve Bayes / SVM with TF-IDF	Supervised classification and evaluation	CO2
16	Sentiment Analysis using TextBlob and VADER	Polarity, subjectivity, sentiment scores	CO2
17	Topic Modeling using Latent Dirichlet Allocation (LDA)	Topic-word and document-topic distributions	CO2
18	Topic Modeling using Latent Semantic Analysis (LSA)	TF-IDF, SVD, latent semantic structure	CO2
19	Opinion Mining on Product / Service Reviews Dataset	Review polarity and sentiment distribution	CO2
20	Information Extraction from Structured / Unstructured Documents	Extracting entities and useful fields	CO2
21	Information Retrieval with TF-IDF Ranking	Query-document similarity and ranking	CO2
22	Sequence Classification using RNN / LSTM	Sequential data, recurrent networks, classification	CO2
23	Attention Mechanism	Attention weights and context-aware representations	CO2
24	Fine-tuning BERT for Text Classification	Pre-trained language models and task-specific fine-tuning	CO3
25	Sentence Embeddings using BERT and GPT-2	Contextual representations and embedding extraction	CO3
26	Text Generation using GPT-2	Autoregressive language modeling and decoding	CO3
27	Named Entity Recognition using Transformers / BERT	Transformer-based token classification	CO3
28	Machine Translation using MarianMT or T5 (Hugging Face)	Sequence-to-sequence translation	CO3
29	Text Summarization using BART or T5	Abstractive summarization	CO3
30	Chatbot Development using a Pre-trained Transformer (DialoGPT / ChatGPT-style)	Conversational input and generated responses	CO3
31	Automatic Document Classification and Separation using ML	Document labeling and grouping	CO3
32	Hybrid Probabilistic + FSM-Based Sequence Modeling for Document Boundary Detection	Probabilistic decisions, finite-state machines, boundary detection	—


CO mappings follow the practical list provided. No CO mapping was specified for Practical 32.
🔎 What Each Practical Covers
Practicals 01–06: Text Preprocessing and Linguistic Analysis
These introduce foundational NLP operations: splitting text into sentences and tokens, reducing words to base forms, removing stop words, identifying grammatical roles, extracting phrase chunks, and detecting named entities.
Practicals 07–14: Text Representation and Similarity
These cover coreference resolution, BoW and TF-IDF representations, n-grams, cosine similarity, Word2Vec, GloVe, and WMD. BoW and TF-IDF create sparse numerical representations, while Word2Vec and GloVe produce dense word vectors. Cosine similarity compares vectors; WMD estimates semantic distance using word embeddings.
Practicals 15–21: Core NLP Applications
These include supervised text classification, sentiment analysis, topic modeling with LDA and LSA, opinion mining, information extraction, and information retrieval. The techniques serve different purposes: classification predicts labels, topic modeling discovers themes, extraction finds structured facts, and retrieval ranks documents for a query.
Practicals 22–30: Neural Networks and Transformers
These explore sequence classification with RNN/LSTM, attention, fine-tuning BERT, sentence representations, GPT-2 text generation, transformer-based NER, translation, summarization, and chatbot development.
Practicals 31–32: Document Processing
These focus on classifying and separating documents, then combining probabilistic modeling with a finite-state machine (FSM) to detect document boundaries.
⚙️ Installation and Setup
1. Install Python
Install Python 3.x and verify it:
python --version
2. Install common dependencies
pip install nltk spacy scikit-learn gensim textblob vaderSentiment transformers torch sentencepiece
Depending on your environment, some practicals may need additional packages. For example, older neuralcoref releases may not support current spaCy versions; use a compatible coreference-resolution implementation.
3. Download common NLP resources
Run in Python:
import nltk

nltk.download("punkt")
nltk.download("stopwords")
nltk.download("wordnet")
nltk.download("averaged_perceptron_tagger")
NLTK resource names can differ across versions. If an error requests another resource, download the exact resource named in that error.
4. Install the spaCy English model
python -m spacy download en_core_web_sm
5. Model downloads
Hugging Face models such as BERT, GPT-2, BART, T5, and MarianMT are usually downloaded the first time they are loaded. Internet access is needed for the initial download unless the model is already cached locally. Large models may require substantial RAM or GPU memory.
▶️ How to Run a Practical
Open a terminal in the repository directory and run the relevant Python file. For example:
python 01_Tokenization.py
python 09_TF_IDF_vs_BoW.py
python 15_Text_Classification_TFIDF.py
python 24_BERT_Text_Classification.py
python 29_Text_Summarization_BART_T5.py
Run one practical at a time. The filename must match the actual file in your repository. If you use Google Colab, install the required packages in a notebook cell and run the practical cells in order.
🧠 Concepts Covered at a Glance
- Preprocessing: tokenization, stemming, lemmatization, stop-word removal, POS tagging, parsing, chunking
- Linguistic analysis: NER and coreference resolution
- Text representation: BoW, TF-IDF, n-grams, Word2Vec, GloVe, sentence embeddings
- Similarity and retrieval: cosine similarity, WMD, TF-IDF ranking
- Machine learning: Naïve Bayes, SVM, document classification, evaluation
- Sentiment and topics: TextBlob, VADER, opinion mining, LDA, LSA
- Deep learning: RNN, LSTM, attention
- Transformers: BERT, GPT-2, BART, T5, MarianMT, transformer-based NER and chatbots
- Document processing: information extraction, classification, separation, boundary detection
🎓 Learning Outcomes
After completing the practicals, learners should be able to:
- Preprocess text and analyze its linguistic structure.
- Convert text into sparse and dense numerical representations.
- Compare documents using vector similarity and embedding-based distance.
- Train or apply text classifiers and evaluate their outputs.
- Analyze sentiment and discover topics in collections of text.
- Extract entities and retrieve relevant documents.
- Explain the basic roles of RNN/LSTM, attention, and transformer architectures.
- Apply pre-trained transformer models to classification, generation, translation, summarization, and conversational tasks.
- Build basic document-classification and boundary-detection workflows.
🌍 Applications of NLP
- Search engines and document retrieval
- Chatbots and virtual assistants
- Spam filtering and text classification
- Customer-review and social-media sentiment analysis
- Machine translation and text summarization
- Resume and document analysis
- Information extraction and question answering
- Topic discovery and document organization
- Text generation and autocomplete
📌 Important Notes
- Practical coverage vs. available files: this README lists all 32 practicals in the supplied practical list. Make sure each corresponding script or notebook is present in the repository before claiming that every program is implemented.
- Model compatibility: library APIs and model availability can change. Check the installed library documentation if a model-loading command fails.
- Coreference resolution: neuralcoref is an older package and may not work with modern spaCy versions; a compatible alternative may be required.
- Preprocessing depends on the task: stop-word removal and stemming are not suitable for every NLP pipeline.
- BoW and TF-IDF: these representations do not inherently preserve full word order or meaning.
- Embeddings: Word2Vec and GloVe provide word vectors; BERT produces contextual representations. These methods are related but not interchangeable.
- Similarity measures: higher cosine similarity generally indicates more similar vectors; lower WMD indicates less semantic distance.
- Topic modeling: LDA and LSA use different approaches and their topics may require human interpretation.
- Transformer resources: large models can take time and memory to download and run. Use a suitable runtime and avoid exposing API keys or credentials in notebooks.
👩‍💻 Author
Aditi Panwar
B.Tech CSE (AI)
⭐ If you find this repository useful, consider giving it a star!
