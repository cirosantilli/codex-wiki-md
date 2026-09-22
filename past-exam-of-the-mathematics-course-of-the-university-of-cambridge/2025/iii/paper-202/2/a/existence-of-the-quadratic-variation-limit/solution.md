<h1 id="2/a/existence-of-the-quadratic-variation-limit/solution">Solution</h1>

↑ **Parent:** [Existence of the quadratic-variation limit](../existence-of-the-quadratic-variation-limit.md)

By the stated Cauchy property and completeness of $\mathcal M^2$, there is a square-integrable continuous martingale $M$ such that

$$
\sup_{t\geq0}\mathbb E|M_t^{(n)}-M_t|^2\longrightarrow0.
$$

Set $A_t=X_t^2-M_t$. This process is continuous and adapted, and

$$
\mathbb E\sup_{t\geq0}|A_t^{(n)}-A_t|^2
=\mathbb E\sup_{t\geq0}|M_t^{(n)}-M_t|^2
\leq4\sup_{t\geq0}\mathbb E|M_t^{(n)}-M_t|^2\longrightarrow0
$$

by the [Doob L2 maximal inequality](../../../../../../../doob-l2-maximal-inequality.md). The process $A$ is the [quadratic variation](../../../../../../../quadratic-variation.md) $[X]$.

## ↑ Ancestors (12)

1. [Existence of the quadratic-variation limit](../existence-of-the-quadratic-variation-limit.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
