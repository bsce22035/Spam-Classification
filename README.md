# SMS Spam Detection
This project implements an SMS spam classifier using NLP and machine learning techniques. It detects whether an incoming SMS message is "ham" (not spam) or "spam".

##  Exploratory Data Analysis
- Distribution of `ham` vs `spam`
- Message length histogram
- Basic statistics (message count, length)

##  Preprocessing
- Convert to lowercase
- Remove punctuation and digits
- Tokenize and remove English stopwords
- Apply stemming using PorterStemmer

##  Model
- **Algorithm**: Multinomial Naive Bayes
- **Feature Extraction**: CountVectorizer (Bag-of-Words)
- **Train/Test Split**: 80/20

##  Evaluation
- **Accuracy**: ~98%
- **Confusion Matrix**: Visualized with `matplotlib` and `seaborn`

##  Example Inference
```python
print(predict_spam("Congratulations! You've won a free iPhone. Call now!"))
# Output: Spam
