# deep-learning-challenge
Challenge 21-Analysis

## Overview
The purpose of the analysis done in this challenge is to see if it is possible to predict a successful outcome of funding a particular charity venture.  Due to the large number of variables involved, a neural network analysis will be very helpful in finding if this is possible or not.

## Results

#### Data Preprocessing
* Target variable for this model is the successful outcome measure
* The feature variables for this model are: application type, classification, use case, organization type, income amount, and ask amount
* The variables not used are: EIN, name, status, and special considerations

#### Compiling, Training, and Evaluating the Model
* Initially the model had two hidden layers with six nodes each.  This was the initial configuration because that was one that was commonly used in class examples and so it was a configuration I was comfortable using and knew would work as a baseline
* I was ultimately not able to achieve the target performance, though I was able to come within approximately 1% accuracy
* To improve the model, I added two more hidden layers and increased the amount of nodes per layer several times
* I also tried some other activation functions from the list in the keras documentation

## Summary
Overall, the model I ended up with was nearly as accurate as required.  I found that after a certain point, adding more layers and nodes did not make appreciable change on the accuracy of the model.  I think the next step would be to try either removing some of the variables to see if there are some that have no impact but convolute the model, or to try creating fewer bins to put the non-numerical variables in.  This would require a more significant time investment as it is more complicated than updating the nodes and layers of the model.  
