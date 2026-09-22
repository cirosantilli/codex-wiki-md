<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $u\in C^2(\overline D)$, [Itô formula](../../../../../../ito-s-lemma.md) shows that

$$
u(B_{t\wedge T})-u(x)
-\frac12\int_0^{t\wedge T}\Delta u(B_s)\,ds
$$

is a [martingale](../../../../../../martingale-split.md). Take [expectations](../../../../../../expected-value.md) and let $t\to\infty$. The function $u$ is bounded on the [compact set](../../../../../../compact-space.md) $\overline D$, while $\Delta u$ is bounded and $\mathbb E_xT<\infty$ by part (a). The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore gives [Dynkin formula for Brownian motion](../../../../../../dynkin-formula-for-brownian-motion.md)

$$
\boxed{\mathbb E_xu(B_T)
=u(x)+\frac12\mathbb E_x\int_0^T\Delta u(B_s)\,ds.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
