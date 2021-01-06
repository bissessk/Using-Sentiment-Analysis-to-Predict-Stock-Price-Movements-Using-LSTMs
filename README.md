# The Effect of Sentiment Analysis on Stock Price Prediction using LSTMs
**Kieran Bissessar and Efrain Galarza**

---

## Data Files
* `appleNextDayNorm.csv` 
* `appleNextDayNotNorm.csv`
* `appleSameDayNorm.csv`
* `appleSameDayNotNorm.csv`
* `djiaNextDayNotNorm.csv`
* `djiaSameDayNotNorm.csv`
* `msftNextDayNorm.csv`
* `msftNextDayNotNorm.csv`
* `msftSameDayNorm.csv`
* `msftSameDayNotNorm.csv`

The data files mentioned in this list were used to test our models. We used data from two companies (Apple and Microsoft) and one index (DJIA)

NextDay or SameDay refers to whether we were trying to predict the stock price change for the same day as the sentiment, or for the next day

Norm or NotNorm refers to whether we used the normalized labels or not 

---

## Notebooks
* Data Prep
	* `dataExplorationipynb.ipynb`
	* `dataProcessingStockNewsNLP.ipynb`
	* `RedditNewsCleanUp`
* LSTMs
	* `nextDayNormLSTM.ipynb`
	* `nextDayNotNormLSTM.ipynb`
	* `sameDayNormLSTM.ipynb`
	* `sameDayNotNormLSTM.ipynb`

The files under *Data Prep* were used to construct and visualize the data. This includes using nltk to retrieve polarity scores.

The files under *LSTMs* were used to run the results of the associated datasets on different types of LSTMs. Unidirectional and Bidirectional LSTMs were evaluated. Also the dropouts, learning rate, and stacked layers were experimented with directly on the file by commenting out the necessary lines.

A total of 96 comparisons were made using these files. These were made by varying the types of datasets, number of layers, types of layers, and dropouts.
