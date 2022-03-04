# Python-Basics--Patika-
## 1. Function which flattens a given list.
```
def flatten(a_list):
  if len(a_list)==0:  
    return[]
  if type(a_list[0])==list:  
    return flatten(a_list[0]) + flatten(a_list[1:])
  else:  
    return [a_list[0]] + flatten(a_list[1:])
```
## 2. Function which reverse a given list. If the list contains lists, the function reverses them too.
```
def reverse(r_list):
  if len(r_list)==0:
    return []
  if type(r_list[-1])==list:
    return [r_list[-1][::-1]] + reverse(r_list[:-1])
  else:
    return [r_list[-1]] + reverse(r_list[:-1])
```
