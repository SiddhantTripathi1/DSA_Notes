### Basic Array Operations
Basic array operations involve fundamental tasks such as insertion, deletion, searching, rotation, and merging of arrays. Below are explanations and examples for each operation:

:::info 
1. Insertion in an Array
Concept: Insertion involves adding an element at a specified index in the array. Depending on where the insertion occurs, the elements after the index may need to be shifted to the right.
```python=

# Insert an element at a specified position
def insert_element(arr, pos, element):
    n = len(arr)
    arr = arr[:pos] + [element] + arr[pos:]  # Insert at pos
    return arr

arr = [1, 2, 3, 4, 5]
pos = 2
element = 10
new_arr = insert_element(arr, pos, element)
print(new_arr)  # Output: [1, 2, 10, 3, 4, 5]

```
Insertion Example Question:
Problem: Given an array of integers, every time you receive an integer value, you have to insert it into the array at the correct position to maintain sorted order.
Explanation: This simulates insertion sort, where elements are inserted in their correct position in a sorted part of the array.