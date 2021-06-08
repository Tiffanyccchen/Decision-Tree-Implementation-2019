# Decision Tree Implementation - 2019

## Introduction
I extend the toy example of a decision tree offered by the amazing Google Developer [Josh Gordon](https://github.com/random-forests).  
The [tutorial video](https://www.youtube.com/watch?v=LDRbO9a6XPU) have a brief introduction.

The extension I made are : 
Part | Original | Extension
:--- | :--- | :--- 
Number of Split | 2 | Numerical variable : 2 / Nominal variable : Number of Levels
Stopping Criteria | Attributes in a leaf are the same | < 3 samples in a Leaf, Class is identical in a Leaf
Splitting Criteria | Gini Index | Gini Index, Gain Ratio, [AUC](http://dmip.webs.upv.es/papers/ICML2002.pdf) 
Evaluation | No | 4-fold CV, indexes : accuracy / recall/ precision/ F1 score
Classification Criteria | Highest-proportion class | Highest weighted propotion (weights : divide by the class's propotion in the training data)
  
## Structure
* decision_tree : toy example by Josh Gordon
* decision_tree_expand : expanded implementation by me

## Notice
I use the postoperative.txt data as input.  

However, by writing a proper data reading code (which can be finished in seconds),  

This Decision Tree can classify ANY TYPE of data!
