<h1 id="26k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every finite Rademacher sum, independence and the vanishing of odd moments give

$$
\mathbb E|S_n|^4
=\sum_{k=1}^na_k^4+6\sum_{i<j}a_i^2a_j^2
=3\left(\sum_{k=1}^na_k^2\right)^2-2\sum_{k=1}^na_k^4
\leq3\left(\sum_{k=1}^na_k^2\right)^2.
$$

The same calculation applied to $S_n-S_m$ shows that $(S_n)$ is Cauchy in $L^4$, because the tail of $\sum a_k^2$ tends to zero. Its $L^4$ limit agrees almost surely with its $L^2$ limit $S$, since both modes imply convergence in probability. Passing to the limit gives

$$
\lVert S\rVert_4^4\leq3\left(\sum_{k\geq1}a_k^2\right)^2=3\lVert S\rVert_2^4,
$$

and therefore

$$
\boxed{\lVert S\rVert_4\leq3^{1/4}\lVert S\rVert_2}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [26K](../../../26k.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
