# Tweet Similarity Analysis with Transformer Embeddings

## Introduction
In the digital age, understanding the semantic similarity between tweets has become increasingly important for various applications such as user profiling, content recommendation, and fake news detection. This project aims to develop a model capable of analyzing the semantic similarity between two tweets and providing a similarity score indicating the likelihood that they were authored by the same user. We leverage transformer-based models for text representation and distance calculations to achieve this goal.

## Project Outline
1. **Data Preparation:**
   - Randomly sample pairs of tweets from the dataset.
   - Ensure a balanced representation of pairs from the same user and different users.
   - Assign similarity labels to each pair (1 for same-user pairs, 0 for different-user pairs).
   
2. **Data Preprocessing:**
   - Lowercase all text.
   - Remove punctuation, symbols, and special characters (keeping hashtags and mentions).
   - Tokenize tweets into individual words.
   - Explore options like stop word removal and stemming/lemmatization.

3. **Model Architecture:**
   - Utilize a pre-trained embedding layer or train one with the model.
   - Select a pre-trained transformer model suitable for text similarity tasks which is BERT.
   - Pass preprocessed text through the transformer encoder.
   - Calculate Manhattan distance between tweet representations.
   - Add a dense layer with a sigmoid activation function to produce a similarity score.

4. **Evaluation:**
   - Evaluate model performance using precision, recall, and F1 score on the testing set.

## Usage
1. Clone the repository:
git clone https://github.com/kawther1010/tweets.git


2. Install required packages:

3. Open and run `main.ipynb` in Jupyter Notebook or any Python environment.

## Results
- Precision: 0.6
- Recall: 0.5
- F1 Score: 0.5454545454545454

## Conclusion
This project successfully develops a model for tweet similarity analysis using transformer embeddings. By leveraging transformer-based architectures and distance calculations, the model demonstrates promising results in identifying semantically similar tweets. The insights gained from this project can be valuable for various applications in social media analytics and natural language processing.
