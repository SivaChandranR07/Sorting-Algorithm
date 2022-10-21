# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.If yes, set the element as the new minimum.
3.  Swap minimum with first unsorted position.
4.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.If yes, move sorted element to the right by 1.
3.	Break the loop and insert X.
4.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
## Selection Sort:

``` python
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Siva Chandran R
RegisterNumber: 22005531
'''
def selectionSort(array, size):
    
    for ind in range(size):
        min_index = ind
 
        for j in range(ind + 1, size):
         
            if array[j] < array[min_index]:
                min_index = j
        
        (array[ind], array[min_index]) = (array[min_index], array[ind])
 
arr = eval(input())
size = len(arr)
selectionSort(arr, size)
print(arr)

```
## Insertion Sort:
```python
'''
Program to sort the elements in the list using the Insertion Sorting Algorithm.
Developed by: Siva Chandran R
RegisterNumber: 22005531
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j >=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
        
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)




```

## Output:
![OUTPUT](out6.png)
![OUTPUT](out8.png)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
