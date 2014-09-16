![image](https://pbs.twimg.com/profile_images/624172340/mah-logo-twitter_normal.png "Malmö Högskola") Malmö Högskola


Artur Olech <br>
M10P2603 <br>
[Kurssida: Advanced Programming](https://www.google.com "Advanced Programming")
# Advanced Programming
### Lecture 4
>Previous lecture was about time complexity and Master Theorem


###Multipliation
* Bit model (bit operation)
  * complexity
* Word complexity
  * O(1) time for arthmetic
  * exponential -> O(4^2) -> O(n^1.54)
  * -> O(nlogn)

## Design Paradigm,
### Divide & Conquer
Classic example, sorting.

###### Merge Sort
```javascript
/* Simple mergesort.
 * Complexity, O(j-i), proportional to #elements
 * A = array
 */
MergeSort (A){
  mSort(A,0,A.lenght-1)
  return A
}
mSort(A,i,j){
  if (j-i > 0){
    k=(i+j)/2
    mSort(A,i,k)
    mSort(A,k+1,j)
    merge(A,i,k,j)
  }
  return A
}
merge(A,i,k,j){
  copy A from i to K to B1
  copy A from b+1 to j to B2
  n = i, l=m=0
  while(n < j+1){
    if(B1[l] <= B2[m]){
      A[n] = B1[l]
      n++
      l++
    } else {
      A[n] = B2[m]
      n++
      m++
    }
  }
}
```
###### Time Complexity
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture4_images/mSort_complexity_0.png "complexity")
![image](https://raw.githubusercontent.com/CommanderAlchemy/Advanced-Programming/master/Lectures/Lecture4_images/mSort_complexity_1.png "Using Master Theorem")
![image](null "Master Theorem vars")
![image](null "Result")

###### Quicksort
```javascript
A = qSort(A,D,A.lenght-1)
return A

qSort(A,i,j){
  if(j-i > 0){
    k= partition(A,i,j)
    qSort(A,i,k-1)us
    qSort(A,k+1,j)
  }
  return A
}
```
