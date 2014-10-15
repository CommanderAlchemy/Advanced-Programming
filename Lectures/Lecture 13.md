![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 13
> Previously,
> * Somestuff
>   * stuff
>   * stuff

# Dynamic Programming
* A problem can be reduced into subproblems of smaller size.
* Linearization of computational order in which to solve subproblems.(
* stuff off time for space!

### Algorithms
![image](url)

![image](url)


*** Not efficient***
```javascript
s(node j){
  dist = infinity
  for every node before j {
    i <= j
    if S(i) + S(i,j) < dist
      dist = S(i) + D(i,j)
  }
}
```

### Problem: Given two words
compute minimum edit distance between them.
* insert letter, 1
* delete letter, 1
* exchange letter, 1

![image](url)

### Algorithms
![image](url)


### Paths
![image](url)

### Shortest path between all pairs of nodes

```javascript
warshall(G){
  for i = 1 to n {
    for j = 1 to n {
      if(ui,uj) € G
        D[i,j,0] = d(i,j)
      else
        D[i,j,0] = infinity
    }
  }
  for k=1 to n-2{
    for i = 1 to n {
      for k = 1 to n {
        if(D[i,k,k-1] + D[k,j,k-1] < D[i,j,k-1]) {
          D[i,j,k] = D[i,k,k-1] + D[k,j,k-1]
        } else {
          D[i,j,k] = D[i,j,k-1]
        }
      }
    }
  }
}
```

### Knapsack
Antique shop has items with weight ***wi*** and value ***vi***  
Your knapsack can take ***W*** weight  
Maximize the value you can steal!  
***Knapsack is NP-complete***
