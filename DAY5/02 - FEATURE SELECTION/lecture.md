Feature selection

Can I undestand what are the most important feature that the model uses?

three methods:
	-filter methods: correlation between features and the object I want to
	predict
	-wrapper methods: evaluate multiple subsets of feature trying to 
	select the best one
	-embedded methods: it's a part of the training problem (they depend on
	the model)

Backward selection (wrapper methods) is better because you start with all the 
feature and start to remove one per each step. So you see the effect of 
removing features starting from the full space.
Feature selection depends on the model you are using.
