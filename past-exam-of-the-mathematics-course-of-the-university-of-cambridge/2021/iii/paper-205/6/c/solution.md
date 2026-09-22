<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A sufficient set of assumptions is: the columns of the deterministic designs have Euclidean norm at most $\sqrt n$; the true support has size $s$; the [compatibility constant](../../../../../../compatibility-constant.md) on that support is bounded below uniformly; $\log p=o(n)$; and $s\log p/\sqrt n\to0$. Choose $A$ large enough that the Gaussian score event

$$
\left\lVert X^T\varepsilon/n\right\rVert_\infty\leq\lambda/2
$$

has probability tending to one. The standard compatibility oracle inequality then gives

$$
\lVert\widehat\beta-\beta^0\rVert_1
=O_p\left(s\sqrt{\frac{\log p}{n}}\right).
$$

Part b consequently yields

$$
\lVert\Delta\rVert_\infty
=O_p\left(\frac{s\log p}{\sqrt n}\right).
$$

Equivalently, for a sufficiently large constant $c$,

$$
\mathbb P\left(\lVert\Delta\rVert_\infty>\frac{cs\log p}{\sqrt n}\right)\longrightarrow0.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
