# Personality Classification from Social Media Posts Using IndoBERT

This project implements **IndoBERT** to classify users' personalities based on their posts on **X (formerly Twitter)**. The classification is based on the **Big Five Personality** model, a widely used and validated framework in psychology. The approach focuses on leveraging Indonesian language data to build an effective personality prediction model.

---

## Background
Social media has become a platform where individuals express their thoughts, emotions, and behaviors, which can reflect their personality traits. The Big Five Personality model provides a structured way to categorize these traits into five dimensions. IndoBERT, a pre-trained transformer model for the Indonesian language, is chosen due to its superior performance compared to traditional machine learning models in text classification tasks.

---

## Objectives
1. Analyze and evaluate the factors that influence the performance of a personality classification model using IndoBERT.
2. Assess IndoBERT’s capability to classify personality traits based on users’ posts on social media.

---

## Dataset
- **Language:** Indonesian
- **Source:** Posts from X (Twitter) with participants who completed the Big Five Inventory (BFI-44) questionnaire.
- **Scope:**
  - Focused on personality classification using IndoBERT.
  - Data is text-only and in Indonesian.
- **Programming Language:** Python

---

## Workflow
1. **Data Preprocessing**
   - Case Folding
   - Text Cleaning
   - Normalization
   - Tokenization
   - Stopword Removal
   - Stemming
2. **Modeling**
   - Model: `indobenchmark/indobert-base-p1` from HuggingFace
3. **Experiment Scenarios**
   - **Scenario 1:** Without stemming
   - **Scenario 2:** With stemming
   - **Scenario 3:** Upsampling data (with and without stemming)

---

## Experiment Results
- **Best Performance:** Scenario 1 (without stemming)
  - **Accuracy:** 59%
  - **F1-Score:** 54%
- Findings indicate that preprocessing choices, such as stemming and balancing the dataset, can significantly impact model performance.

---

## Key Insights
- Proper preprocessing and balanced datasets improve classification results.
- The absence of stemming yielded higher performance in this specific dataset.
- Upsampling methods may require further tuning to enhance results.

---

## Future Improvements
- Increase dataset size and ensure balanced class distribution.
- Apply additional preprocessing steps such as:
  - Translating emojis into descriptive text.
  - Translating English words into Indonesian.
- Explore alternative data balancing techniques.

---
