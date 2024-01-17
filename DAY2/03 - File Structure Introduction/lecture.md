Model validation

Checking whether your model is doing what you want to do or not (based on your
 reasearch question).
Model needs to satisy the following requirements:
	-speed
	-energy consuption
	-memory consuption

Overfitting: the model capture the noise present in the data. The model is too
complex that you learn noise and not data.
How can we detect overfitting?
the model evaluated on unseen data will have bad performance.

Cross-validation:
statistical methods to estimate the skill of ml model. Cross because you want
more statistical informations about the datasets. You divide datasets into
portions and test on another portion.

Model (cross)validation methods:

hold-out approach.
If the error on the new model is higher than the train, ypu are overfitting. 

You want the bias-variance trade-off. You can train your model for not long 
time in order to don't reach the overfitting.
Underfitting:model too simple that you cannot capture the structure of the 
data.

Stratified sampling:
	-shuffle
	-if the dataset is divided in classes you have to make sure that your
	 splitted dataset is representative of the original one

Data leakage
some information from test dataset come into the train dataset. The new 
trained dataset have information from original dataset. So it will an
impact on the performance. Are not 'unseen' data anymore.

Monte-Carlo cross validation
hold-out approach with multiple splits.
It is computationally heavy because you change the model N time. But it tells
you much more statistical information. In the hold-out you can be luky because
the split you done is luky. This method is the solution. Ypu have to make
sure the your model is good trained and this don't depend on 'lucky' data.
In this way you can study statistically the model performance.
You test the performance of N model on N datasets. 
If you would have only N dataset ypu would be in the situation of testing
one model on N datasets.
The higher is the dataset narrower is the MSE distribution (teo limite 
centrale).
The average is a good estimator, instead the standard deviation not.

This phase of splitting is only to calibrate your model. Then come back and 
test the model on the whole dataset without splitting.

K-fold approach
MC is expense, so use k-fold. Used when dataset is small.

Model selection
Choosing the most appropriate model from a set of models for a given dataset.
