# Quick Sort

# How does one do a ‘quick sort’?

1. Start with an unsorted array (obviously)

```python
[11, 9, 12, 7, 3]
```

1. The **final** value is chosen as the *pivot* element

```python
[11, 9, 12, 7, 3]
```

1. 3 is the smallest element in the array so needs to be swapped with the current value in position 1 (PC 0) 

```python
[3, 9, 12, 7, 11]
```

1. 3 is in the correct position, the values to the right of 3 need to be sorted so the last value 11 is the new pivot element

```python
[3, 9, 12, 7, 11]
```

1. The value 7 needs to be to the left of 11 and 12 has to be to the right
    1. First, move 7 and 12
    
    ```python
    [3, 9, 7, 12, 11]
    ```
    
     b.   Now, swap 11 with 12 so that 9 and 7 are on the left and 12 is on the right
    
    ```python
     [ 3, 9, 7, 11, 12] 
    ```
    
2. 11 and 12 are in the correct positions. 7 should be the pivot element in the sub array [9, 7] to the left of 11
    
    ```python
    [3, 7, 9, 11, 12]
    ```
    
3. Swap 9 with 7
    
    ```python
    [3, 7, 9, 11, 12]
    ```
    

— The array is sorted —

- The last value of the array is chosen as the pivot element, then the rest of the values are arranged so that the values smaller than the pivot are to the left, and higher to the right
- Then the pivot element is swapped w