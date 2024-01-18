Errors in labels

What are the effect of error in the labels?
look at slides and paper linked into slides.
Regression is when you want to estimate for example parameters of your model
(so the parameters are the labels). Classification is when you want to assess
a label for example to an image.
In the first case you use MSE to understand if your model is good or bad, in 
the second one the accuracy.
You do the same as previous days ( arcchitecture, loss function ecc..). 
From the loss function you have an estimate of MSE, so here you have to take
into account of error labels. For the MSE you have to sum the gaussian 
varinace to the MSE estimate. (If the error is not gaussian distributed?).
The error is the error of the labels and not of the NN model. It's like
error on gw parameters (I think).
