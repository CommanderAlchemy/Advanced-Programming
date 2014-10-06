![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 12
> Previously,
> * Greedy algorithms
>   * Krukals alg -> MST
>   * Huffman coding

# Dynamic Programming
* Richard Bellman

#### Shortest path problem
* Dijkstra
  * No negative weights
  * No negative cycles
  * Path is unique _ie_ tree thus not interesting.
* Bellman Ford

### Directed Graphs
* Strong connectivity
  * V and A are strongly connected
  if path from A to V **and**  
  path from V to U.

Any directed graph can be split into strongly connected components.

### Directed acyclic graph
![image](url)

Always contains a **source** and a **sink**

### Linearization
When converting normal fraph to a linear one.

![image](url)
```javascript
for each v in G{
  v.dist = infinity
  v.prev = null
}

for each v in G{
  // (in linearized order)
  for each node u having
  arc (a,v)
  if (a.dist + d(u,v) < v.dist){
    v.dist = a.dist + d(u,v)
  }
}
```

### Longest increasing subsequence (LIS)
![image](url)

### Longest common subsequence (LCS)
![image](url)

```javascript
G(V,A){
  V = nodes
  A = arcs // directed
}
```
