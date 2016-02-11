#Time Complexity

##Introduction
In computer science, the time complexity of an algorithm quantifies the amount of time taken by an algorithm to run as a function of the length of the string representing the input.

##Big O notation
The time complexity of an algorithm is commonly expressed using big O notation, which excludes coefficients and lower order terms. When expressed this way, the time complexity is said to be described asymptotically, i.e., as the input size goes to infinity.

For example, if the time required by an algorithm on all inputs of size n is at most 5n3 + 3n, the asymptotic time complexity is O(n3). More on that later.

###Examples:

+ 1 = O(n)
+ n = O(n2)
+ log(n) = O(n)
+ 2 n + 1 = O(n)

## O(1) Constant Time:

An algorithm is said to run in constant time if it requires the same amount of time regardless of the input size.

###Examples:

+ array (list): accessing any element
+ fixed-size stack: push and pop methods
+ fixed-size queue: enqueue and dequeue methods

## O(n) Linear Time
An algorithm is said to run in linear time if its time execution is directly proportional to the input size, i.e. time grows linearly as input size increases.

Consider the following example (in C): below I am linearly searching for an element, this has a time complexity of O(n).


```
int find = 66;
var numbers = new int[] { 33, 435, 36, 37, 43, 45, 66, 656, 2232 };
for (int i = 0; i < numbers.Length - 1; i++)
{
    if(find == numbers[i])
    {
        return;
    }
}
```

More Examples:

+ array(list): Linear Search, Traversing, Find minimum etc
+ queue: contains method

## O(log n) Logarithmic Time:
An algorithm is said to run in logarithmic time if its time execution is proportional to the logarithm of the input size.

Example: [Binary Search] (http://en.wikipedia.org/wiki/Binary_search)

Recall the "twenty questions" game - the task is to guess the value of a hidden number in an interval. Each time you make a guess, you are told whether your guess is too high or too low. Twenty questions game implies a strategy that uses your guess number to halve the interval size. This is an example of the general problem-solving method known as binary search
Another analogy: Consider how you search a phone book: You can split the problem in half each time. (eg. Is the first letter of the name greater than or less than M?)

## O(n2) Quadratic Time
An algorithm is said to run in quadratic time if its time execution is proportional to the square of the input size.

###Examples:

1. Bubble Sort
1. Selection Sort
1. Insertion Sort

## Some Useful links
+ [Big-O Misconceptions](http://ssp.impulsetrain.com/big-o.html)
+ [Determining The Complexity Of Algorithm](http://philipstel.wordpress.com/2011/03/07/determining-the-complexity-of-an-algorithm-the-basic-part/)
+ [Big O Cheat Sheet](http://bigocheatsheet.com/)

Taken from [Introduction to Time Complexity of an Algorithm](http://careerbaba.in/2014/01/introduction-to-time-complexity-of-an-algorithm/)

## Other
+ More answers on [Stack Overflow] (http://stackoverflow.com/questions/11032015/how-to-find-time-complexity-of-an-algorithm)
+ Definitions on [Wikipedia] (https://en.wikipedia.org/wiki/Time_complexity)
