# LLM-Cancer-Classification-using-Pathology-text

Dataset used: TCGA_Reports (https://www.cancer.gov/ccg/research/genome-sequencing/tcga)

# Project Overview
This project explores the integration of advanced large language models for cancer classification through the analysis of pathology text data. Utilizing Natural Language Processing (NLP) techniques, the goal is to enhance the understanding of various cancer pathologies and streamline clinical decision-making processes.

# Abstract
This project leverages GPT-3 and LangChain to enhance cancer classification using pathology text data. By embedding large datasets into a Vector Store, we enable efficient data access and improved computational performance. A key comparison highlights that using an index significantly improves the model's ability to generate accurate, context-specific responses compared to operating without one. Utilizing pathology reports from trusted sources like TCGA, this study demonstrates the potential of NLP and LLMs in advancing diagnostic precision and personalized treatment in healthcare.

# Introduction
Cancer classification plays a critical role in modern healthcare by enabling precise diagnosis and personalized treatment strategies. Pathology reports, rich in clinical insights, serve as vital resources for understanding cancer types. However, manually extracting information from these reports is time-consuming and prone to inconsistencies. The integration of Natural Language Processing (NLP) with advanced large language models (LLMs) like GPT-3 offers a transformative solution by automating this process with speed and accuracy.

This project utilizes GPT-3 alongside LangChain, a framework designed to optimize LLM performance by managing large datasets efficiently. LangChain organizes and embeds extensive data sources, such as pathology reports, into a Vector Store, ensuring seamless access and minimal computational overhead. By comparing the model's performance with and without indexing, the study highlights the value of structured data in improving context-specific responses. Pathology data from trusted sources, including TCGA Pathology Reports, further strengthens the reliability of this approach.

Through this innovative combination of LLMs and data management frameworks, this project underscores the potential of NLP in advancing cancer diagnostics and improving patient outcomes.

# Understanding the Data Set
The data used in this research is sourced from the Cancer Genome Atlas (TCGA), containing extensive pathology reports useful for NLP applications. The dataset includes several types of cancer, such as ovarian peritoneal adenocarcinoma, colorectal adenocarcinoma, malignant melanoma, and retinal cell carcinoma.

# Methodology
This project employs a structured approach to leverage GPT-3 and LangChain for cancer classification using pathology text data. The methodology begins with data collection from trusted repositories like The Cancer Genome Atlas (TCGA), where pathology reports related to various cancer types are sourced. These reports are then organized within the LangChain framework, ensuring efficient data management and accessibility.

Data preprocessing is a critical step in preparing the raw pathology text for analysis. Initially, the text is encoded using standardized format such as UTF-8, ensuring compatibility across the dataset. Noise elements such as special characters, HTML tags, and irrelevant symbols are removed to maintain data integrity. Tokenization is performed using libraries like NLTK and spaCy, which break down the text into meaningful units (tokens). Additionally, text normalization is applied, converting all characters to lowercase and performing stemming to ensure consistency in the dataset.

For feature engineering, Named Entity Recognition (NER) is employed to extract crucial entities like cancer types, biomarkers, and diagnostic terms from the unstructured text. To enhance the semantic richness of the data, techniques such as TF-IDF and BERT embeddings are used to capture contextual relationships and preserve the meaning of words within the reports. This enables a more accurate understanding of the pathology data.

Once the data is preprocessed and feature extraction is complete, machine learning models are trained to classify cancer types. Initial performance is assessed using baseline models like Naive Bayes (Bernoulli, Multinomial, and Gaussian), which are well-suited for text classification tasks. The project also incorporates LangChain for indexing and embedding the data into a Vector Store, facilitating more efficient data retrieval and improving the model's ability to produce context-aware responses. The indexing step ensures that the model can reference specific documents, thereby enhancing its accuracy.

The dataset is split into training and testing sets (80:20 ratio) to evaluate the model's performance. Key metrics such as precision, recall, F1-score, and confusion matrices are used to assess the model's classification effectiveness. Additionally, experiments are conducted to compare the model's accuracy when indexing is applied versus when it is not, demonstrating the advantage of using indexed data for more specific and accurate predictions.

Throughout the project, Python libraries such as NLTK, spaCy, and scikit-learn are utilized for preprocessing, feature extraction, and model evaluation. LangChain serves as the core framework for managing large datasets and embedding them into the Vector Store, while GPT-3 is employed to perform cancer classification. This methodology highlights the power of structured data management and the application of advanced NLP techniques in improving cancer diagnosis and patient outcomes.
<img width="471" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/1856dd65-5046-4753-9465-1e6528e5e6c9">

# Data Preprocessing
Key preprocessing steps include text cleaning, tokenization, and transformation of pathologic text data using TF-IDF. Principal Component Analysis (PCA) is used for data reduction, and a data sampling approach ensures balanced class distribution.

<img width="470" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/5b1f802b-8c1c-4965-90d9-60319136194a">

# Data Analysis
Advanced classification techniques, specifically Naive Bayes and Logistic Regression, are employed to analyze and categorize pathology reports. Logistic Regression demonstrated superior performance in accuracy and overall efficacy.

<img width="312" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/eb728fef-a26a-4e91-95ad-2723079b15fa">

# Implementation
The implementation involves a structured program for data processing, model training, testing, and cross-validation. Both Naive Bayes and Logistic Regression models are evaluated based on key performance metrics like accuracy, precision, recall, and F1-score.


<img width="478" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/da79a76f-2d1d-4919-9f9d-c4b2b0225e04">


<img width="472" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/7f46b2fc-9353-4bbc-a095-f35b0155cad3">

# Logistic Regression Implementation

<img width="469" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/89d12b3c-5ddf-41f9-8c2c-ed43f3e91315">

# Naive Bayes Implementation

<img width="475" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/7f1aec8c-101e-4ac2-a545-ed389e48b3d4">

# Experiment Results and Analysis
The results highlight the effectiveness of NLP techniques in extracting meaningful information from pathology reports. Logistic Regression outperformed Naive Bayes, achieving higher accuracy and better handling the complexities of medical texts.

# Null Value Checking and Labeling

<img width="444" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/7cf94713-8e21-4301-95c7-7e9468e9deac">

# Patients File Name Value Count
<img width="432" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/fcc0494f-b0b5-4ad0-8d52-e4f836f00b4c">

# Word Cloud of Overall Text Data
<img width="373" alt="image" src="https://github.com/MarySuneela/LLM-Cancer-Classification-using-Pathology-text/assets/107396938/00fc4a2e-15f9-42c7-85c6-6c41767435d7">

