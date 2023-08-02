# deep-learning-challenge

### Repo contents

This repo contains our data ("charity_data.csv") and our notebook, as well as the saved .h5 versions of our model.
There are several models, which represent different shapes of neural net.
The last version developed is coded "5-50 mix", which represents 5 hidden layers with 50 nodes each.

## Report

### Overview
The purpose of this analysis was to develop a neural net machine learning model that could predict if a campaign was going to be successful or not.
The target variable is the "IS_SUCCESSFUL" variable
We removed the "NAME" and "EIN" variables because they are not features in the model

We tested several node, layer, and epoch combinations, but with different activations through the layers and Sigmoid for the final layer.
The model was not much more accurate with more nodes or epochs - 15 nodes was a balanced limit and 15 epochs was not really different from 100.
The model was ever so slightly more accurate with more layers but stopped improving between 4 and 5
The final model contains 5 layers with 15 nodes, run over 15 epochs.

### Results

I was not able to achieve the 75% target. I got to ~73% with all combinations of activations, layers, nodes, etc.
Model performance was tweaked with the various hyperparameters, but the results were all pretty similar.

### Summary

One issue faced in this project was that Tensorflow crashed the Python kernels on VS Code. I was not able to rectify the issue with lower versions of Tensorflow or other approaches.

The result of this model was 72.8% accuracy. This was close to the maximum accuracy achieved through all the attempts.

It is possible that this is not the right model to approch the data with. I might try a different model, such as XGBoost, if I were to attempt this again.