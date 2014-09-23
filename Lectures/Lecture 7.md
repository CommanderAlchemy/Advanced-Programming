![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603  
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 7
>Previous lecture, dont remember...

#TODO
* Compile notes.

***bfs-variant***
```javasscript
bfs-variant(G,s){
  for each v in G v.visited = false {
    s.visited = true
    s.dict = 0
    s.parent =null
    q.enQ(jj)
    while not q.isEmpty() {
      v=Q.deQ()
      for each neighbout u of v in g{
        if not u.visited {
          u.visited = true
          u.dist = v.dist+1
          Q.enQ(u)
          u.parent = v
        }
      }
    }

  }
}

```
