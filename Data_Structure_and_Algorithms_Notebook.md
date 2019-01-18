## Data Structure and Algorithms Notebook

Shiyu 

shiyumou@usc.edu

### Hashmap

- Use Python dictionary as a Hashmap. Store index and value together. If we are looking for index, we can store 'value' as key in the dictionary. Then dict[value] would be the index.

### Array

- **Traverse** − print all the array elements one by one.
- **Insertion** − Adds an element at the given index.
- **Deletion** − Deletes an element at the given index.
- **Search** − Searches an element using the given index or by the value.
- **Update** − Updates an element at the given index.

```python
from array import *
array1 = array('i', [10,20,30,40]) # only int, string is 'c'
array1.insert(1, 60)
array1.remove(20)
array1.index(60)
```

```python
import numpy as np
array2 = np.array([10, 20, 50, 'da'])
np.insert(array2, 1, 'sad')
np.delete(array2, 1) # fill index
index = np.where(array2=='da') # this will give you (array([3]),) use [0][0] to get 3
# or simply
list(array2).index('da')
```

### List

- Delete element. 

- ```python
  # delete
  del list1[2]
  # concatenate
  [1,2,3]+[4,5,6] = [1,2,3,4,5,6]
  # repeat
  ['Hi']*4 = ['Hi!', 'Hi!', 'Hi!', 'Hi!']
  # membership
  3 in [1,2,3]? True
  # insert 
  T = [[11, 12, 5, 2], [15, 6,10], [10, 8, 12, 5], [12,15,8,6]]
  T.insert(2, [0,5,11,13,6])
  ```


### Dictionary

```python
dict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}
del dict['Name']; # remove entry with key 'Name'
dict.clear();     # remove all entries in dict
del dict ;        # delete entire dictionary
```

###Numpy array

```python
from numpy import * 
m = array([['Mon',18,20,22,17],['Tue',11,18,21,18],
		   ['Wed',15,21,20,19],['Thu',11,20,22,21],
		   ['Fri',18,17,23,22],['Sat',12,22,20,18],
		   ['Sun',13,15,19,16]])
# append a row to numpy array
m_r = append(m,[['Avg',12,15,13,11]],0) # remember to add the axis
```

### Set

```python
Days=set(["Mon","Tue","Wed","Thu","Fri","Sat"])
Days.add("Sun")
Days.discard("Sun")

DaysA = set(["Mon","Tue","Wed"])
DaysB = set(["Wed","Thu","Fri","Sat","Sun"])
# union operation on two sets
AllDays = DaysA|DaysB
# Intersection of Sets
AllDays = DaysA & DaysB
# Difference of Sets
AllDays = DaysA - DaysB # produces a new set containing only the elements from the first set and none from the second set

# Compare Sets, check if a given set is a subset or superset of another set. 
DaysA = set(["Mon","Tue","Wed"])
DaysB = set(["Mon","Tue","Wed","Thu","Fri","Sat","Sun"])
SubsetRes = DaysA <= DaysB
SupersetRes = DaysB >= DaysA
True
True
```



### 