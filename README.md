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
Developed by: Aadithya.R
RegisterNumber: 23006361
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lv=i
        for j in range (i+1,len(nums)):
            if nums[j]<nums[lv]:
                lv=j
        nums[i],nums[lv]=nums[lv],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Aadithya.R
RegisterNumber: 23006361
'''
def insertion_sort(num):
    for i in range(len(num)):
        item=num[i]
        j=i-1
        while j>=0 and num[j]>item:
            num[j+1]=num[j]
            j-=1
        num[j+1]=item
num=eval(input())
insertion_sort(num)
print(num)
```

## Output:
![Screenshot 2023-12-28 154905](https://github.com/Aadithya2201/Sorting-Algorithm/assets/145917810/ee7e90c7-1c4e-4eba-a448-1e413f544dcc)

![Screenshot 2023-12-28 154925](https://github.com/Aadithya2201/Sorting-Algorithm/assets/145917810/44ddd260-0da9-4036-bd8c-8fd72561080a)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
