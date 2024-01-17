Regularization

When you construct a neural network ypu can incur in overfitting.
Regularization is to fine tune the complexity of neural network: how can I 
construct a model that generalise in the best way possible on new and unseen 
data.
Any technique that made the model generalize better.
For example, you can regularize the loss function adding a regularization 
term.
When you kill a weight it's like you kill a connection between neurons.
Small weights can be a result of regularization. You are making the model
simpler. (Remember: weights are the coefficent of linear combination inside 
neurons, they combine inputs linearly to obrain outputs).
Slide 15: the overfitting is reduced as lambda increases.
Weights are going to zero as an exponential decay (mathematical explanation).
Regularization adds new hyperparameters (!!).

Regularization methods

Dropout
You remove neurons randomly after compute the loss function. So you are training
different networks.
Slides 25 and 27: they oscillate because I'm training different networks.

Early stopping

It stop the training before gets too bad (overfitting).

Additional methods
	-get more data: less overfitting (but be careful on what data!)
	-augmentation

