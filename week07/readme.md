## Week07
### Assignment:
You will be making changes to the starter code for final assignment 1 to show the effect of multiple alterations on a margin size parameter (C) for the Support Vector Machines classifier (SVC) in scikit-learn. You will show the results of different values for the C parameter in the SVC class on the various performance measures defined by Flach on page 57 and implemented in my_measures.py. 

Your graph(s) will show multiple comparisons (at least five!) of different values (including the default value) for the C parameter of the SVC class, for both the training and test sets. Values for C must be strictly positive. Smaller values of C correspond with larger (a.k.a. “softer”) margins (see this example). 
<br>

### Result:
At first, I tried the SVC model, but my computer can't run and get a result from it. So I switched to LinearSVC model. I started with the default value, C=1.0, and then tried bigger number such as 100, 10000, and smaller number such as 0.001, 0.00001 and 0.000000000001. But I didn't see a difference in the result. The final accuracy and precision is actually pretty good, but I can't figure out why I can't get a different result by trying different C values in the model.

Train set:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week07/Screen%20Shot%202022-03-29%20at%2023.01.03.png "sketch1")
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week07/Screen%20Shot%202022-03-29%20at%2023.01.10.png "sketch1")
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week07/Screen%20Shot%202022-03-29%20at%2023.01.18.png "sketch1")

Test set:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week07/Screen%20Shot%202022-03-29%20at%2023.01.27.png "sketch1")
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week07/Screen%20Shot%202022-03-29%20at%2023.01.34.png "sketch1")

