# classification-of-english-words-into-CEFR-levels
The files in this repository are the outcomes of a research project. We introduced a method that automatically classifies English words into their Common European Framework of Reference (CEFR) levels based on word complexity factors. The words and their CEFR levels from The Oxford 5000 word list were used to train the model: https://www.oxfordlearnersdictionaries.com/wordlists/oxford3000-5000

Please note that we ignored the C2 level since it is not present in The Oxford 5000.

The content of the folders is as follows:

**features:**
* The file demonstrating the data and the initial 45 features used in the machine learning methods before the feature selection and EDA process.


**data analysis:** 
*	The applied EDA and feature selection techniques: univariate analysis (bar charts), correlation analysis, bivariate analysis (box plots), mutual information, Fisher score, variance threshold, analysis of variance (ANOVA), random forest importance, and LASSO Regularization. (The features selected using the variance threshold method with a threshold of 0.2 achieved the best performance in the classification method.)

**XGBoost:**
*	The Jupyter Notebook file for the XGBoost classification method to predict CEFR levels of words. We used this method to classify 14,000 new words that have not been classified before. The model has an accuracy of 54.48%, using 10-fold cross-validation, and 70% precision for the A1 and C1 levels.
*	The dataset of selected features to train and test the model.
*	The csv file for unclassified words.


**all classification methods:**
*	The other classification methods used in our research which performed worse than XGBoost in terms of accuracy.
*	The dataset of selected features to train and test the model.


**datasets:**
*	The collection of the datasets required to run all of the ipynb files.

**classified_dictionary_for_14K_words.csv** is a dictionary containing 14,000 words, not included in The Oxford 5000, classified into their CEFR levels using the methods and features we introduced. The words and their definitions are taken from:  https://www.kaggle.com/datasets/dfydata/the-online-plain-text-english-dictionary-opted?resource=download

**created by:**

Eylül Appak- https://github.com/eylulappak

Esra Alın- https://github.com/esralin
