![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech <br>
M10P2603 <br>
[Kurssida: Advanced Programming](https://www.google.com "Advanced Programming")
# Advanced Programming
### Lecture 5
>Previous lecture

>Mergesort -> O(nlogn)
* Drawback, needs extra memory.

> Quicksort -> O(n^2) worst case
* Randomization of pivot O(nlogn)
* Partially fast

# Three useful sums
###### Arithmetic sum
![image](null "Arithmetic sum")
###### Geometric sum
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture5_images/geometric_sum.png "Geometic sum")

###### Harmonic sum
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture5_images/Harmonic_sum.png "Harmonic sum")

![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture5_images/Harmonic_sum_0.png "gamma")
# Order Selection
What is the kth element in order in the list?

What is the middle element?

```javascript
// O(nlogn)
SimpleAlgorithm(A){
  Sort              // O(nlogn)
  Lookup middle pos // o(1)
}
```

```javascript
// Randomized Selection
// O(j-i) like quicksort.
median(A,i,j,m)
  k = partition (A,i,j)       // O(1)
  if (k=m){                   // O(1)
    return A[k]
  } else if (k<m){            // T(j-k-1)
    return median (A,k+1,j,m)
  } else if (k>m){            // T(j-k-1)
    return median (A,i,k-1,m)
  }
}
```

```javascript
// Randomized Selection
// O(j-i) like quicksort.
median(A,i,j,m)
  k = partition (A,i,j)       // O(1)
  if (k=m){                   // O(1)
    return A[k]
  } else if (k<m){            // T(j-k-1)
    return median (A,k+1,j,m)
  } else if (k>m){            // T(j-k-1)
    return median (A,i,k-1,m)
  }
}
```
