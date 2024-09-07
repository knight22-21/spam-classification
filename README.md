# spam-classification

End to end code for the spam classifier project


# Project Report: Spam Classifier Using Naive Bayes

## 1. Introduction

In this project, we developed a spam classifier using the Naive Bayes algorithm and deployed it as a web application. The objective was to create an effective model for identifying spam emails, which can be integrated into email systems to filter out unwanted messages and enhance user experience.

## 2. Objectives

1. **Develop a Spam Classifier:** Utilize the Naive Bayes algorithm to build a classifier capable of distinguishing between spam and non-spam (ham) emails.
2. **Evaluate Model Performance:** Assess the classifier's performance using metrics such as accuracy and precision.
3. **Deploy the Model:** Create a user-friendly web application for real-time spam classification.

## 3. Methodology

### 3.1 Data Collection

For this project, we used the "SMS Spam Collection Dataset", which includes a diverse set of spam and non-spam texts. The dataset was preprocessed to extract relevant features for the classification task.

### 3.2 Data Preprocessing

1. **Text Cleaning:**
    Before extracting features, we performed text cleaning to ensure that the data is in a suitable format for analysis. The steps involved:

      -> Removing Punctuation: Punctuation marks were removed as they do not contribute to the meaning in the context of spam detection.
      -> Lowercasing: All text was converted to lowercase to ensure uniformity and to prevent discrepancies between the same words in different cases.
      -> Removing Stop Words: Common words such as "and," "the," and "is" were removed because they do not contribute significant information for spam                       classification.
      -> Tokenization: The cleaned text was split into individual words or tokens to facilitate further processing.
2. **Feature Extraction:** We created several new features from the existing data to further enhance the model

### 3.3 Model Development

The Naive Bayes algorithm was chosen due to its simplicity and effectiveness in text classification tasks. We implemented the Naive Bayes classifier using the following steps:

1. **Model Selection:** We used the Multinomial Naive Bayes model, which is well-suited for text classification problems.
2. **Training:** The model was trained on a training dataset consisting of labeled emails (spam and ham).
3. **Evaluation:** Performance was evaluated using a separate validation dataset.

### 3.4 Performance Evaluation

We assessed the classifier using the following metrics:

- **Accuracy:** Measures the overall correctness of the model.
- **Precision:** The proportion of true positives among all predicted positives.
- **Recall:** The proportion of true positives among all actual positives.

Results:
- **Accuracy:** 97%
- **Precision:** 100%
- **Recall:** 98  %


## 3.5 Model Deployment
**Development Environment**
PyCharm: We used PyCharm for developing the Flask web application, which included writing, debugging, and testing the code.

## Hosting
**Connecting to Git Repository:** Integrated the app with a Git repository for continuous deployment.
**Configuration:** Set up deployment settings and environment variables on Render.
**Deployment:** Render handled the build and deployment, making the application accessible via a public URL.

## 4. Results

The deployed spam classifier successfully classified incoming texts into spam or ham with high accuracy. The web application provided real-time feedback and demonstrated ease of use, fulfilling the project objectives.

## 5. Conclusion

The project successfully developed and deployed a spam classifier using the Naive Bayes algorithm. The model achieved high performance metrics and was effectively integrated into a user-friendly web application. This project demonstrates the practical application of machine learning in improving email management systems and provides a foundation for future enhancements, such as incorporating more advanced algorithms or additional features.


## 7. References

- SMS Spam Collection Dataset: [kaggle](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- Scikit-learn Documentation: [Scikit-learn](https://scikit-learn.org/)

---

This report outlines the process of developing and deploying a spam classifier, highlighting key methodologies and results. The success of this project sets a strong precedent for future developments in spam filtering technology.
