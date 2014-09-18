![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech  
M10P2603  
[Kurssida: Advanced Programming](https://www.google.com "Advanced Programming")
# Advanced Programming
### Lecture 6
>Previous lecture

> Whats the element in ordered pos m in the list

> Randomized selection
* O(n) expected

# Linear time selection
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture6_images/lts_drawing.JPG "Linear Time Search")
```javascript
select(A,m){
  return doSelect(A,0,A.lenght,m)
}
doSelect(A,i,j,m){
  k=partition(A,i,j)
  if k=m return k
  if k>m return doSelect(A,i,k-1,m)
  if k<m return doSelect(A,k+1,j,m)
}
partition(A,i,j){
  s=0
  for (l=i, i <= j, +=5){
    sort(A,l,l+5)         // O(j-i)
    swap(A,l+2,i+s)
    s++
  }
  k = doSelect(A,i,i+(j-i)/5,i+(j-i)/10) // O(n)
  partition as usual around A[k]
}
```
###### Time complexity
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture6_images/lts_0.png "Linear Time Search")

# Graphs
###### A graph G is a tuple (VcE)
* V is a set of nodes / vertices
* E is a set of edges / arcs

###### Useful to represent stuff like:
* Facebook connections
* Bordering countries
* Computer networks
* Mazes
* Transportation networks

###### Types
* Adjucence list
* Adjucence matrix
* Incidence matrix

## Graph Transversal
Organised transversal
* Depth first search

###### Connected Graphs
```javascript
dfs(G,v){
  for each u in G{
    u.visited = false
  }
  explore(G,v)
}
explore(G,v){
  if (v.visited = false){
    v.visited = true
    do stuff on v
    for each neighbour a of v{
      explore(G,v)
    }

  }
}
```
##### Disconnected Graphs
```javascript
dfs(G){
  for each u in G{
    u.visited = false
  }
  for each u in G{
    if not u.visited{
      explore(G,u)
    }
  }
}
```
