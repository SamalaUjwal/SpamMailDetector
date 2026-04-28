## Spam Mail Detector (Machine Learning Project)

## Objective

Build a machine learning model to classify messages as:

* **Spam** 
* **Ham (Not Spam)** 
using text data.


## Dataset

* Source: SMS Spam Collection Dataset (UCI)
* Total Messages: ~5,500
* Labels:
  * `ham` → Normal message
  * `spam` → Unwanted message


## Project Workflow

### Data Loading

* Dataset loaded from public source
* Two columns:

  * `label` (spam/ham)
  * `message` (text)

### Text Preprocessing

* Converted text to lowercase
* Removed stopwords
* Tokenization handled by vectorizer

### Feature Engineering

* Used **TF-IDF Vectorization**
* Converted text → numerical features

### Train-Test Split

* 80% training
* 20% testing

###  Model Used

* **Logistic Regression**

### Model Evaluation

* Accuracy Score
* Confusion Matrix
* Precision, Recall, F1-score

## Results

| Metric            | Value |
| ----------------- | ----- |
| Training Accuracy | 0.969 |
| Testing Accuracy  | 0.966 |

* Model performs well in detecting spam messages with high accuracy.


## Confusion Matrix
<img width="637" height="477" alt="image" src="https://github.com/user-attachments/assets/388e5fda-4025-40fb-903e-b6cee063ade8" />

## Key Insights

* Spam messages often contain:

* promotional words (“win”, “free”, “offer”)
* Ham messages are more conversational
* TF-IDF effectively captures important words


## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn


## Project Structure

```
spam-detector/
│
├── spam_model.ipynb
├── mail_data.csv
├── README.md
```


## Author

Samala Ujwal
