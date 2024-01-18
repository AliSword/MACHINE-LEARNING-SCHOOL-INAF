Principal component analysis

Expressing the original data in a new basis. It is a linear combination of 
the original basis. PCA does not reduce the number of dimension (it's like
rotating the axis).
It a method to have a better representation of your data. How can we decide
if it is a good or bad representation?
The directions along which the data show the largest variance. And correlated
features are redundant (for example weight, height and BMI: BMI is redundant
because is a linear combination of the fisrt two).
You find a basis where data are varyin, where it happen somenthing and discard
the one where nothing happen (redundant).
See covariance matric: diagonal terms variance and off-diagonal correlations.
You have to find a new basis that maximise the variance and minimise the 
covariance. In practise you need to find a basis that diagonalize the 
covariance matrix.
