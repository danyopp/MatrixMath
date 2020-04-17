This is a bash script for calculating basic matrix operations. 
call the script using the following structure

**matrix** *OPERATION* *ARGUMENT* *ARGUMENT2*

**Operations:**
*dims* - will provide the dimensions of the input matrix
*transpose* - refects elements of matrix along main diagonal. MxN -> NxM
*mean* - calculates the matrix mean of each column and returns a matix with result
*add* - adds two matrices, requires two arguments with same dimensions.
*miltiply* - multiplies two matrices, requires two arguments. MxN * NxP = M*P

**Arguments**
Data within rows of the matrix should be delimited by tabs
Rows of the matrix should be delimited by a newline character

The following matrix is in acceptable format:

    8   5   6
    3   2   2

using ^I to repersent tab and $ to represent newline the matrix would read

    8^I5^I6$
    3^I2^I2$

Note this program will test for a valid file input but does not test for matrix format. The behavior is undefined with invalid matrix format
Undefined examples include:
  empty matrix, matrix where final entry has a tab char following, matrix with empty lines, matrix with non-integer data, matrix dimensions larger than 100x100
