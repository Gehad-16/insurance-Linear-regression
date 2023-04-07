# Insurance Linear Regression
## Linear Regression model
1. Steps to think in this way:-
  - First we read the data, then we search the given data , If we find words, we will replace them with possible numbers in the binary system or any system.
  -	After converting the entire data into numbers, we will draw a correlation matrix in order to find the relationship between the features and the desired outcome, if the relationship between them is close to zero, this means that the correlation between them is very weak, so it is possible to drop this feature without any problem.

![image](https://user-images.githubusercontent.com/63863517/230667047-be4bdf22-65ac-488c-b896-2d9a365b52e3.png)

  -	Then we will do rescaling the data until the numbers converge with each other.

  -	Our goal is to reduce the value of error resulting from the cost function by using the gradient decent to create an update for weights until it reaches the optimum value.


  -	After the data preparation stage, we will convert the features into arrays in order to perform the arithmetic operations on them, and we also add a zero array whose 
  number of rows is equal to the same number of features +1 where it is w0.

  -	We will increment a feature column equal to 1 to be used in the gradient Decent calculation.

### We will calculate the cost function this way:-
  ![image](https://user-images.githubusercontent.com/63863517/230667189-4ebc201b-649a-4638-9307-9da49b105d10.png)
  
  
### We will calculate the gradient Decent using this equation:
![image](https://user-images.githubusercontent.com/63863517/230667323-9b9090d8-171a-40a3-8ad1-fc841186245b.png)

### We will stop the duplication when we find that the error rate remains the same without reducing.
![image](https://user-images.githubusercontent.com/63863517/230667392-985cfc6c-1538-4fb2-b2cc-059c12766dc5.png)

- Finally, we will calculate the expected output by multiplying the new weights * test features:-        my_pre=(X_test_matrix * updated_waights.T).

- We will calculate the prediction error percentage, and this ratio is what evaluates our work.

