
# Welcome to the Hitler Sort Repo :clipboard:

![poster](stalin-sort.jpeg)

## What is Hitler Sort? :question:

### Introduction

Hitler Sort is an efficient sorting algorithm, serving as a systematic method for placing the elements of a random access file or an array in order. Hitler Sort is also know as the best sorting algorithm of all times because of its AMAZING capacity of always ordering an array with an O(n) performance.

### How it works?

It's simple, all you need to do is iterate through the array, checking if its elements are in order. Any element that isn't in order you pull out, in other words, you send it to Gulag.

### Step-by-step example

1. (1 2 5 3 5 7) -> (**1** 2 5 3 5 7) Here the algorithm stores the first of element of the array
2. (**1** 2 5 3 5 7) -> (1 **2** 5 3 5 7) Now it will compare the stored element with the second one, if this is bigger than the stored, it replaces the stored element by this
3. (1 **2** 5 3 5 7) -> (1 2 **5** 3 5 7) Repeats step 2
4. (1 2 **5** 3 5 7) -> (1 2 **5** 5 7) Since the 4th element is smaller than the 3rd one, the 4th element will be eliminated.
5. (1 2 **5** 5 7) -> (1 2 5 **5** 7) Equal elements are preserved
6. **(1 2 5 5 7)** Ordered array!

### Pseudocode implementation

Keep in mind that this is pseudocode, and is just an example. We strongly encourage you to code a different approach. 

```
FUNCTION hitlerSort(A : list OF sortable items)
    n := length(A)
    bigger := 0
    B SET empty list

    FOR i := 0 TO n NOT inclusive DO
        IF A[i] >= bigger THEN
          bigger := A[i]
          B.push(A[i])
        END IF
    END FOR

    RETURN B
END FUNCTION
```

## Want to help? :raised_hands:

Please check the [CONTRIBUTING.md](./CONTRIBUTING.md)

### Give this Project a Star! :star:

## About

> Hitler sort began first as a Hacktoberfest 2018 repo

Hacktoberfest is a program organised by Digital Ocean and Github, where you can easily win a T-Shirt just by making 5 pull requests in the month of October to any open source projects on Github.
