# Python_numpy
## One, the understanding of NumPy

(1) Definition: NumPy is called [Numerical Python]. It is an open source Python data analysis and scientific computing library. NumPy is the basis for our later learning of Pandas (data analysis), SciPy (scientific computing) and Matplotlib (drawing library)

(2) Features of NumPy: ①The bottom layer of NumPy is implemented in C language, which is fast. ②NumPy provides data structures (ie arrays) with higher access efficiency than Python's built-in data structures. ③Supports a large number of high-dimensional arrays and matrix operations ④Provides a large number of mathematical functions Library

(3) Install Anaconda: Anaconda is an open source Python distribution that contains more than 1,500 scientific packages such as conda and Python and their dependencies.

    Software installation website: ①Official website: https://www.anaconda.com ②Tsinghua University open source software mirror station: https://mirrors.tuna.tsinghua.edu.cn
    
    
## Two, one-dimensional array

1. Array characteristics:

(1) Used to store collections of the same type

(2) Each element has an area of the same storage size in memory

2. The data type of the array

(1) The data type of the array-integer

![image](https://github.com/chengkangck/Python_numpy/blob/main/images/integer.png)

(2) The data type of the array-floating point
![image](https://github.com/chengkangck/Python_numpy/blob/main/images/floating%20point.png)

(3) The data type of the array-complex number
![image](https://github.com/chengkangck/Python_numpy/blob/main/images/array%20complex.png)

(4) The data type of the array-string
![image](https://github.com/chengkangck/Python_numpy/blob/main/images/array%20string.png)

(5) The data type of the array-Boolean
![image](https://github.com/chengkangck/Python_numpy/blob/main/images/array%20Boolean.png)

## 3. Function to create one-dimensional array

   Use numpy.array(object) to create a one-dimensional array, where the object type can be a list or an ancestor
   1) numpy.arange(start,stop,step,dtype)
Syntax: start: start value, default is 0, including start value; stop: end value, not including end value; step: step size, default value is 1, the value can be a negative number; dtype: array element type
(2) numpy.linspace(start,stop,num,endpoint,retstep,dtype)
Syntax: num: set the number of generated elements; endpoint: set whether to include the end value, False is not to return, the default value is True; retstep: set whether to return the step size (ie tolerance), False is not to return, the default is False, When the value is True, the return value is a two-tuple, including an array and step size
(3) numpy.logspace(start,stop,num,endpoint,base,dtype) Syntax: start: start value, value is base**start; start: start value, value is base**start; stop: end value, The value is base**stop; base: base

## Third, the function to create a two-dimensional array

   1. numpy.array(object) fill in the nested list or tuple nested tuple in the list in the object

(1) ones() generates an array of all 1s according to the specified shape and data type
numpy.ones(shape,dtype=None)
(2) Generate an array of all 0s
numpy.zeros()   
(3) The full() function generates an array according to the specified shape and data type, and fills it with the specified data
numpy.full(shape,fill_value,dtype=None). fill_value: specify the filled data
(4) The identity() function creates an identity matrix (that is, a matrix whose diagonal elements are 1 and other elements are 0)

numpy.identity(n,dtype=None). n: array shape
