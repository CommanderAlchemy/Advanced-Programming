![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 8
>Previous lecture, dont remember...

# Dijkstra
_does not work if you have negative weight cycles_  
***PriorityQueue Implementations***
* Heap O(logn)
* BST. O(logn)
* Sorted List O(1) + O(n)   (d+i)

O((n+m)logn), using fibonacci Priority Que it is possible to lower it to O(nlogn+m)

```javascript
PriorityQueue(){
  insert
  deleteMin/Max
  build
  isEmpty
  decreaseKey // maintain structure given a change in value for an element.
}
```


```javascript
dijkstra(G,s){
  for each v in G {
    v.visited = false
    v.dist = infinity

    s.visited = true
    s.dist = 0
    s.parent = null

    PQ.insert(s)
    while not PQ.isEmpty(){
      v=PQ.deleteMin()
      for each neighbor u of v {
        if(v.dist+d(v,u) < u.dist){
          u.dist = v.dist+d(v,u)
          if(not u.visited){
            u.visited=true
            PQ.insert(u)
          } else {
            PQ.decreaseKey(u)
          }
          u.paret = v
        }
      }
    }
  }
}

```
