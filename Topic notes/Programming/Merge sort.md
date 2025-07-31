# Merge sort

# What is merge sort?

A ‘divide and conquer algorithm’ that breaks down a problem into many subproblems recursively (repetition) until they are simple to solve

*In the case of merge sort, they get divided until the list is separated into individual elements*

Sub problems then get combined to solve the original problems

Has the $O(n * log(n))$ running time, which is the most optimal for comparison based algorithms

## Typical principle

1. Split the array in half
2. Call merge sort on each half to sort them recursively
3. Merge both sorted halves into a single sorted array

*Typically merge sort is left bias, so if the array is odd, the left side will have more values*

## How the list gets ‘merged’ back

Once put into its individual elements, it begins to get put back together

1. Each element is compared to the one next to it to put it back into groups of 2, the one that is the lower value is placed on the left most side, this is repeated until all of the array is in blocks of 2 (plus 1 left over if the list is odd)
2. Then, starting from the left, two of the blocks of 2 numbers are compared to make a block of 4; the **left most values in each block are compared** and the lowest value number is moved into the left most slot of the next block. This then repeats but not including the number that was moved
3. This process repeats until a sorted list is created