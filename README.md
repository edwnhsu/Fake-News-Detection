### Fake News Detection Using Machine Learning

### Project Overview
This project aims to build a classification model that can accurately detect fake news using various machine learning techniques. The goal is to mitigate the spread of misinformation and enhance the reliability of information consumed by the public, particularly during crucial events like elections.

### Problem Identification

**Objective:**

To develop a classification model that distinguishes between real and fake news. This model is critical in mitigating the harmful impact of misinformation, especially during elections in Taiwan 🇹🇼 and the upcoming 2024 US presidential election 🇺🇸.

**Importance:**

Fake news has been shown to skew public perception, influencing important democratic processes. By accurately identifying fake news, we aim to improve the quality of information shared with the public.

**Citation:**

Kumar S, Asthana R, Upadhyay S, Upreti N, Akbar M (2019) Fake news detection using deep learning models: a novel approach. Trans Emerg Telecommun Technol 5

### Assumptions & Hypothesis
* **Assumption:** Logistic regression might not be the best fit for the classification task due to the non-linear nature of relationships between features (words) and labels (fake or real news).
* **Hypothesis:** Models using more sophisticated algorithms, such as Random Forest or SVM, will perform better given the complexity and high dimensionality of the text data.

### Approach
1. Data Preprocessing:
* **Stop Words Removal:** Removing common stop words to focus on meaningful content.
* **Cleaning:** Removed URLs, newline characters, tabs, and special characters to ensure clean text.
* **Tokenization:** Splitting text into individual words for numerical conversion.
2. Feature Extraction:
* **TF-IDF Vectorizer:** Used to convert text into numerical features, quantifying the importance of words in the dataset.
3. Model Building:
* **Logistic Regression:** A simple linear model for binary classification.
* **Decision Tree:** A non-linear model that builds a tree-like structure to make predictions.
* **Random Forest:** An ensemble method combining multiple decision trees to improve performance.
* **Support Vector Machine (SVM):** A model that finds the optimal separating hyperplane in a high-dimensional space.
4. Model Evaluation:
* **Metrics:** Accuracy, F1 Score, Confusion Matrix, and ROC AUC Score were used to evaluate model performance.
* **Best Performing Model:** The SVM model with parameters C = 0.1, γ = 1, and kernel = 'rbf' achieved an accuracy of approximately 90%.

### Conclusion

This project demonstrates the effectiveness of machine learning algorithms, particularly SVM, in detecting fake news. With careful preprocessing and feature extraction, the model was able to achieve high accuracy, making it a valuable tool in combating misinformation.

### How to Use
* Run the provided Python notebook (.ipynb) to see the full analysis.
* Visualizations are included in the html file to help understand the selection of models.
