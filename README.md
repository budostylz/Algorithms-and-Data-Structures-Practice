[Algorithm Design & Analysis Process | What are the steps to design an algorithm ?](https://www.youtube.com/watch?v=6BWvV4xVh8U&list=PLftH_KTPtiBKPAbFwv0srGgzxVZFm65JX)

[Big-O notation in 5 minutes — The basics](https://www.youtube.com/watch?v=__vX2sjlpXU)

[Proving that 1+2+3+...+n is n(n+1)/2](http://www.maths.surrey.ac.uk/hosted-sites/R.Knott/runsums/triNbProof.html)

[Step Count Method to Measure Time Complexity of an Algorithm - Part 1](https://www.youtube.com/watch?v=53sC2ioHUM0)

[Step Count Method to Measure Time Complexity of an Algorithm - Part 2](https://www.youtube.com/watch?v=lcAq5bID_zs)

[Time Complexity - Operation Count Method](https://www.youtube.com/watch?v=rL1GdFEJ6c4)

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
## Order

We should note that when people refer to the rate of increase of an algorithm, they will sometimes instead use the term order. Or to put that another way:

    The rate of increase of an algorithm is also referred to as the order of the algorithm.

For example, instead of saying "this relationship has a linear rate of increase", we could instead say, "the order of this relationship is linear".


![Computational Complexity](https://github.com/budostylz/Algorithms-and-Data-Structures-Practice/blob/Efficiency/computational_complexity.PNG)

## Big O Notation

```python

function decode(n):
    create output string
    for each letter in n: # O(n + 2)
        get new_letter from letter's location in cipher
        add new_letter to output
    return output



```

![Step Count Method.](https://github.com/budostylz/Algorithms-and-Data-Structures-Practice/blob/Efficiency/Step%20Count%20Method.pdf)

