# Python Learning
# fibonacci Series
The fibonaci_series.py is written using recursion, this approach is good when you 
generate small number of fibonaci series, but if you generate large execution will
get slow down lets see why?
when you generate series    fibonacci(5) it will caluclate like this
                   fibo(4)       +          fibo(3)
             fibo(3)  +  fibo(2) +  fibo(2) + fibo(1)
    fibo(2) + fibo(1) +   1      +   1      +  1
      1     +  1      +   1      +   1      +  1 = 5

so as you can see to calucalte fibonacci(5) total 8 executions were made which is
going to slow down for larger numbers

fibonaci_memoization.py uses a memoization teqniue which is for faster exection.
#Memoization
Storing the results of functions in a cache, and then returing the stored value
when a function is called with same arguments, here we are using functools modules
which have LRU cache implmented
