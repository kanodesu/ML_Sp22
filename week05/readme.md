## Week05
### Assignment:
You will be making changes to the starter code for final assignment 1 to show the effect on one or more alterations on feature selection, extraction, and transformation (the topic for this week’s class) on the various performance measures defined by Flach on page 57 and implemented in my_measures.py.

Your graph(s) will be showing the before/after comparison of the starter code before you make any changes, to the code after you have made one or more changes in the process_raw_data function, which can include one or more alterations on one or more of the following scki-kit learn classes/modules: 

CountVectorizer , including Bi-grams and other n-grams (Links to an external site.)
* HashingVectorizer
* TfidfTransformer 
* The creation of Polynomial features 
* Any other feature extraction method or module for text
* Any other alteration related to feature selection, extraction, and transformation, which can include the addition/removal of features

The changes can be to the addition/removal of any of the classes/modules listed above and/or alterations to values for parameters within any of the classes/modules listed above. 

<br>

### Result:
I choose to do the movie review dataset. In the starter code, I noticed that in the `process_raw_data function`, the original code used `HashingVectorizer` module to convert a collection of text documents to a matrix of token occurrences. Instead of using `HashingVectorizer`, I used the `CountVectorizer` to convert a collection of text documents to a matrix of token counts. It can count the frequency of each word that occurs in the entire text and build a vocabulary of known words, and also to encode new documents using that vocabulary. Maybe the good movie reviews shared some common words, and thus we can predict the test sets. The result of the seven different models is quite similar except for `Random Forest Classifie`r model.

Screenshot of ROC plots for train set before:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week05/Screen%20Shot%202022-03-07%20at%2019.39.00.png "sketch1")

Screenshot of ROC plots for train set after:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week05/Screen%20Shot%202022-03-07%20at%2019.39.41.png "sketch1")

Screenshot of ROC plots for test set before:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week05/Screen%20Shot%202022-03-07%20at%2019.40.09.png "sketch1")

Screenshot of ROC plots for test set after:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week05/Screen%20Shot%202022-03-07%20at%2019.40.16.png "sketch1")
