<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Baire category theorem](../../../../../../baire-category-theorem.md) states that every countable intersection of open dense subsets of a [complete metric space](../../../../../../complete-metric-space.md) is dense. Equivalently, no nonempty open subset of a complete metric space is a countable union of [nowhere dense sets](../../../../../../nowhere-dense-set.md).

To prove the first form, let $G_1,G_2,\ldots$ be open dense subsets of a complete metric space $X$, and let $V\subseteq X$ be nonempty and open. Choose a closed ball

$$
\overline B(x_1,r_1)\subseteq V\cap G_1,
\qquad 0<r_1<2^{-1}.
$$

Inductively, density and openness of $G_{n+1}$ allow a closed ball

$$
\overline B(x_{n+1},r_{n+1})
\subseteq B(x_n,r_n)\cap G_{n+1},
\qquad 0<r_{n+1}<2^{-(n+1)}.
$$

The balls are nested and $d(x_m,x_n)<2^{-n}$ for $m>n$, so $(x_n)$ is Cauchy. Completeness gives $x_n\to x\in X$. For every $n$, all later centres lie in $\overline B(x_n,r_n)$; closedness gives $x\in\overline B(x_n,r_n)\subseteq G_n$. The first ball also lies in $V$, hence

$$
x\in V\cap\bigcap_{n=1}^\infty G_n.
$$

Since every nonempty open $V$ meets the intersection, that intersection is dense.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
