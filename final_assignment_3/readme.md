## Final Assignment 03 (option 2)

### Assignment:

You are going to use [KMeans](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) to cluster a set of images **on their metadata.** The measure of success is subjective; you know you have chosen the right features and number of clusters when the images in each cluster "seem" like they belong together. 

Your work will be assessed on: 
1. data processing and transformation  
2. choosing the right number of clusters for the problem  
3. the organization and documentation of your GitHub repository  
4. communication of your work in class reflections and final presentations  
5. model improvement over the semester

### Solution
#### Choose features
In addition to the seven visual variables defined by Bertin, I also added variables like `kinetic`, `spatial_dimension`, and `reflection`.
At first, I tried to include variables such as `primary_medium`, but the kmeans could not read the string, and could not convert string to float. I might need to transform the medium categories to number/boolean ahead to let the kmeans read the data. So I only picked the variables that are numbers or booleans.

```python
X = data[['kinetic', 'spatial_dimension','reflection','pl', 'si', 'va', 'te', 'co', 'or', 'sh']]
```
<img src="https://github.com/kanodesu/ML_Sp22/blob/main/final_assignment_3/img/Screen%20Shot%202022-05-02%20at%2019.41.42.png">

#### Find cluster numbers
From the inertia score plot, I think the ideal cluster numbers is range from 5 - 30.
<img src="https://github.com/kanodesu/ML_Sp22/blob/main/final_assignment_3/img/Screen%20Shot%202022-05-02%20at%2019.59.21.png">
So I tried from `range_n_clusters = [5, 8, 11, 14, 17, 21, 25, 29]`, and find out the best result is when n_clusters = 11.
<img src="https://github.com/kanodesu/ML_Sp22/blob/main/final_assignment_3/Screen%20Shot%202022-05-08%20at%2022.33.48.png">

#### Results
Some of the clusters with images:
<img src="https://github.com/kanodesu/ML_Sp22/blob/main/final_assignment_3/Frame%203.png">
<img src="https://github.com/kanodesu/ML_Sp22/blob/main/final_assignment_3/Frame%202.png">
Cluster 8 is my favourite cluster, I like these contemporary/abstract artworks that kind of showed the opposite of life.




