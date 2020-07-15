[Algorithm Design & Analysis Process | What are the steps to design an algorithm ?](https://www.youtube.com/watch?v=6BWvV4xVh8U&list=PLftH_KTPtiBKPAbFwv0srGgzxVZFm65JX)

# Efficiency

## Quantifying Efficiency



```python

# Which Function is More Efficent
# Line Count = 5
def some_function(n): # Line1
    for i in range(2): # Line2
        n += 100 # Line3 + Line4
    return n # Line5

#Line Count = 104
def other_function(n): # Line1
    for i in range(100): # Line2
        n += 2 #Lines = 100 
    return n #Line4

# some_function is more efficent.

```

## Input Size and Efficency

```python

# As the input to an algorithm increases, the time required to run the algorithm may also increase.

def say_hello(n):
    for i in range(n):
        print("Hello!")


say_hello(3) #This input will add 3 lines of code to run.

say_hello(1000) #This input will add 1000 lines of code to run.


def say_hello(n):
    for i in range(n): #n^1
        for i in range(n): #n^2
            print("Hello!") # n=2, 2^2 = 4, This line will run 4 times.

# As the input to an algorithm increases, the time required to run the algorithm may also increase—and different algorithms may increase at different rates.



```


![Computational Complexity](https://github.com/budostylz/Algorithms-and-Data-Structures-Practice/blob/Efficiency/computational_complexity.PNG)

