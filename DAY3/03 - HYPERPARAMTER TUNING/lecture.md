Hyper-parameter tuning

Any ML model has many parameters. How can we choose the parameters that give me 
after treaining the best model without overfitting?
Training different models with different parameters and then compare 
performance.
Hyperparameter is not depending on the dataset. Hyperparameter is not 
necessary a number: continous, discrete and can assume infinite number of
values, discrete and can assume finite number of values (e.g. activation
functions or normalization approaches).
Model usually depend mostly on learning rate (usually set to 10^-4/10^-3).
You start trying from the one that has more influence on the model, so
learning rate, epochs, ecc..
Hyperparameters are not modiefied by the training of the data, are not
modified by the gradient descendent.

Chosing hyperparameters is a problem because is a black-box optimisation.
I can only evaluate NN, but I don't know what function it is, I don't know
what exactly is.
Two types of BB functions:
	-cheap ones
	-costly ones

Grid search: you try all the values.It is expensive because you evaluate the
model many times (maybe you can use it on cheap fnctions.

Random search: as grid seacrh but you don't sample all the points in the
range.

Coarse to fine optimisation: first you do random search, you find candidate 
and take small interval around the candidate and then search again a 
candidate. Repeat the process. The problem is that you have to find a good
candidate  in the first search.

Sampling on a logarithmic scale: grid search with not equally spaced points but
logarithmic.
