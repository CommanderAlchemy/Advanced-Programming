![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 18
>Computational Geometry

# Exams (1)

##1
  b = 2* (b-1) / 2 + 1
  b = 2 * b / 2

```javascript
// Even
exp(a,b) {
  if a = 0 return 1
  if b is even
    r = exp(a,b//2)
    return r*r
  else
    r=exp(a, (b-1)/2)
    return r*r*a
}
```
 > Everything takes constant time, the division moves 1 byte on each recursion.
 > Thus is O(m) time.

##2
> Hoffman encoding

| A | C | G | T
|--|--|--|--
|30|14|10|19

> Pick the least used and combine the number, then pick the two least frequency and combine them into a tree.
> Put out numbers on each arch, 0 on left and 1 on right.
> Follow through and now give each letter a binary number.

Calculating we can get to know the ammount me save on using this encoding.

##3

> If j is 0 we get 0 in every case.
> If I is 0 we get 1 in every case.

```javascript
p(n,m){
  A = array(n,m)
  // Fill the first row
  for i = 0 to n
    A[i,0] = 0
  // Fill the first column
  for j = 0 to m
    A[0,j] = 1
  for i = 1 to n
    for j = 1 to m
      A[i,j] = (A[i-1,j] + A[i,j-1]) / 2
}
```
> Because above use n times or m times complexity begins to rise on n * m in the two for loops.

###4

```javascript
Kernel(G){
  for every v in G
    BFS (G,v) -> gives a tree
    traverse tree to find furthest node u
    label v with distance to u
  min = infinte
  for every node u
    if label of u < min
      min = label of u
  for every node u
    if label of u = min
      report u
}
```
> BFS visits every node and traverses edges to O(n+m)
> A graph is at most m € O(n²) and if no loops m<= n*(n-1)/2

###5
> Run 3 runs of the closest pair. First run will give you closest pair.
> Run it again with one of the point that should give you second closest pair.
> Run it a third time with the disregarded point to check if that is not closer.

# Exams (2)
###1
```javascript
peak(A,i,j){
  if i = j return i


  l = (i+j) / 2     // Middle
  if A[l] < A[l+1]  // Find the direction of K
    return peak(A,l+1,j)
  else
    return peak A,i,l)
}

peak(A,0,n-1)
```
> Two times log n so time complexity is O(logn)

###2
```javascript
bipartite(G,u){
  for every node v in G
    v.visited = false
  enQ(u)
  while que is non-empty
    u = deQ()
    u.visited = true
    for every neighbour v of u
      if not v.visited
        enQ(v)

// Modified
bipartite(G,u){
  for every node v in G
    v.visited = false
  enQ(u)
  u.set"x"
  while que is non-empty
    u = deQ()
    u.visited = true
    for every neighbour v of u
      if v.visited
        if v.set= u.set
          report "not bipartite"
      if not v.visited
        if u.set = "x"
          v.set = "y"
        else
          v.set = "x"
        enQ(V)
        report "y is bipartite"
```
##### Bipartite
> Be able to ....
