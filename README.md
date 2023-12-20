# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by:Ezhil sree J
RegisterNumber:23012968
'''
def selection_sort(nums):
    for i in range(0,len(nums)):
        min_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[min_index]:
                min_index=j
        nums[i],nums[min_index]=nums[min_index],nums[i]
    print(nums)
list_of_nums = eval(input())
selection_sort(list(list_of_nums))
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Ezhil sree J 
RegisterNumber:23012968
'''
def insertion_sort(nums):
    n=len(nums)
    for i in range(1,n):
        key=nums[i]
        j=i-1
        while j>=0 and key<nums[j]:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=key
    print(nums)
list_of_nums = eval(input())
insertion_sort(list_of_nums)
```

## Output:
![image](https://github.com/EzhilsreeJ/Sorting-Algorithm/assets/144870412/cdaa005a-fa94-40ff-8eea-2273f6daa2fe)
![image](https://github.com/EzhilsreeJ/Sorting-Algorithm/assets/144870412/fcd8f0f4-f02f-4f76-9836-4c1986df2f18)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
