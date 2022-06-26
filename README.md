# Yelp_Dataset_Challenge_NLP
Performing NLP tasks on Yelp dataset

**What's in the repo:**<br />
Text Mining for YELP dataset challenge 2015<br />
The dataset contains 650k training samples and 50k test samples. The dataset contains the reviews and ratings (from 1-5) by the customers for different restraurants that customers have visited and had their meals.<br />
All the required operations have been performed and described in below steps.<br /><br />
**Data Preprocessing** - <br />
    The data picked from csv and duplicates/nans have been removed<br /><br />
**Data Cleaning** - <br />
    - Removed all whitespaces <br />
    - Removed all punctuations<br />
    - Removing Contractions<br />
    - Removing Emoticons, digits<br />
    - Removing stopwords<br />
    - Performing Lemmatization on the words<br /><br />
**Data Visualization** -<br />
	- Plotting of histograms for each label with respect to the length of the reviews<br />
	- Plotting of bar chart showing distribution of reviews in each label<br />
	- Plotting unigram word frequencies<br />
	- Plotting bigrams word frequencies<br />
	- Plotting unigram word frequencies in each label<br /><br />
**Model Building and Training** - <br />
	- Two models based on Tensorflow have been created and trained- LSTM and Simple RNN<br />
	- Pretraining stuffs related to texts have been performed here like Tokenizer, sequencing, padding etc.<br />
	- Plotting of history from both the models showing the training and validation accuracy-loss.<br /><br />
**Model Prediction and Evaluation** - <br />
	- Predicition on test set<br />
	- Plotting of confusion matrices for both the models<br />
	- Logging all the TPs, TNs, FPs, FNs for both the model<br /><br />
**Steps to reproduce the notebook:**<br />
	- Set the path to the dataset (TRAIN_CSV and TEST_CSV) in the inital lines of the code (comments have been provided for each of them)<br />
	- Set the number of records you want to run for both training and test data. This is because running the whole dataset is too slow and a never ending process on colab. It's helpful if you have acces to some bigger GPUs.<br />
	- Run from the training heading if you have already the filtered data. Just give the path to the filtered dataset under the keys- TRAIN_CSV_FILTERED and TEST_CSV_FILTERED.<br /><br />
