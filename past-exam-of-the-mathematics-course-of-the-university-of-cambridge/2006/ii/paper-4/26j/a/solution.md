<h1 id="26j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an interval of length $t$, the joint [probability generating function](../../../../../../probability-generating-function.md) of the marked counts is

$$
\mathbb E[s^{M^{(1)}}r^{M^{(2)}}]
=\exp\{\lambda t[ps+(1-p)r-1]\}
=\exp\{\lambda pt(s-1)\}\exp\{\lambda(1-p)t(r-1)\}.
$$

This factors into two Poisson generating functions. Independent parent increments on disjoint intervals and independent marks give independent increment vectors, so the factorization holds jointly over all intervals. Thus **the two processes are independent Poisson processes of rates $\lambda p$ and $\lambda(1-p)$**. For $m$ types the same calculation gives $\prod_j\exp[\lambda p_jt(s_j-1)]$, proving independent Poisson processes of rates $\lambda p_j$. A zero probability gives an identically zero process.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
