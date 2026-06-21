# 🎬 CineSafe

**Building a Content Warning and Accessibility Dataset for Movies**

CineSafe is a data engineering and machine learning project that augments movie datasets with detailed **content warnings** and **accessibility metadata**. The goal is to help viewers make informed decisions about the movies they watch by going beyond traditional age ratings such as PG-13 and R.

---

## 🌟 Motivation

Movie rating systems often lack information that many viewers care about, including:

* Sexual assault scenes
* Self-harm or suicide content
* Animal cruelty
* Flashing lights and strobe effects
* Jump scares
* Drug and alcohol use
* Accessibility features such as subtitles and audio descriptions

This missing information can significantly impact:

* Parents selecting movies for children
* People with PTSD or trauma triggers
* Individuals with sensory sensitivities
* Deaf and visually impaired viewers

CineSafe aims to provide richer and more personalized movie metadata to address these needs.

---

## 🎯 Research Question

> Can machine learning automatically generate meaningful content warnings and accessibility metadata from existing movie information?

---

## 🚀 Project Goals

* Create an augmented movie dataset.
* Predict content warnings using machine learning.
* Generate accessibility metadata.
* Build a personalized recommendation engine.
* Develop an interactive dashboard.

---

## 🏗️ System Architecture

```text
Movie Metadata
        +
     Subtitles
        +
 Feature Engineering
        +
Multi-label Classifier
        +
 Augmented Dataset
        +
Recommendation Engine
        +
 Interactive Dashboard
```

---

## 📊 Dataset Augmentation

### Content Warning Labels

* Violence
* Gore
* Death
* Suicide / Self-harm
* Sexual content
* Sexual assault
* Child abuse
* Domestic abuse
* Drug use
* Alcohol use
* Animal cruelty
* Racism
* Bullying
* Torture
* Flashing lights
* Jump scares

### Accessibility Labels

* Closed captions available
* Audio descriptions available
* Sign language support
* Low-dialogue content
* Foreign language indicators

### Intensity Scores

Each warning receives an intensity score:

| Score | Meaning  |
| ----: | -------- |
|     0 | None     |
|     1 | Mild     |
|     2 | Moderate |
|     3 | Severe   |

---

## 🧠 Machine Learning

### Problem Formulation

Multi-label classification.

**Input**

* Movie metadata
* Plot summaries
* Subtitles
* Keywords
* Genres

**Output**

* Content warnings
* Accessibility labels
* Severity scores

### Potential Models

* Logistic Regression
* Random Forest
* XGBoost
* Fine-tuned BERT

### Evaluation Metrics

* Precision
* Recall
* F1 Score
* Hamming Loss
* AUROC

---

## 💡 Recommendation Engine

Example user preferences:

```json
{
  "avoid": [
    "sexual_assault",
    "animal_cruelty",
    "flashing_lights"
  ]
}
```

The system recommends movies that match the user's safety preferences.

---

## 📈 Future Features

* Interactive dashboard
* Genre versus trigger visualizations
* Historical trend analysis
* LLM-assisted content warning generation
* Browser extension for streaming services

---

## 🌍 Social Impact

CineSafe promotes:

* Accessibility and inclusion
* Mental health awareness
* Informed viewing decisions
* Better parental guidance
* Richer movie metadata for recommendation systems

---

## 🛠️ Proposed Tech Stack

| Area             | Technology                     |
| ---------------- | ------------------------------ |
| Data Collection  | Python, Pandas                 |
| NLP              | NLTK, spaCy, Transformers      |
| Machine Learning | Scikit-learn, XGBoost, PyTorch |
| Visualization    | Plotly, Matplotlib             |
| Dashboard        | Streamlit                      |
| Dataset Storage  | CSV, SQLite                    |

---

## 📁 Repository Structure

```text
cinesafe/
├── data/
├── notebooks/
├── src/
│   ├── preprocessing/
│   ├── models/
│   ├── recommendation/
│   └── dashboard/
├── docs/
├── index.html
└── README.md
```

---

## 📄 Project Status

🚧 Proposal and initial design phase.

---

## 📜 License

This project is intended for educational and research purposes.

---

## 👥 Authors

Created as a school project exploring:

* Data Engineering
* Natural Language Processing
* Machine Learning
* Accessibility Research
* Human-Centered AI
