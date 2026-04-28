# KeyBERT Stakeholder Values

## Overview

This project develops an unsupervised Natural Language Processing (NLP) framework using **KeyBERT** to identify stakeholder-value themes from transportation resilience literature.

Transportation systems face increasing disruptions from disasters, climate-related events, and infrastructure failures. Understanding stakeholder priorities is important for resilient planning and recovery. However, manually reviewing literature to identify these concerns is time-consuming, subjective, and difficult to scale.

This project addresses that challenge by applying machine learning–based keyphrase extraction to automatically discover meaningful stakeholder values from academic documents.

---

## Objectives

- Develop a KeyBERT-based unsupervised machine learning framework for stakeholder-value extraction.
- Identify dominant stakeholder-value themes in transportation resilience literature.
- Evaluate extraction relevance, consistency, and robustness.

---

## Repository Structure

```text
keybert-stakeholder-values/
│── Data/
│── Notebooks/
│── Outputs/
│   ├── Figures/
│   └── Tables/
│── Docs/
│   └── Presentations/
│── README.md
│── requirements.txt
```

## Folder Description

- **Data/** : input datasets and literature corpus  
- **Notebooks/** : Jupyter notebook containing preprocessing, modeling, evaluation, and visualization workflow  
- **Outputs/** : generated figures, charts, and result tables  
- **Docs/** : presentation slides and supporting project files

---

## Data

### Source of Data

The dataset was developed from academic literature collected through Google Scholar and related scholarly sources.

### What the Data Contains

A curated corpus of **20+ transportation resilience papers** with:

- Title  
- Author keywords  
- Full text (where available)

### Is Data Included in Repository?

Yes. Processed project data and generated outputs are included.

### If Some Data Is Not Included

Some copyrighted full-text papers may not be redistributed. Processed outputs and metadata are provided.

---

## Methods

This project follows a complete machine learning workflow:

1. Data collection and screening  
2. Text preprocessing  
3. KeyBERT keyphrase extraction  
4. Semantic similarity ranking  
5. Stakeholder-value category mapping  
6. Precision@10 validation  
7. Robustness checks

### Core Modeling Components

- KeyBERT  
- SentenceTransformers  
- MiniLM embeddings  
- Cosine similarity ranking

### Example Parameters

- top_n = 20  
- ngram_range = (1,3)  
- diversity = 0.7

---

## Requirements

### Software

- Python 3.10+

### Python Libraries

- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- keybert  
- sentence-transformers  
- jupyter

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/keybert-stakeholder-values.git
```

### 2. Enter Project Folder

```bash
cd keybert-stakeholder-values
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open Notebook

```text
Notebooks/submission_guided_keybert_stakeholder_values.ipynb
```

### 6. Run All Cells

All figures and output tables will be generated in the **Outputs/** folder.

---

## Key Results

Highest Support Categories:

- Sustainability  
- Adaptability  
- Accessibility  
- Equity

Moderate Support Categories:

- Recoverability  
- Economic Continuity  
- Responsiveness

Lower Relative Support Categories:

- Reliability  
- Robustness  
- Functionality

These findings suggest increasing emphasis on adaptive, social, and sustainable dimensions of resilience.

---

## Authors

Shah Salah Uddin Chowdhury  
Machine Learning Final Project  
The University of Texas at Arlington
