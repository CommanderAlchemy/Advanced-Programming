![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech
M10P2603
[Kurssida: Advanced Programming](http://edu.mah.se/DA405A "Advanced Programming")
# Advanced Programming
### Lecture 8
> Previously,
> * Greedy algorithms
>   * Krukals alg -> MST
>   * Huffman coding

Greedy algorithms proceed in some linearized sequence
and tries to construct a solution based on knowledge of
current and previous parts of the input.

> When a greedy algorithm may be a good choice.

### e-commerce
Given products and costumers,
what is the smallest set of products that sell to all costumers?

**Set Cover**  
Given a familyn (customers) of sets (products) from some universe of items,
find the smallest subfamily of sets that **cover** all items.

```javascript
GreedyAlg(F,u){
  x= empty set
  F* = empty set
  while x!= u {
    pick largest set
    s from F
    X = X U S
    F* = F* u{s}
    reverse each element in s
    from all the sets in F
  }
  return F*
}
```

Greedy set cover produces a solution F* of size |F*| <= k O(logn)  
where k is the size of the optimal solution.

***Proof***  
Let n***i*** denote the number of unnmoved elements before iteration ***i***. n***0*** = n, n***0*** > n***1*** > n***2*** ... > 0  
#####(It. 1)  
Since k is the size of the optimum, each set contains at most n/k elements.  
We pick biggest |S| >= n/k elements.  
n***1*** = |U| - |S| <= n - n/k = n(1-1/k)  
#####(It. 2)  
Some set in opt must contain at least n***!***/k elements.  
We pick biggest n***1*** <=n***1*** - n***1***/k = n***1***(1-1/k)  
After some math we get n()



# Meanwhile in set theory...
> What is a set?

A set is a group of elements such that each element is either in the set or not  
Rerp. S = {a,b,c,d,e}  
ø empty set _contains nothing_  

| Operation | Desc |
|:--:|--|
|x € s| ***x*** is in _belongs_ ***s***
|S=PuQ| union ***S*** contains element in ***P*** or in ***Q***  
|S=PnQ\| ***S*** contains elements in ***P*** and in ***Q*** (intersect)  
|S=P\Q| ***diff*** elements in ***P*** but not ***Q***  
| `S` | number of elements in ***S***
