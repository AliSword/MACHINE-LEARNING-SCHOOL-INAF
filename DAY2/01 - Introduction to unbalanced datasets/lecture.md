Unbalanced datasets

when the accuracy is similar to the fraction of one class is not good. 
Sensitivity and specificity have to be similar.

How to pre-process data to restore the class balanced?
	-more data (often not possible)
	-undersampling(take few samples from one class of
	data, mostly if you have many of them) and oversampling (clone data 
	samples but doing do the model generalize worse
	because has seen very few cases of such class, or generate new points)
	-use different metrics (you can train models to maximise balanced accuracy
	instead of accuracy, because in this case accuracy doesn't show the problem.

Anyway if the model works (look at hte confusion matrix!), okay don't touch it.
When you do subsampling, make sure that datasets over which you perform it is
a representative case of dtasets (because maybe you can have subpopolations 
within dataset.
Such things (sub/over sampling) are only for training, not tp do analysis.
