## Comparative Analysis of Machine Learning Algorithms for Spam Detection using Ensemble Techniques

### Project description
This project investigates the effectiveness of machine learning algorithms and ensemble methods for spam text message detection. It aims to implement and compare the performance of Logistic Regression, K-nearest Neighbor, Support Vector Machine, Multinomial Naive Bayes, Random Forest, Decision Tree, and Meta model of Gradient Boosting classifier on the SMS Spam Collection Dataset, develop and evaluate a stacking ensemble approach that combines the strengths of both models for improved spam classification, and analyze the impact of hyperparameter tuning on the performance of these models.

### Team member’s role and contribution:
In this project, I will 
* download, explore, and pre-process the SMS Spam dataset
* implement and evaluate the baseline
   * Logistic Regression,
   * K-nearest Neighbor,
   * Support Vector Machine,
   * Multinomial Naive Bayes,
   * Random Forest,
   * Decision Tree,
   * Gradient Boosting 
* develop and evaluate the stacking ensemble approach
* conduct hyperparameter tuning for all models
* analyze and interpret the results
* prepare project deliverables (code, documentation, presentation)

### Dataset
[SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
* The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.

### Data preprocessing
* Drop unnecessary columns: Unnamed: 2, Unnamed: 3, Unnamed: 4 
* Rename column names: v1 -> Label, v2  -> Message
* Drop duplicates  
* Remove special characters
  * Example: !"#$%&\'()*+,-./:;<=>?@[\\]^_{|}~`
* Remove stop words: don’t provide valuable information for downstream analysis
  * Example: “I, the, me, what”
* Lemmatize text: reduce words to their lemma or meaningful base form
  * Example: swims -> swim, flying -> fly
* Apply Term Frequency – Inverse Document Frequency

### Proposed approach model structure
![model_structure](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/e5121543-e90d-41ae-a51e-d9dce25579c3)

### Out-of-fold predictions
![out_of_fold](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/2dcd441f-965b-4bce-93fd-d799e55100d4)

### Performance
#### Baselines
![image](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/1e4aa11d-1e1b-460f-90cd-86935390f6f6)

#### Tuned models 
##### Accuracy performance
![accuracy_performance](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/9ed32bd9-5b00-4bb3-ab50-ebdd7e06f12e)
<br></br> 
##### Precision, Recall, F1 performance
![perfomance](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/6e618dae-3248-4b35-b66e-5bc9edcd167e)
<br></br> 
##### AUC performance
![auc](https://github.com/TienNguyen93/Spam-prediction/assets/43976085/6a5e121f-8f4d-4907-aa63-fcd3653d51e7)


