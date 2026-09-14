NLP Practicals
📌 Description

This repository contains a collection of basic Natural Language Processing (NLP) practical programs implemented using Python, NLTK, spaCy, and Regular Expressions (RegEx).

The practicals cover important NLP concepts such as tokenization, stemming, lemmatization, stop-word removal, Part-of-Speech tagging, parsing, chunking, and Named Entity Recognition (NER).

These programs are designed to provide a basic understanding of how computers process and analyze human language.

🎯 Objectives

The main objectives of these practicals are:

To understand the fundamentals of Natural Language Processing.
To perform sentence and word tokenization.
To understand stemming and lemmatization.
To remove unnecessary stop words from text.
To perform Part-of-Speech (POS) tagging.
To understand parsing and chunking.
To identify important entities from text using Named Entity Recognition.
To gain practical experience with NLTK, spaCy, and RegEx.
🛠️ Technologies Used
Python 3.x – Programming language used to implement all practicals.
NLTK – Used for tokenization, stemming, stop-word removal, and POS tagging.
spaCy – Used for tokenization, POS tagging, chunking, and Named Entity Recognition.
Regular Expressions (RegEx) – Used for pattern-based parsing and chunking.
📂 Repository Structure
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
📚 Practicals Explained
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

NLP, is, interesting, It, is, used, in, AI
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

Tokenization is generally one of the first steps of NLP preprocessing, because later NLP operations work on individual sentences and words.

2️⃣ Stemming and Lemmatization
File:

02_Stemming_Lemmatization.py

🔹 What is Stemming?

Stemming reduces a word to its root-like form by removing prefixes or suffixes.

For example:

playing → play
played  → play
studies → studi

The result produced by stemming may not always be a valid English word.

🔹 What is Lemmatization?

Lemmatization converts a word into its meaningful base or dictionary form, called a lemma.

Examples:

running → run
better  → good
studies → study

Unlike stemming, lemmatization generally produces a meaningful word.

🔹 What does the program do?

The practical:

Takes a list or sentence containing different words.
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

the, is, a, an, of, and, in, to
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

Note: Stop words should not always be removed. Their importance depends on the NLP task. For example, words such as "not" can be important for sentiment analysis.

4️⃣ Part-of-Speech (POS) Tagging
File:

04_POS_Tagging.py

🔹 What is POS Tagging?

Part-of-Speech tagging assigns a grammatical category to each word in a sentence.

Common POS categories include:

POS	Meaning	Example
Noun	Name of person, place, thing, etc.	book
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

Output:

The       DT
student   NN
reads     VBZ
a         DT
book      NN

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

Named Entity Recognition (NER) is the process of identifying important entities in a text and assigning them categories.

Common entities include:

PERSON – Person's name
ORG – Organization
GPE – Geopolitical entity/place
DATE – Date
MONEY – Monetary value
LOC – Location
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

Aditi      → PERSON
Microsoft  → ORG
Noida      → GPE
Monday     → DATE

The exact entities recognized depend on the spaCy model and context.

🔹 Important Functions/Concepts
spacy.load() – Loads the trained NLP model.
nlp() – Processes the input text.
doc.ents – Returns recognized entities.
ent.text – Gives the entity text.
ent.label_ – Gives the entity category.
💡 Key Learning

NER is useful for extracting important information from unstructured text and is widely used in applications such as information extraction, search engines, chatbots, and document analysis.

🔄 Overall NLP Workflow

The practicals collectively demonstrate a basic NLP preprocessing and analysis workflow:

                Input Text
                    │
                    ▼
              Tokenization
                    │
                    ▼
        ┌───────────┴───────────┐
        ▼                       ▼
 Stemming/Lemmatization   Stop-word Removal
        │                       │
        └───────────┬───────────┘
                    ▼
               POS Tagging
                    │
                    ▼
           Parsing / Chunking
                    │
                    ▼
          Named Entity Recognition
                    │
                    ▼
              Processed Text

These steps do not have to be applied in exactly this order for every NLP application. The preprocessing pipeline depends on the problem being solved.

⚙️ Installation and Setup
1. Install Python

Make sure Python 3.x is installed on your system.

Check the installation using:

python --version
2. Install Required Libraries

Open the terminal in the project directory and run:

pip install nltk spacy
3. Download Required NLTK Resources

Depending on the practicals and your NLTK version, download the required resources:

import nltk

nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')

If your installed NLTK version asks for newer resource names, download the resources indicated by the error message.

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
🧪 Sample Input

The following text can be used for testing several practicals:

Natural Language Processing is a part of Artificial Intelligence.
It helps computers understand and process human language.
📖 Concepts Covered
Practical	Main Concept	Library/Tool
01	Tokenization	NLTK, spaCy
02	Stemming & Lemmatization	NLTK
03	Stop-word Removal	NLTK
04	POS Tagging	NLTK
05	Parsing & Chunking	NLTK, RegEx, spaCy
06	Named Entity Recognition	spaCy
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
Work with basic NLP libraries such as NLTK and spaCy.
Understand the basic workflow of text preprocessing and analysis.
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
👩‍💻 Author

Aditi Panwar
B.Tech CSE (AI)
