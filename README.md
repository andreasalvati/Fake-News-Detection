# Predicting Coca Cola Earnings

The objective is to apply NLP tecniques to classify fake news

## Analysis Goals

We will hereby quickly summarize the flow of the work. The main steps we took will be briefly described below. At first, we imported the data and started preparing it to be suitable for analysis (after having performed some EDA). The main steps in the preparation were cleaning and preprocessing using vectorizers to get the data into a suitable format for processing it with the chosen algorithms. The cleaning was performed for the most using bs4 BeatifulSoup.

Before the modelling phase though, there are two more steps, lemmatization being the first one. Lemmatization helps to achieve greater precision in the modelling stage as it considers the root of the word and not the word itself. On top of this, we decided to adopt a Chi Square test for feature selection so to make processing leaner and more efficient, while isolating noise and achieving better results.

The modelling phase consisted of iteratively running the same models multiple times with different input data (in terms of preprocessing) to discover what treatment generated the best results. Naive Bayes, Support Vector Machines and Logistic Regression (MaxEnt) were the models we adopted to classify the news as fake or real. The best results were achieved while running the optimized SVM model where the accuracy was as high as 0.9458, when the input was the data preprocessed through lemmatization, Chi Square and TF-IDF. Below a summary of the results achieved in the different models.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
