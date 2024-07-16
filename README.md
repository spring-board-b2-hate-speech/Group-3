# Group-3

# Hate Speech Detection on the Reddit platform

## Description

With the rise of social media, people have the liberty to express themselves, many users misuse this liberty and we can see abuse, offense, and hate spread all across social media platforms, in the form of comments, blogs, etc. This project aims to create a deep-learning model to automatically detect and classify hate speech in text, promoting healthy interactions on Reddit.

## Datasets

### Original Dataset - Reddit

The dataset is imported from A Benchmark Dataset for Learning to Intervene in Online Hate Speech. 
<p><b>Link:</b> https://github.com/jing-qian/A-Benchmark-Dataset-for-Learning-to-Intervene-in-Online-Hate-Speech</p>
<p>The dataset includes approximately 5,000 posts and comments. Each row contains a specific post's comments and an index indicating which comments are considered hate speech. Additionally, the dataset features human-written explanations for why these comments are classified as hate speech.</p>

### Preprocessed Dataset

The preprocessed dataset files are stored in Google Drive
<p><b>Link:</b> https://drive.google.com/drive/folders/1uJnUbNHYbTXL4nOLgki3kHIhFD6HgKCu?usp=sharing</p>

#### Restructured Reddit

<p>The dataset has been restructured so that each row contains only one comment. If a comment is hate speech, it is indicated with a hate_speech value of 1; otherwise, it is marked as 0. The responses column has been removed.</p>

#### Reddit Cleaned

<p>The dataset contains NaN values and comments marked as [deleted] or [removed]. These comments are dropped to clean the dataset.</p>

#### Reddit Preprocessed

<p>The dataset undergoes preprocessing to prepare it for training. This involves several steps such as converting text to lowercase, removing HTML tags and URLs, eliminating stop words and punctuation, handling numbers and autocorrecting, treating chat words, managing emojis, and performing tokenization, stemming, and lemmatization.</p>

#### Data Files

<p>chat_words.json: Contains chat word abbreviations and their corresponding meanings.</p>
<p>number_meanings.json: Contains special number meanings and their interpretations.</p>

#### Reddit Tokenization

<p>The dataset includes tokenized and lemmatized text data from Reddit comments, ensuring that each word is broken down to its base form.</p>

#### Data Splits

<p><b>Train: </b> Contains the training data used to train the models.</p>
<p><b>Test</b> Contains the test data used to evaluate the models.</p>

#### Encoded Datasets

<p><b>Train Encoded:</b> Contains the encoded version of the training data, transformed using FastText or BERT embeddings as appropriate.</p>
<p><b>Test Encoded:</b> Contains the encoded version of the test data, similarly transformed.</p>

<p>To ensure the integrity and validity of our model evaluation, the encoding process was performed separately on the training and test datasets. This prevents any potential leakage of patterns between the training and test data, ensuring that our model's performance metrics are accurate and reliable. </p>

## Tokenization 

<p>On the preprocessed dataset, we performed word tokenization to break down the text into individual words. Following this, we applied lemmatization to convert each word to its base form, which helps reduce inflectional forms and variations to a common base.</p>

## Encoding

<p>After tokenizing the sentences, we utilized FastText to encode the words into dense vector representations. This encoding process is crucial for transforming the text data into a numerical format that can be effectively used for training our machine learning model.</p>

## Evaluation Metrics

<p>Our key evaluation metrics for this hate speech detection project are accuracy and F1 score. We chose accuracy because it provides a straightforward measure of how often our model correctly classifies hate speech and non-hate speech instances. However, considering the imbalanced nature of hate speech data, where instances of hate speech are typically less frequent than non-hate speech, we also included the F1 score. The F1 score offers a balance between precision and recall, making it a more informative metric for assessing the model's performance in minority classes. This ensures that our model not only predicts accurately but also performs well in identifying and classifying instances of hate speech.</p>

## Machine Learning Models

<p>We implemented various machine learning models to identify hate speech, including:</p>
<pre>Linear Regression
Logistic Regression
Gradient Boosting
K-Nearest Neighbour
SGD Classifier
Random Forest
Support Vector Machine (SVM)
Voting Classifier</pre>
<p>After evaluating the performance of these models, we chose the Support Vector Machine (SVM) because it delivered superior results compared to the other models. Following the selection, we performed hyperparameter tuning on the SVM to optimize its parameters for better performance. The final results yielded an accuracy score of 82% and an F1 score of 66% for hate speech detection. These scores were set as our benchmark for evaluating deep learning models, ensuring that any deep learning approach we test meets or exceeds these performance metrics.</p>

## Deep Learning Models

<p>We explored several deep learning models for hate speech detection, including:</p>
<pre>Simple Neural Network (NN)
Convolutional Neural Network (CNN)
Long Short-Term Memory Network (LSTM)
BERT</pre>
<p>To enhance the performance of these models, we implemented techniques such as early stopping and learning rate reduction. For the Simple NN, CNN, and LSTM models, we utilized FastText encodings to represent the input text. However, for the BERT model, we used BERT embeddings, which provide more context-aware representations of the text. 
The performance metrics for the Simple NN, CNN, and LSTM models were similar, achieving an accuracy of 85% and an F1 score of 71% for hate speech detection. In contrast, the BERT model outperformed the others, achieving an accuracy of 89% and an F1 score of 89%.
Based on these results, we selected BERT as our final model for hate speech detection and saved this model for further implementation and deployment.</p>

### The individual implementations of the models can be found in separate branches of the repository. Each team member experimented with different approaches and models, and we decided to use the best methods from these individual efforts.
