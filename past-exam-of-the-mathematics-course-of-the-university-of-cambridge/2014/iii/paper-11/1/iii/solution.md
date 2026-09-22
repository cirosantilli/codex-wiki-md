<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Identify cube vertices with subsets of $[n]$. In a [down-set](../../../../../../down-set.md) $D$, every $A\in D$ has all its $|A|$ immediate lower neighbors in $D$. Counting each internal edge by its upper endpoint gives the [edge boundary of a down-set in a cube](../../../../../../edge-boundary-of-a-down-set-in-a-cube.md)

$$
b_e(D)=nm-2\sum_{A\in D}|A|,\qquad m=|D|.
$$

To maximize it, minimize the sum of set sizes. Among all families of $m$ sets, the minimum is obtained by taking the smallest ranks first. This choice is a down-set: take every set of size below $r$, followed by any required selection of $r$-sets.

Write $M_j=\sum_{i=0}^j\binom ni$, with $M_{-1}=0$, and choose $r$ such that $M_{r-1}\le m\le M_r$. The [largest edge boundary of a down-set](../../../../../../largest-edge-boundary-of-a-down-set.md) is therefore

$$
\boxed{h(m)=nm-2\left[\sum_{j=0}^{r-1}j\binom nj+r(m-M_{r-1})\right]}.
$$

Equivalently, it is $\sum_{j<r}(n-2j)\binom nj+(n-2r)(m-M_{r-1})$. This includes $m=0$ and $m=2^n$, with boundary zero. If $m$ is exactly a complete-level size, either adjacent choice of $r$ gives the same value.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
