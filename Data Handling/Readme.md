##Summary of my Work on Machine Learning and Deep Learning Models for Imbalanced Data

### Machine Learning Models:
- <b>Logistic Regression:</b> Implemented with class balancing techniques to handle imbalanced datasets. Hyperparameters were fine-tuned using GridSearchCV and RandomizedSearchCV.<br>
- <b>Random Forest:</b> Used with class weights to address imbalance, with extensive hyperparameter tuning to enhance performance.<br>
- <b>Naive Bayes:</b> Applied Multinomial Naive Bayes for text classification.<br>

### Evaluation Metrics:

- Assessed models using Precision, Recall, F1-score, ROC-AUC, and confusion matrices to visualize performance and error distribution.<br>
### Deep Learning Models:

- <b>LSTM:</b>  Leveraged for sequence data such as text, utilizing Keras for model construction.<br>
- <b>Bidirectional LSTM:</b>  Enhanced context understanding by processing data in both directions.<br>
- <b>Attention Mechanism: </b> Incorporated to focus on significant input sequence parts for improved performance.<br>
### Evaluation and Techniques:

- Similar evaluation metrics as machine learning models were used, along with methods like early stopping and learning rate adjustments to fine-tune training.<br>
### Data Preprocessing and Feature Engineering:

- Tokenized text and used FastText vectors and TfidfVectorizer for feature extraction. Cleaned comments for noise reduction.<br>
- Applied SMOTE for class balancing and balanced class weights in models.<br>
- Utilized TruncatedSVD for dimensionality reduction and pipeline approaches for streamlined model training.<br>
### Imbalanced Data Handling Techniques:

- <b>Resampling: </b>Used SMOTE for oversampling and NearMiss for undersampling.<br>
- <b>Algorithmic Approaches:</b> Employed cost-sensitive learning and ensemble methods like Balanced Random Forest and EasyEnsemble.<br>
- <b>Anomaly Detection: </b>Treated minority classes as anomalies using One-Class SVM.<br>
- <b>Data Augmentation:</b> For image data, used transformations to boost minority class samples.<br>
