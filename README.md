# Chick-fil-A

# Extracting Information from Textual Data Using NLP

## Project Overview
This project applies **Natural Language Processing (NLP)** techniques to extract key information from textual franchise agreements, particularly focusing on **"Item 5: Initial Fees"** in franchise disclosure documents. The goal is to automate the extraction of franchise-related financial data using **Topic Modeling** and **Question-Answering (Q&A) models**.


## Dataset
The dataset consists of **50 franchise disclosure documents** covering "Item 5: Initial Fees". The documents were analyzed using various NLP techniques to extract key terms, financial details, and structured answers.

## Methods Used
### 1. **Frequency-Based Methods**
- **Bag of Words (BoW)**: Counts word frequency to identify common terms in franchise agreements.
- **N-Gram Analysis**: Uses bigrams to extract common phrases that provide better context.
- **TF-IDF (Term Frequency-Inverse Document Frequency)**: Identifies words that are important within specific franchise documents.

### 2. **Topic Modeling**
- **K-Means Clustering**: Groups franchises into categories such as food vs. non-food franchises based on textual content.
- **Sentence-BERT Embeddings**: Identifies underlying topics using a deep learning-based approach.

### 3. **Question-Answering Task**
- **Model Used**: RoBERTa (pre-trained transformer model)
- **Objective**: Automatically extract the **initial franchise fee** using predefined questions.
- **Questions Asked**:
  - What is the initial fee?
  - What is the initial fee in dollars?
  - What is the initial franchise fee in dollars?
  - What is the initial nonrefundable franchise fee in dollars (standard)?

## Results
- The Q&A model successfully extracted **initial fees** with high accuracy.
- Question 3 ("What is the initial franchise fee in dollars?") provided the **best results**, achieving an **F1-score of 0.76**.
- Clustering methods showed that franchises can be grouped based on fee structures and business models.

## Files in the Repository
- `chik-fil-a.ipynb` – NLP analysis on the Chick-fil-A dataset.
- `Combination of Methods_Item 5.ipynb` – Combines frequency-based and embedding-based methods.
- `QnA_BERT_VS_v1_1.ipynb` & `QnA_BERT_VS_v2.ipynb` – Question-answering models based on RoBERTa.
- `Word_Cloud_Visualization.ipynb` – Visual representation of keywords from the franchise agreements.
- `FourQuestions_m.csv` & `FourQuestions_roberta_m.csv` – Datasets containing extracted Q&A results.
- `6_Report_Extracting Information from Textual Data Using NLP.pdf` – Detailed report on project findings.


## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/your-repository.git
