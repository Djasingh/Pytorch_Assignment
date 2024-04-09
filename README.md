## Problem:
The data is supplied in the attached .pkl file, and comprises a 50x50 grid of digital terrain
elevation heights. A value of -100 indicates a missing value. Your first task will be to read the
data into Python and to extract some basic information describing the data. You can plot the
data if you feel it adds to your understanding.
You should then assign data points to training or test sets as you see fit, and give your
reasons for making your assignment in the way you selected.

Next you should fit a linear model to your training data using a linear least squares approach
(hint torch.linalg.lstsq might be useful, although the same solution can be computed in
multiple ways).

To extend this model you can select a number of data points as the centres for a set of basis
functions. Each basis function should return the exponential of minus the squared distance to
the basis function centre. Each 2D input data point can be replaced with the values of the
basis functions. Start with 10 basis functions which will transform the 2D data into 10D data.
Fit another linear model to the new data and measure how well it models the test data.
Comment on how it compares to the purely linear model.
