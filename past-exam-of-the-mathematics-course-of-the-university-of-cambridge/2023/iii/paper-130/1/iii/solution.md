<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We prove the [Hilbert cube theorem](../../../../../../hilbert-cube-theorem.md) directly by [mathematical induction](../../../../../../mathematical-induction.md) on its dimension. Dimension zero is immediate. Suppose every finite coloring contains a monochromatic Hilbert $n$-cube, and let $c:\mathbb N\to[k]$ be a $k$-coloring. Refine it to the finite coloring

$$
C(t)=\bigl(c(t),c(t+1),\ldots,c(t+k)\bigr).
$$

By the induction hypothesis, some Hilbert $n$-cube

$$
H=\left\{a+\sum_{i\in I}x_i:I\subseteq[n]\right\}
$$

is monochromatic for $C$. Consequently, for every $j\in\{0,\ldots,k\}$ the translate $H+j$ is monochromatic for $c$; denote its color by $\gamma_j$. By the [pigeonhole principle](../../../../../../pigeonhole-principle.md), two of the $k+1$ colors $\gamma_0,\ldots,\gamma_k$ agree, say $\gamma_s=\gamma_t$ with $s<t$. Then

$$
(H+s)\cup(H+t)
=
\left\{a+s+\sum_{i\in I}x_i+\epsilon(t-s):I\subseteq[n],\ \epsilon\in\{0,1\}\right\}
$$

is a monochromatic Hilbert $(n+1)$-cube. This proves the result without using the [Finite sums theorem](../../../../../../finite-sums-theorem.md) or the [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
