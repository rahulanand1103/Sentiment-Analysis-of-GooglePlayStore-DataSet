# Sentiment-Analysis-of-GooglePlayStore-DataSet 
## 1.Business Problem
### 1.1 Description
#### Description
### Source
https://www.kaggle.com/lava18/google-play-store-apps/home

## 2.Machine learning problem
### 2.1 Data
#### 2.1.1 Data Overview

total rows=64295 <br>
Features=5 <br>

Attribute Information:<br>

1.App- Application name <br>
2.Translated_Review- User review (Preprocessed and translated to English) <br>
3.Sentiment-Positive/Negative/Neutral (Preprocessed) <br>
4.Sentiment_Polarity- Sentiment polarity score <br>
5.Sentiment_Subjectivity- Sentiment subjectivity score <br>

### 2.2 Mapping the real-world problem to a Machine Learning Problem
#### 2.2.1 Type of Machine Learning Problem
Binary Classification problem,Given a review we need to predict it is negative,neutral,postive reviews
#### 2.2.2 Performance metric
F1-score

## Conclusion

<b>1.Naive Bayes</b>

|Model |hyper parameter|F1-score cv|Accuracy cv|F1-score test|Accuracy Test|
|------|------|------|------|------|------|
|uni-gram|0.0005| 0.882|0.770|82.701%|
|bi-gram |0.0005| 0.882|0.770|82.701%|
| TF-IDF|0.0005| 0.882|0.770|82.701%|

<b>2.Logistic Regression</b>

|Model|hyper parameter|F1-score cv|Accuracy cv|F1-score test|Accuracy Test|
|------|------|------|------|------|------|
|uni-gram|1| 0.925|0.911|92.893%|
|bi-gram |100| 0.931|0.919|93.521%|
| TF-IDF|100| 0.932|0.915|93.388%|

<b>3.Linear SVM</b>

|Model |hyper parameter|F1-score cv|F1-score test|Accuracy Test|
|------|------|------|------|------|
|unigram|0.0001| 0.897|0.869|89.861%|
|bi-gram|0.00005| 0.895|0.858|88.792%|
| TF-IDF |0.00005| 0.882|0.846|88.298%|
