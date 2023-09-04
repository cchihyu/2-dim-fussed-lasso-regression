# 2-dim-fussed-lasso-regression
This project is an R package that aims to solve both one and two-dimensional fussed lasso problems in a more efficient way.
## Introduction
Fussed lasso regression transfers the original function into a smoother function, and it is widely used in financial, survival, and geographical data analysis. Unlike the traditional loss function like mean square error, fussed lasso regression adds the penalty which is defined as the difference between the point itself and its neighbors. This makes the result function smoother and also close to the original function. Users can directly install the tar.gz file to access the package, the details can be found at the R.Studio official website.

## 1-dimension fussed lasso regression
### create_1D
create_1D is the function that creates the matrix D in the fussed lasso problem. We only need to input the penalty vector and the length of the data in order to get matrix D.

### flp_1D
flp_1D defines the function of solving fused lasso problems in one-dimensional cases using the ADMM method.

## 2-dimension fussed lasso regression
### create_2D
The create_2D function uses the length of data, the penalty vector on the x-axis, and the penalty vector on the y-axis as the input, the output of create_2D is matrix D.

### flp_2D
flp_2D defines the function of solving fused lasso problems in two-dimensional cases using the ADMM method.
