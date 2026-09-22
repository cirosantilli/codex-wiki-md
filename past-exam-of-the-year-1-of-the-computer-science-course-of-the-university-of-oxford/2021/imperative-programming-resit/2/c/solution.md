<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [array](../../../../../array-data-structure.md) of size $2n+1$, the first probe finds the uniformly selected target with [probability](../../../../../probability.md) $1/(2n+1)$. Otherwise it leaves a half of size $n$; conditional on entering that half, its target is uniform there. Counting the first iteration in every case gives

$$
e_{2n+1}=1+\frac{2n}{2n+1}e_n.
$$

For $n=2^k-1$, the successful-search decision tree has $2^d$ targets at depth $d$, requiring $d+1$ iterations. Thus

$$
e_n=\frac{\sum_{d=0}^{k-1}(d+1)2^d}{2^k-1}.
$$

The numerator is $(k-1)2^k+1$, as follows by [induction](../../../../../mathematical-induction.md) or by shifting and subtracting a finite geometric sum. Substituting $2^k=n+1$ gives

$$
\boxed{e_n=k-1+\frac{k}{n},\qquad a=-1,\quad b=1.}
$$

The base $k=1,n=1$ gives one iteration, as required.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
