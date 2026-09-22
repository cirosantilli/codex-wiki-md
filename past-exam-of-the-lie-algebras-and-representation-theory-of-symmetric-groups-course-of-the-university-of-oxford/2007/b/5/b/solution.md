<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [hook length](../../../../../hook-length.md) of a cell is one plus the number of cells to its right in the same row and below it in the same column. The [hook-length formula](../../../../../hook-length-formula.md) is

$$
f^\lambda=\frac{n!}{\prod_{c\in\lambda}h(c)}.
$$

For $\lambda=(n-k,k)$, with $0\le k\le n/2$, the second-row hook product is $k!$. In the first row, the hooks are $n-k-j+2$ for $1\le j\le k$ and $n-k-j+1$ for $k<j\le n-k$, so their product is $(n-k+1)!/(n-2k+1)$. Consequently

$$
f^{(n-k,k)}=\frac{n!(n-2k+1)}{k!(n-k+1)!}
=\boxed{\binom nk-\binom n{k-1}}.
$$

At $k=0$, interpret the second binomial coefficient as zero.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
