## Week10
### Assignment:
You will be making changes to the starter code for final assignment 2 to show the effect of multiple alterations on the hidden_layer_sizes parameter for a neural network (a.k.a. Multi-layer Perceptron in scikit-learn). You will show the results of different image feature set representations on the various performance measures defined by Flach on page 57 and implemented in my_measures.py. Changes to the hidden_layer_sizes parameter should be the only variable in your experiment; hold constant all other variables (such as feature set representation and other parameters). 

Your graph(s) will show multiple comparisons (at least five!) of different values for the hidden_layer_sizes parameter, for both the training and test sets. The input is a tuple, which conveys both the number of layers and the number of neurons within each layer. For example, the default value of default=(100,) adds a single hidden layer with 100 neurons in that layer. A tuple of (20, 15, 10) would add three hidden layers, with 20 neurons in the first layer, 15 neurons in the second layer, and 10 neurons in the third layer. 

### Result:
This week's assignment is to change the hidden_layer_sizes parameter in neural network. I first tried to compare with different neurons in a single layer, and I tried hidden_layer_sizes = (100,), and (1000,). The result turned out that hidden_layer_sizes = (1000,) had a better performance, but it's a really slightly change.

Then I started to add more layers in the network, I tried four different times, hidden_layer_sizes=(100,50,25), (100, 50, 25, 10), (50,20,20), and (20,20,). I still got some quite similar results, except for the last one. Maybe it's because the last one has the least number of layers and also the least amount of neurons in each layer.

Results in total:
![sketch1](https://github.com/kanodesu/ML_Sp22/blob/main/week10/Screen%20Shot%202022-04-19%20at%2014.47.18.png "sketch1")
