![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech <br>
M10P2603 <br>
[Kurssida: Advanced Programming](https://www.google.com "Advanced Programming")
# Advanced Programming
### Lecture 3
>Previous lecture was about uploading assignments to gov, thus no notes.

#TODO
* Clean up pictures from other clutter
* Upload to github
* Redo links
* Update hoover information on pictures

### Datastructures
* List Arrays
* Binary Search Trees
* Heaps, Priority Ques
* Stacks, Maps
* Has tables

### Graphs
* DFS, (Deph First)
* BFS, (n/a)
* Dijkstra,A*
* MST
* Bellamn Ford

### Sorting Algorythm
* Bubblesort, Quicksort
* Merge sort, Heapsort

## Complexity

### Different model of computation
* Word complexity
* Bit complexity

### Addition
```javascript
/* Complexity, O(n)
 * Becaue most of the operation depends on the ammount of executions.
 */
for i = 1 to n
  s <-- s*i+3
```

> An addition takes max #digits (a), #digits (b) <br>
> That gives O(log(max(a,b)))


### Multiplication
```javascript
/* Complexity 2^n O(n) */
if a=0 or b=0 return 0
p = 0
for i = 1 to a
  p = p + b
return p
```
> O(n) time, n #digits in a

#### Faster method
Using divide and conquer, (split and multiply left parts and right parts sep.).
![image](http://i.imgur.com/JmqPASk.jpeg "Malmö Högskola")

Calculating the time complexity
![image](http://i.imgur.com/5mmJIwU.jpeg "Malmö Högskola")

Result
![image](http://i.imgur.com/P8yszpR.jpeg "Malmö Högskola")


### Even faster method
By using factorisation and calculating all values from parts
![image](http://i.imgur.com/CkNIZ1N.jpeg "Malmö Högskola")

Calculating the time complexity
![image](http://i.imgur.com/1MjrNyc.jpeg "Malmö Högskola")

### Another method that is even faster
![image](http://www.imgur.com/GdGpkEK.jpeg "Malmö Högskola")


### Master Theorem
![image](http://www.imgur.com/lb79znC.jpeg "Malmö Högskola")

Example problems
![image](http://www.imgur.com/TkcnTF0.jpeg "Malmö Högskola")

Using the "Masther Theorem" gives
![image](http://www.imgur.com/ilc0K1R.jpeg "Malmö Högskola")
