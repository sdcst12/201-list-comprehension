# 201-list-comprehension

Objectives
* create lists from lists using list comprehension

List comprehension is a shortcut; it is not strictly necessary, but is worth knowing because you will often run into examples that use it to make code more concise.  List comprehension is used to make a list from an existing list.  Consider the following code:

```
oldList = [3,4,5,6,9,10]
newList = []
for i in oldList:
  newList.append(i)
```

This code interates through the old list, and each entry is added to the new list.  With list comprehension, the code can be simplified to the following:
```
oldList = [3,4,5,6,9,10]
newList = [i for i in oldList]
```

List comprehension can also be used to use conditional operators to choose specific values from a list:
```
# finds all even numbers from the oldList
oldList = [3,4,5,6,9,10]
newList = [i for i in oldList if i%2==0]
```


The syntax for list comprehension is:

newlist = [*expression* for *item* in *iterable* if *condition* == True]
 
A great resource for looking at list comprehension includes the w3schools page at https://www.w3schools.com/python/python_lists_comprehension.asp
