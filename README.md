# SentimentAnalyzer
Sentiment Analyzer with RapidMiner that
- Collects latest film reviews from a website (scraping)
- Process the reviews. Tokenizing, removing stopwords and outliers and stemming.
- Analyze data and generated a Naive Bayes and a Support Vector Machine model.
- Using the model generated in the last step, predicts the sentiment of new films reviews.

### Data
Holds part of data that will be processed

The **pang_lee** folder contains the training and test data

The **filmaffinity** folder contains manually downloaded data to do predictions

### Process
Contains all the RapidMiner files.

The **generator** process takes the data from the data folder and trains and tests a model

The **optimizer** process iterates the same model with differents parameters to find the best one

The **scraper** process downloads new film reviews from www.rottentomatoes.com to do predictions

The **predictor_rottentomatoes** does predictions to the downloaded film reviews from that page

The **predictor_filmaffinity** does predictions to the manually downloaded film reviews from the filmaffinity data folder



