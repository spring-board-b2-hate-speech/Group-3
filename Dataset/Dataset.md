
# Dataset

## Original Dataset - Reddit

The dataset is imported from A Benchmark Dataset for Learning to Intervene in Online Hate Speech. 
<b>Link:</b> https://github.com/jing-qian/A-Benchmark-Dataset-for-Learning-to-Intervene-in-Online-Hate-Speech
<p>The dataset includes approximately 5,000 posts and comments. Each row contains a specific post's comments and an index indicating which comments are considered hate speech. Additionally, the dataset features human-written explanations for why these comments are classified as hate speech.</p>

## Restructured Reddit

The dataset has been restructured so that each row contains only one comment. If a comment is hate speech, it is indicated with a hate_speech value of 1; otherwise, it is marked as 0. The responses column has been removed.

## Reddit Cleaned

The dataset contains NaN values and comments marked as [deleted] or [removed]. These comments are dropped to clean the dataset.

## Reddit Preprocessed

The dataset undergoes preprocessing to prepare it for training. This involves several steps such as converting text to lowercase, removing HTML tags and URLs, eliminating stop words and punctuation, handling numbers and autocorrecting, treating chat words, managing emojis, and performing tokenization, stemming, and lemmatization.
