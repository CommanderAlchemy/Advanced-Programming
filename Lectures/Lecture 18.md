![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 18
>Computational Geometry

# Triangulation

### Polygon is monotone
if the boundary can be partisioned into two parts each being monotone.
> A chain is a **x-monotone** if it interccts ang vertical line as a connected component.

### 1. Variant
 The stack contains vertices of upper boundary forming left turns.
 or of the lower boundary forming right turns.

 ```javascript
 if new vertex belongs to upper boundary
  if it forms left turn with two top verteces on stack
    push it on stack
  if it forms right turn with two top verteces on stack
    construct triangle
    pop top vertex
    try again.
  if lower boundary
    enter stack and start over.

 ```

 # Planar Straight Line Graph
 pic
 
