![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 16
>Halting problem, NP etc.

# Computational Geometry
> How to solve geometric problems using algorithms.  
> Standard algometric model + a few extra primites.

* **Point**  
  Sequence of coordinates (x,y)

*  **Line**  
  Given tree constants A,B,C  
  A ***Line*** is the locus of the equation Ax+By=C

* **Segments**  
  Given two points ***p*** and ***q***  
  a segment is the locus  
  (t * px + (1 - t) qx ), t * py + (1 - t) qy ) ***for*** ```0 <= t <= 1```

* **Half line**  
  Lines when t is 0.....

* **Curve**  
  Cotinues line.

* **Closed**  
  It starts and stops on the same point.

* **Polygon**  
  Closed curve consisting of a seuence of line segments. Simple polygon and polygons with wholes.  
  ***Representation:*** sequence of coordinates of vetices.

* **Vertex**  
  Convex > 180c, Reflex < 180c  
  Always a corner.

* **Vector**  
  Direction (x,y) and magnitude. sqrt(y²+x²)

# Directions
* Left turn positive
* Right turn negative
* use right hand.

  ux * vq - uq * vx  
![image](url "Calculate turn")



# Problem:
Given n points in the plane, find the convex hull of the point set.  
**Convex hull** is the inium perimeter polygon that cointains all the points.

```javascript
// Returns true if its a left turn.
lt(p,q,r)

// Returns true if its a right turn
rt(p,q,r)

CH(p){
  Sort(p) // Onlogn
  SCH(p)  // Onlogn (behaves as merge sort)
}

CSH(P){
  split p into p1 and p2
  CSH(P,1)
  CSH(P,2)
  combine(p)
}
```
Sorting NLOGN B!

### Greedy algorithm
Line sweep algorithm
Plane sweep algorithm
