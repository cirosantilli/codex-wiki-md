<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A suitable [precondition](../../../../../precondition.md), including the empty [array](../../../../../array-data-structure.md) case, is

$$
\boxed{bs(i)\geq1\ (0\leq i<N),\qquad 0\leq n<\prod_{i=0}^{N-1}bs(i).}
$$

A base of one is allowed: its only valid digit is zero. The empty [product](../../../../../product-of-numbers.md) is one, so $N=0$ permits exactly $n=0$. Each [Euclidean division](../../../../../euclidean-division.md) extracts the next least significant digit.
```
def intToDigs(n: Int, bs: Array[Int]): Array[Int] = {
  // Pre: every base is positive, and 0 <= n < product(bs).
  val N = bs.length
  val xs = new Array[Int](N)
  var i = 0
  var q = n
  while (i < N) {
    xs(i) = q % bs(i)
    q = q / bs(i)
    i += 1
  }
  xs
}
```
The expensive [precondition](../../../../../precondition.md) is a caller obligation, rather than a separately computed [product](../../../../../product-of-numbers.md) inside the conversion. Define $P_i=\prod_{j=0}^{i-1}bs(j)$. The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq i\leq N,\qquad
n=\sum_{k=0}^{i-1}xs(k)P_k+qP_i,\qquad
0\leq q<\prod_{j=i}^{N-1}bs(j),
$$

together with $0\leq xs(k)<bs(k)$ for each processed digit. The [Euclidean division](../../../../../euclidean-division.md) identity $q=(q\bmod bs(i))+bs(i)\lfloor q/bs(i)\rfloor$ proves preservation of the reconstruction equality. Positivity of the bases gives the digit bounds and the next bound on the quotient. The [loop variant](../../../../../loop-variant.md) is $N-i$. At exit, $0\leq q<1$ forces $q=0$, hence

$$
\boxed{xs\otimes bs=n,\qquad 0\leq xs(i)<bs(i).}
$$

There are exactly $N$ remainder operations and $N$ divisions, hence $2N$ counted operations. The returned [array](../../../../../array-data-structure.md) occupies $O(N)$ space and the remaining [auxiliary space](../../../../../auxiliary-space.md) is constant. A represented value can never exceed $\prod_i bs(i)-1$, as follows either by the same nested expansion or by telescoping $\sum_i(bs(i)-1)P_i=P_N-1$; thus the stated range is also necessary for positive bases.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
