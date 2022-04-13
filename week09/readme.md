## Week09
### Assignment:
You will be making changes to the starter code for final assignment 2 to show the effect of multiple alterations on the feature set for a neural network (a.k.a. Multi-layer Perceptron in scikit-learn). You will show the results of different image feature set representations on the various performance measures defined by Flach on page 57 and implemented in my_measures.py. 

Your graph(s) will show multiple comparisons (at least three!) of different feature set representations (including the default representation in the starter code), for both the training and test sets. This Jupyter notebook can be used as a sandbox for experimenting with various feature set representations in scikit-image. 

### Result:
I tried with canny, harris corner, and the shape index feature that I tried in class, and I changed percentage of downscaling the images from 50% to 25%. For canny feature, I changed the sigma value of it from 01. to 3, and I think when sigma = 2, it gets the best result. The result of shape index feature is pretty good, but I got an error message at the X_test_submission.shape part, so I cannot get a prediction result from it.



