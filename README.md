# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array = eval(input())
# sort the array
k = eval(input()) # k-item to be seared for
n=len(array)
array.sort()
print(array)
result =linearSearch(array,n,k)
# use if-else to print sorted array and "Element not found" if the item is not present in the list otherwise print sorted array and "Element found at index: ", result
if result != -1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")
    



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
def binarysearchIter(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array = eval(input())
array.sort()
k = eval(input()) 
result=binarysearchIter(array,k,0,len(array)-1)
print(array)
if result !=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")







```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
def binarysearchIter(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array = eval(input())
array.sort()
k = eval(input())
result=binarysearchIter(array,k,0,len(array)-1)
print(array)
if result!=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")






```
## Sample Input and Output
i)
![lin in 1](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/cdcffd46-e6d3-4d28-adf0-a945e414898f)

ii)
![lin in 2](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/a6fc8f93-2c09-4be3-9171-e13e47ff8c6c)

iii)
![lin 3 in](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/1529cd00-0cd2-41ea-bc30-75f7fd565902)

## output
i)
![lin out 1](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/b48159bd-41e3-4e44-ae02-09ea292f1866)

ii)
![LIN 2 OUT](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/20c1e341-23e2-44e5-acde-48c49d341e22)


iii)
![lin 3 out](https://github.com/vinodhini-17/Search-Algorithm/assets/145742741/8171da73-ad8f-457e-8062-42a76e7ad15e)





## Result
Thus the linear search and binary search algorithm is implemented using python programming.
