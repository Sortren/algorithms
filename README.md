﻿# Algorithms
 Most common algorithms, such as binary search, merge sort, quick sort, Dijkstra's algorithm and so on, will be added here on this repository using python.
 If you are intrested, just click the follow button and enjoy ;). 
 
 # Merge sort:
 In brief, this algorithm is quite efficient with O(n log n) complexity (worst case scenario). It's based on recursion, it slices the passed array to smaller arrays
 and it's purpose is to decrease the size of an each array to one. When it will be done, the comparision part will be started. It will compare values from left array 
 with values on right array. Smaller value will be put on the first place at the main array. Due to recursively calling a function, we have to deal with a call stack. 
 When the first "if statement" returns false, the function will go back to the last part of the call stack and continue running, so we have to keep it in mind if we want
 to know how it works properly. That might sound a bit confusing but it will be present better on the diagram.
![first_step](https://user-images.githubusercontent.com/79079000/115121259-f0a05800-9fb1-11eb-9d66-29b80ff094cb.png)
First part was to choose the mid point of an array. It will be always floored length of array divided by two. Next step is to slice the array, everything what's on left side
from mid point goes to "left" array, analogically the same will happen to the right side of the array. When we recursively call this function couple times, we will be
at the point where all arrays are limited to one element, that's what we need! Now we have to travel beetween the elements and compare them to each other. 
So we simply declare variables to represent the indexes of given arrays and start to compare. If the value on the right is lesser than value on the right, it's going to 
be put at the first place in the main array. We increase the values of index variables when the statements retun true, and start to merging all the arrays so on. 
The main goal is to reach the point when we've got one part of the array that is sorted. I hope that it will be understood after this image:
