Transfer learning

Can I used a network already trained (base model) to generate features on my 
own?
I remove some layers from the trained network and I add some other layers to
train. In such a way you already have features that you can use for the
layesr that you add subsequently. The layers that you add are less than the 
ones in the starting network, so more efficient for example for 
number of parameters.
You have pieces of network that ypu can extract, frozen, unfrozen ecc..It's 
like in autoencoders.
Anyway you have to train the model on all the layers (also the ones frozen).
It can be slow.
Thus you can generate a new dataset with the frozen part (frozen weights) of 
the base network and then  you have a featire dataset and now train the new 
layers having as input the feature dataset.

ultralytics is one of the best github repositories for already trained models.
