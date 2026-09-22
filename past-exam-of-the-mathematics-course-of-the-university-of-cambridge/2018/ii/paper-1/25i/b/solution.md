<h1 id="25i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Rabinowitsch trick](../../../../../../rabinowitsch-trick.md). In the polynomial ring $k[x_1,\ldots,x_n,t]$, consider

$$
I=(J,1-tf).
$$

If $I$ were proper, it would lie in a maximal ideal. Part (a), together with algebraic closedness of $k$, is the [Weak Hilbert Nullstellensatz](../../../../../../weak-hilbert-nullstellensatz.md), so that maximal ideal would be evaluation at a point $(a_1,\ldots,a_n,b)\in k^{n+1}$. We would then have

$$
a=(a_1,\ldots,a_n)\in Z(J),
\qquad 1-bf(a)=0.
$$

But the hypothesis gives $f(a)=0$, a contradiction. Therefore $I$ is the unit ideal.

There are polynomials $g_j$ and $h$ such that

$$
1=\sum_jg_jj+h(1-tf),
\qquad j\in J.
$$

Substitute $t=f^{-1}$ in the localization $k[x_1,\ldots,x_n]_f$. This gives $1\in J_f$; clearing a power of $f$ yields

$$
\boxed{\ f^N\in J\text{ for some }N\geq1.\ }
$$

This is the [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md) inclusion $I(Z(J))\subseteq\sqrt J$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25I](../../25i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
