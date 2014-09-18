![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech  
M10P2603  
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 3
>Previous lecture was about uploading assignments to gov, thus no notes.

### <br>

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
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/axb.png "Divide & Conquer")

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/axb_0.png "a*b=")

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/axb_1.png "cont")

**Calculating the time complexity**  
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/multiplication_complexity_calc.png)


### Even faster method
By using factorisation and calculating all values from parts  
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/multiplication_factorisation.png)

**Calculating the time complexity**  
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/multiplication_complexity__factorisation_calc.png "Malmö Högskola")

### Another method that is even faster
![image](http://www.imgur.com/GdGpkEK.jpeg "Malmö Högskola")

### <br>

# Example problems using "Master Theorem"

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/Master_Theorem.png "Master Theorem")


### <br>


***Example problems***  
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/Example_Problems.png "Example Problems")

***Using the "Masther Theorem" gives***  
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/T1.png "1")

<br>

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/T2.png "2")

<br>

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/T3.png "3")

<br>

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture3_images/T4.png "4")
