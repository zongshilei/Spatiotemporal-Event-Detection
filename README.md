# LLM-based Geographic Location Prediction for Spatio-Temporal Event Detection

This repository contains the implementation of a course project that explores the use of Large Language Models (LLMs) for geographic location prediction in social media posts.

The goal of this project is to improve spatio-temporal event detection by utilizing both geotagged and non-geotagged Twitter posts. Currently, the project focuses on data preprocessing and location prediction, while event clustering using SBERT and HDBSCAN is planned as future work.

---

## Project Overview

Traditional spatio-temporal event detection methods only use geotagged posts, which represent a very small portion of Twitter data.

This project investigates whether LLMs can infer state-level locations from tweet content, allowing non-geotagged posts to participate in regional event detection.

Current workflow:

```

Twitter Dataset
↓
Data Cleaning
↓
LLM Geographic Information Extraction
↓
State-level Location Prediction
↓
(Future Work)
SBERT + HDBSCAN Event Detection

```

---

## Repository Structure

```

.
├── Cleaning data and LLM process.ipynb
├── locationpredicate.ipynb
├── TRECIS-CTIT-H-extracted-merged.json
└── README.md

```

---

## Files

### Cleaning data and LLM process.ipynb

Performs:

- Data preprocessing
- Text cleaning
- Geographic entity extraction using LLM
- Preparation of prediction inputs

---

### locationpredicate.ipynb

Implements state-level location prediction based on:

- Geographic entities extracted by the LLM
- OpenStreetMap (OSM) information
- Rule-based location selection

---

### TRECIS-CTIT-H-extracted-merged.json

Dataset used in this project.

The dataset contains Twitter posts collected for crisis and event analysis and is used for location prediction experiments.

---

## Current Progress

| Module | Status |
|------------------------------|------------|
| Dataset Preparation | ✅ Completed |
| Data Cleaning | ✅ Completed |
| LLM Geographic Extraction | ✅ Completed |
| State-level Location Prediction | ✅ Completed |
| SBERT Semantic Embedding | ⏳ Planned |
| HDBSCAN Event Clustering | ⏳ Planned |
| Real-time Event Detection | ⏳ Planned |

---

## Technologies

- Python
- Large Language Models (LLM)
- OpenStreetMap (OSM)
- Jupyter Notebook

Future work:

- Sentence-BERT (SBERT)
- HDBSCAN

---

## Future Work

Due to time constraints, the semantic event detection module has not yet been implemented.

Future improvements include:

- SBERT-based tweet embeddings
- HDBSCAN event clustering
- Keyword-based event topic extraction
- Real-time regional event monitoring

---

## Purpose

This repository was developed as a course project for exploring the application of LLMs in geographic location prediction and spatio-temporal event detection.

The current implementation focuses on the location prediction stage and serves as the foundation for future event detection experiments.
