![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 15
> **Previously**  
>
> Complexity  
> P and NP
> decision problems/languages  
> MST -> LMST  
> SAT € NP  
> Cook Levin 1970  
> Halting Problem

<br>
# Completeness

<br>
### Definition
> Given a complexity class **X**  
> a decision problem **L** is  
> X-complete if any  
> decision problem **L** in **X**  
> can be ***reduced*** to L  
> under the ***resource constraints***  
> defined by **X**

<br>
### Specific Definition
> A decision problem **L** is  
> NP-complete if any  
> decision problem **L** € NP  
> can be ***reduced*** to **L**  
> in polynomial time


# Vertex Cover
![image](url)

> Undirected graph

<br>

> Select smallest subset of nodes s.t.  
> each edge is adjacent to some node.

<br>

> Given graph G and parameter K  
> is there a vertex cover (subset of nodes)  
> of size <= k?
