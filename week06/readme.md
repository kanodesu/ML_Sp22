## Week06
### Assignment:
You will be making changes to the starter code for final assignment 1 to show the effect of multiple alterations on a regularization parameter (the topic for this week’s class) on the various performance measures defined by Flach on page 57 and implemented in my_measures.py.

Your graph(s) will show multiple comparisons (at least five!) of different values (including the default value) for the alpha parameter of the Ridge() (Links to an external site.) class, for both the training and test sets. Values for alpha must be a positive float and larger values specify stronger regularization.  

<br>

### Result:
The default value for the alpha parameter of the Ridge() class is 1.0, and larger values specify stronger regularization.  In the experiment to change the regularization parameter in RidgeClassifier (Alpha), I tried to add "0" to the alpha values to see if there's a change in the result. The result doesn't change until alpha=10000. I tried 10000, 100000, and 1000000 first, and the best result among these there was alpha = 100000. Then I tried 70000 and 130000 next, and I think the best iteration of this experiment was alpha=70000.

Alpha default value:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week06/default.png "sketch1")

alpha=70000
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week06/70000.png "sketch1")
