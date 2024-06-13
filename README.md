
# Group-3

## Hate Speech Detection on the Reddit platform

### Description

With the rise of social media, people have the liberty to express themselves, many users misuse this liberty and we can see abuse, offense, and hate spread all across social media platforms, in the form of comments, blogs, etc. This project aims to create a deep-learning model to automatically detect and classify hate speech in text, promoting healthy interactions on Reddit.

### Datasets
<<<<<<< HEAD
<b>Preprocessed DatasetLink :</b> https://drive.google.com/drive/folders/1uJnUbNHYbTXL4nOLgki3kHIhFD6HgKCu?usp=sharing

<b>Original Dataset Link :</b> https://github.com/jing-qian/A-Benchmark-Dataset-for-Learning-to-Intervene-in-Online-Hate-Speech
=======

#### Original Dataset - Reddit

The dataset is imported from A Benchmark Dataset for Learning to Intervene in Online Hate Speech. 
<p><b>Link:</b> https://github.com/jing-qian/A-Benchmark-Dataset-for-Learning-to-Intervene-in-Online-Hate-Speech</p>
<p>The dataset includes approximately 5,000 posts and comments. Each row contains a specific post's comments and an index indicating which comments are considered hate speech. Additionally, the dataset features human-written explanations for why these comments are classified as hate speech.</p>

#### Preprocessed Dataset

The preprocessed dataset files are stored in Google Drive
<p><b>Link:</b> https://drive.google.com/drive/folders/1uJnUbNHYbTXL4nOLgki3kHIhFD6HgKCu?usp=sharing</p>

##### Restructured Reddit

<p>The dataset has been restructured so that each row contains only one comment. If a comment is hate speech, it is indicated with a hate_speech value of 1; otherwise, it is marked as 0. The responses column has been removed.</p>

##### Reddit Cleaned

<p>The dataset contains NaN values and comments marked as [deleted] or [removed]. These comments are dropped to clean the dataset.</p>

##### Reddit Preprocessed

<p>The dataset undergoes preprocessing to prepare it for training. This involves several steps such as converting text to lowercase, removing HTML tags and URLs, eliminating stop words and punctuation, handling numbers and autocorrecting, treating chat words, managing emojis, and performing tokenization, stemming, and lemmatization.</p>
>>>>>>> main
