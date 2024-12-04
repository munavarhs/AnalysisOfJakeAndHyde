# AnalysisOfJakeAndHyde

## Overview
This project explores the intriguing behavior of Reddit users who actively participate in two contrasting subreddits: **r/ToastMe** and **r/RoastMe**. These users, referred to as "Jekyll and Hyde" (JH) users, demonstrate remarkable adaptability, switching between supportive and critical personas depending on the community. The study leverages machine learning and natural language processing (NLP) techniques to analyze user behavior and achieve high accuracy in classifying posts from the two subreddits.

---

## Motivation
Understanding how users adapt their behavior across distinct online communities can:
- Provide insights into digital identity and social adaptability.
- Help design healthier online communities and moderation systems.
- Inform algorithms that account for user adaptability while recommending content or moderating behavior.

---

## Key Features
- **Dataset:** Comments from r/ToastMe (positive interactions) and r/RoastMe (humorous criticism), with over **390,000 records collected**.
- **Machine Learning Models:**
  - Logistic Regression
  - Multinomial Naive Bayes
  - Decision Tree
  - Linear SVM
- **Feature Engineering:**
  - TF-IDF vectorization
  - Count Vectorization
  - Word embeddings using GloVe
- **Accuracy Achieved:** 95% classification accuracy for distinguishing subreddit-specific language.

---

## Technical Implementation
- **Data Collection:** Due to API limitations, publicly available datasets were used. Challenges included dataset imbalance between subreddits.
- **Feature Engineering:**
  - TF-IDF for capturing linguistic differences.
  - GloVe embeddings to capture semantic relationships.
- **Model Training:** Optimized for computational efficiency using parallel processing and batch processing techniques.
- **Evaluation Metrics:** Precision, recall, and F1-score were prioritized to account for dataset imbalance.

---

## Challenges
1. **Dataset Imbalance:** r/RoastMe comments significantly outnumbered r/ToastMe comments.
2. **Missing Metadata:** Lack of timestamps and thread hierarchy limited in-depth analysis.
3. **Reddit-Specific Slang:** Pre-trained embeddings struggled with subreddit-specific language.

---

## Conclusions
- Traditional models like Naive Bayes and SVM outperformed advanced techniques (e.g., GloVe embeddings) due to the distinct and separable linguistic patterns of the subreddits.
- Linguistic boundaries between communities reveal how users adapt to community norms, shedding light on the fluid nature of online identities.

---

## Future Work
- Incorporate hierarchical modeling to capture thread structures.
- Explore transformer-based models like BERT for deeper semantic analysis.
- Develop moderation tools using insights from user adaptability.

---

## How to Run
1. **Clone the repository:**
  - git clone https://github.com/munavarhs/AnalysisOfJakeAndHyde/
  - cd AnalysisOfJakeAndHyde
2. **Install dependencies:**
   pip install
3. **Run the analysis notebook:**
   jupyter notebook RoastMeAndToastMeAnalysis.ipynb

---

## Authors
- **Aniket Dineshkumar Hirpara** - anikethirpara@vt.edu
- **Munavar Hussain** - munavarh@vt.edu
