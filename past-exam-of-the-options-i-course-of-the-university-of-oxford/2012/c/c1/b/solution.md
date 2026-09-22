<h1 id="c/c1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $R_n=\{k\in\mathbb Z:0<k<n,\ \gcd(k,n)=1\}$. The map $k\mapsto n-k$ sends $R_n$ to itself because

$$
\gcd(n,n-k)=\gcd(n,k)=1.
$$

Applying it twice returns $k$, so it is a bijection. Reindexing the finite sum by this bijection gives

$$
\boxed{\sum_{k\in R_n}k=\sum_{k\in R_n}(n-k).}
$$

There is no need to assume that every residue belongs to a pair of distinct elements; the reindexing also handles the fixed point when $n=2$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [C1](../../c1.md)
3. [C](../../../c.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
