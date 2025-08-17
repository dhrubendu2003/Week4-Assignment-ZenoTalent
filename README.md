# NLP Assignment: Text Analysis and Topic Discovery

## 📌 Assignment Title  
**Text Analysis and Topic Discovery Using NLP Techniques**

## 📚 Dataset Used  
A custom corpus of **12 short text documents** related to **technology, data science, artificial intelligence, and machine learning**. The texts were designed to simulate real-world content such as blog posts or Wikipedia-style articles on AI topics.

Each document is 1–2 sentences long and covers themes like:
- Machine Learning
- Deep Learning
- Natural Language Processing (NLP)
- Data Science
- Unsupervised Learning
- Python Programming

This small but thematically rich dataset was used to demonstrate key NLP techniques effectively.

---

## 🔍 Analysis Steps Overview

The project followed a structured pipeline to analyze the text corpus:

### 1. **Text Preprocessing**
- Converted all text to lowercase.
- Removed punctuation and special characters.
- Tokenized into words.
- Filtered out English stopwords and non-alphabetic tokens.

### 2. **TF-IDF Analysis**
- Computed TF-IDF scores for each word in the corpus.
- Identified top 10 high-scoring words per document to extract key terms.

### 3. **Word2Vec Embeddings**
- Trained a skip-gram model using Gensim to learn dense word representations.
- Found most similar words to key terms like *data*, *learning*, and *analysis*.
- Visualized embeddings using **t-SNE** to reveal semantic clusters.

### 4. **Topic Modeling with LDA**
- Applied Latent Dirichlet Allocation (LDA) to discover **5 latent topics**.
- Extracted top 5 words per topic to interpret themes.
- Assigned dominant topic to each document based on highest probability.
- Used **pyLDAvis** for interactive visualization of topic coherence and term relevance.

---

## 🖼️ Visualizations

### 1. Word2Vec Embeddings (t-SNE Visualization)
This plot shows the 2D projection of Word2Vec embeddings using t-SNE. Words that are semantically similar appear close together, revealing natural groupings such as "deep", "neural", "learning" clustering around AI concepts.

![Word2Vec Embeddings (t-SNE Visualization)](https://raw.githubusercontent.com/dhrubendu2003/Week4-Assignment-ZenoTalent/main/word2vec_tsne.png)

> *Caption: t-SNE visualization of Word2Vec embeddings showing clusters of semantically related words.*

---

### 2. pyLDAvis Topic Visualization
This interactive intertopic distance map displays the 5 discovered topics. The size of each bubble reflects the topic’s prevalence in the corpus. The right panel shows the top-30 most relevant terms for each topic, with color indicating term saliency within the selected topic.

![pyLDAvis Topic Visualization](https://raw.githubusercontent.com/dhrubendu2003/Week4-Assignment-ZenoTalent/main/pyldavis_topics.png)

> *Caption: pyLDAvis output showing topic distribution, keyword relevance, and intertopic distances.*
