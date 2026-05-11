# Resume Matching Engine

A Python-based Resume Matching Engine that takes in resumes and job descriptions, and outputs the top matching candidates for each job description.

---

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Algorithm](#algorithm)
- [Example Use Cases](#example-use-cases)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

The **Resume Matching Engine** is a Python-based application designed to automate resume screening by matching resumes with job descriptions based on skill similarity.

The system processes a collection of resumes and job descriptions, analyzes the skills present in each, and ranks candidates according to how well they match a specific role.

This project demonstrates concepts from:

- Natural Language Processing (NLP)
- Information Retrieval
- TF-IDF Vectorization
- Cosine Similarity
- Data Preprocessing

---

## Features

### ✅ Skill Normalization
Standardizes skills into a common format using a predefined alias mapping.

Example:
- `JS` → `JavaScript`
- `Py` → `Python`

---

### ✅ Deduplication
Removes duplicate skills from each resume to improve matching accuracy.

---

### ✅ Vocabulary Construction
Builds a shared vocabulary containing all unique skills extracted from resumes.

---

### ✅ TF-IDF Vector Construction
Represents each resume as a TF-IDF vector where:
- Each dimension corresponds to a skill
- Importance is weighted using TF-IDF scoring

---

### ✅ Binary Vector Construction
Represents each job description as a binary vector indicating the presence or absence of required skills.

---

### ✅ Cosine Similarity Calculation
Calculates similarity scores between:
- Resume TF-IDF vectors
- Job description vectors

---

### ✅ Candidate Ranking
Ranks resumes based on cosine similarity scores for each job description.

---

## Requirements

- Python 3.8+
- No external libraries required

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/resume-matching-engine.git
