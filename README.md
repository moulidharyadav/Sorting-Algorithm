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
Developed by: your nameMOULIDHAR.G
RegisterNumber: 23009285
'''
def selection_sort(nums): # write your code here using selection sort
    for i in range(len(nums)):
        lowest_vaule_index = i
        for j in  range(i+1 , len(nums)):
            if nums[j] < nums[lowest_vaule_index]:
                lowest_vaule_index = j
        nums[i],nums[lowest_vaule_index] =nums[lowest_vaule_index], nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
# use the selection sort function
# print the sorted list
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: your name moulidhar.g
RegisterNumber: 23009285
'''
def insertion_sort(nums):
    # Write your code here to sort the elements in the list using Insertion sort algorithm
    for i  in range(1, len(nums)):
        item_to_insert = nums[i]
        j = i -1
        while j >=0 and nums[j]> item_to_insert:
            nums[j+1] = nums[j]
            j-=1
            nums[j+1] =  item_to_insert
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
# use the insertion sort function to get the sorted list
# print the sorted list
```
## Output:
![image](https://github.com/moulidharyadav/Sorting-Algorithm/assets/147078316/95e8dc34-41ae-4c5e-a687-b42eac93689d)
![image](https://github.com/moulidharyadav/Sorting-Algorithm/assets/147078316/5d83d02e-04dd-46bf-9d30-b6eb1dea4747)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
