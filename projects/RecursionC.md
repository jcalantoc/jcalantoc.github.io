---
layout: project
type: project
image: img/Recurse3.jpg
title: "Recursion Project for ICS 212"
date: 2022
published: true
labels:
  - C
  - Recursion
summary: "A project on Recursion done for ICS 212"
---


I was given an assignment to create recursive functions that performed basic math operations to better get the hang of recursion and how to implement it in C.  Before the assignment, recursion was a concept I had learned in the past but did not particularly like because of how I struggled to grasp the idea of it.After this assignment, which included multiple recursive functions to perform operations on numbers in between the range of two parameters, I grew to really enjoy recursion and the idea of it much more.  

...
/* Use recursion to add the sum of the integers
 * (i.e. the summation (upperc\ase Sigma))
 * from the first integer to the second integer and return it.  
 * @param startAdd the first integer inputed to start adding.
 * @param endAdd the second integer inputed and the last to add.
 * @return resultA the result of adding all the numbers.
 */
int recursiveAdd(int startAdd, int endAdd){
  
    int resultA = 0;
    /*
 Default Case
    */
    if (startAdd == endAdd) {
        resultA = endAdd;
    } else {
      /*
Add each number to with each next one until the second value inputed
      */
        resultA = startAdd + recursiveAdd(startAdd + 1, endAdd);
    }
        return resultA;
  
    
}

...

One of the functions included this function shown above which calculates the sum of a given range of numbers, and the function recursively starts from the first given number until it reaches the ending number resulting in the base case and end of the function's calculation.  A simple but powerful concept like recursion used to be one of the hardest things for me to grasp while learning it in Java, but going back over it in C grew my appreciation for it, and I enjoy thinking about problems recursively as opposed to always thinking of using loops.

Since then I have looked a lot more into the applications of recursion vs iteration, as well as the different reasons why it is powerful and important to understand. If a function is able to be implemented recursively, I ponder the different tradeoffs of recursion for the specific function.  Recursion is a concept that embodies the needed programmer perspective of divide and conquer, and the idea of splitting up a collective problem into smaller, more manageable problems is necessary to succeed not only in this tech field, but in every challenging aspect of life.
