# **Malicious URL Detection using Machine Learning**

## **Project Overview**
<br/>

**Objective:** <br/>
To formulate malicious URL detection as a binary classification task for two-class prediction: **malicious** or **benign**

**Detection Technique:** <br/>
Extract lexical features (static analysis) from malicious and benign URLs to train a machine learning algorithm so that it learns to accurately identify unseen malicious URLs

<br/>

## **Data Preprocessing**
<br/>

Total number of data: **594,806 URLs**
- Malicious URLs = 158,081
- Benign URLs = 436,725

Steps:
1. Malicious & benign URLs are combined into one dataset (.csv) using Pandas and then randomly shuffled
2. Tokenize URLs using custom tokenizer function
Feature extraction using TF-IDF Vectorizer (Scikit-learn Feature Extraction module)
3. Convert URL dataset to a matrix of TF-IDF features
    - Number of features extracted = 1,418,106
4. Split dataset into 2 subsets:
    - Training data: 80%
    - Test data: 20%

<br/>

## **Model Training**
<br/>

Model: **Logistic Regression**
1. Create logistic regression classifier
2. Train model using training data
3. Test model using test data

<br/>

## **Performance Evaluation**
<br/>

Accuracy
- Training: 0.9686
- Test: 0.9567

Precision: 0.9666

<br/>

## **Prediction**
<br/>

Additional data
- Source: GitHub
- Total number of URLs = 420,464
    - Malicious URLs = 75,643
    - Benign URLs = 344,821

<br/>

Model Performance
1. Dataset is preprocessed and are fed into trained model as input.
    - Model predicts labels of URLs (malicious/benign)
2. Prediction results:
    - Accuracy: 0.8327
    - Precision: 0.9037


> High model accuracy and precision recorded in classifying URLs of an unseen dataset.

<br/>

## **Conclusion**
<br/>

**Project Outcome:**
- Designed a practical malicious URL detection algorithm with fast detection speed to effectively distinguish genuine and malicious URLs
- Performed static analysis by extracting useful lexical features of URLs which are used to train the machine learning model
- Achieved a satisfying end product which is a logistic regression classifier of high prediction accuracy & precision








