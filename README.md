# Natural Language Processing NLP - Sentiment-Analysis

### About: 
Sentiment analysis conducted on tweets written by customers from 6 major U.S. airlines 

### Sentiment Analysis Context
The term "Sentiment Analysis" was coined by Nasukawa et al. in 2003. The esential issue in Sentiment Analysis is to identify how sentiments are expressed in texts and whether the expressions indicate positive or negative opinions about a particular subject, and this in term requires identification of sentiment expressions, polarity and strenght of expressions and their relationship to the subject.

### General Objective: 
To conduct a Sentiment Analysis on the tweets written about major U.S. Airlines by implementing the techniques learned as a part of the subject "Natural Language Processing".

### Specific Objectives: 
- SO1) Demonstrate basic understanding of text pre-processing, 
- SO2) Provide practical application of the process after pre-processing, 
- SO3) Apply Bag of Words, 
- SO4) Apply Tf-idf, 
- SO5) Build classification models, 
- SO6) Evaluate models, 
- SO7) Summarize the understanding of application of the various techniques on the dataset.

### Key Questions: 
- KQ1) Can we predict whether a tweet contains positive, negative or neutral sentiment about a particular airline?, 
- KQ2) Can analysis/classification of tweets help Airlines to detect negative social mentions that could harm their business?, 
- KQ3) Which pre-processing techniques are more suitable cleaning procedures to to reduce noise text and to make sure they are suitable for machine learning modeling?

### Learning Outcomes: 
- LO1) Basic understanding of text pre-processing, 
- LO2) What to do after text pre-processing, 
- LO3) Bag of words, 
- LO4) Tf-idf, 
- LO5) Build the classification model, 
- LO6) Evaluate the Model

### Code:
- The code was written and tested with Python 3.8 in a jupyter notebook 
- The jupyter notebook includes a table of contents with all information about Python libraries needed
- The process is also explained in detail in the jupyter notebook
- The dataset is identified as "Tweets.csv" 

### General Process:
The Sentiment Analysis Process is depicted in the figure below:

![General Process](https://github.com/onofre2021/NLP--Sentiment-Analysis-Twitter-US-Airlines-/blob/main/Sentiment%20Analysis%20Process%20(JLOrtizV).jpg)

Sentiment Analysis is one of the text analysis applications for machine learning algorightms that is the subject of this project.

As raw text data cannot be fed directly to the machine learning algorithms, we need to convert them in numerical feature vectors with a fixed size rather than the raw text documents with variable lenght. Turning a collection of text documents into numerical feature vectors is called "vectorization".

There are various ways to extract numerical features from text content such as "Bag of Words" or "Bag of n-grams" which covers: tokenizing, counting ocurrences of tokens and normalizing/weighting with disminihing importance tokens that ocurr in the documents.

There are other text feature extraction techniques provided by scikit-learn such as: Sparcity, CountVectorizer, stop words, Tf-idf term weighting, decoding text files, HashingVectorizer. We are going to apply several of these in the execution of this project but more information is available in the following link:

https://scikit-learn.org/stable/modules/feature_extraction.html


### Detailed Processs:
<ol>
  <li>Import all necessary libraries</li>
  <li>Load the subject dataset</li>
  <li>Data Summmary (shape, description)</li>
  <li>Exploratory Data Analysis
    <ol>
      <li>Plot the distribution of all tweets among each airline & plot the distribution of sentiment across all the tweets</li>
      <li>Plot the distribution of Sentiment of tweets for each airline & plot the distribution of all the negative reasons.</li>
      <li>Plot the distribution of Sentiment of tweets for each airline & plot the distribution of all the negative reasons.</li>
    </ol>
  </li>
  <li>Plot the word cloud graph of tweets for positive and negative sentiment separately.</li>
  <li>Understanding of Data Columns.
      <ol>
      <li>Drop all other columns except "text" and "airline_sentiment"</li>
      <li>Check the shape of the data</li>
      <li>Print the first 5 rows of data</li>
    </ol>
    </li>
  <li>Plot the word cloud graph of tweets for positive and negative sentiment separately.</li>
  <li>Data Pre-processing.
      <ol>
      <li>Apply all necessary pre-processing steps and print the first few rows of data after pre-processing.</li>
      <li>Html tag removal</li>
      <li>Tokenization</li>
      <li>Remove the numbers</li>
      <li>Removal of special characters and punctuations</li>
      <li>Replace contractions in string. (e.g. replace I'm --> I am) and so on.</li>
      <li>Removal of stopwords</li>
      <li>Conversion to lowercase</li>
      <li>Lemmatize or stemming</li>
      <li>Join the words in the list to convert back to text string in the data frame (so that each row contains the data in text format)</li>
      <li>Print the first 5 rows of data after pre-processing</li>
      <li>Note: Each pre-processing function will be applied on the required column one at a time and print the first few rows after applying the function</li>
      </ol>
      </li>
  <li>Vectorization - Apply count vectorizer, Tf-IDF vectorizer on the required text column to make it suitable for fitting the model</li>
      <ol>
      <li>Use CountVectorizer</li>
      <li>Use TfidfVectorizer</li>
      </ol>
 <li>Modeling, Tuning and Evaluation  
      <ol>
      <li>Fit the model using vectorized column</li>
      <li>Tune the model (optimize the parameters to improve the accuracy)</li>
      <li>Evaluate the model using both types of vectorization using the confusion matrix.</li>
      <li>Print the top 40 features and plot their word cloud using both types of vectorization</li>
      <li>Unsupervised Learning Methods: VADER Sentiment and TextBlob</li>
      <li>Machine Learning Model Creation for Classification: Random Forest</li>
      <li>Test Data Transformation</li>
      <li>Model Evaluation</li>
      </ol>
      </li>
<li>Conclusion - Summary from the understanding of the application of various pre-processing, vectorization and performance of the model on the dataset</li>   
