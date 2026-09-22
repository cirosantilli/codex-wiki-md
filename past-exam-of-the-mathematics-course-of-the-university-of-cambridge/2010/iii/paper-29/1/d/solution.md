<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

No [quadratic variation](../../../../../../quadratic-variation.md) argument is needed. For deterministic $u<v$, the [martingale](../../../../../../martingale-split.md) property and square integrability give

$$
\mathbb E(X_vX_u)=\mathbb E\bigl[X_u\mathbb E(X_v\mid\mathcal F_u)\bigr]=\mathbb E X_u^2.
$$

Consequently

$$
\mathbb E(X_v-X_u)^2=\mathbb E X_v^2-\mathbb E X_u^2.
$$

Apply this identity separately to each consecutive grid increment. The second moments telescope, giving

$$
\boxed{\mathbb E V_t^{n,|\cdot|^2}=\mathbb E X_{t_n}^2-\mathbb E X_0^2
\le\sup_{s\ge0}\mathbb E X_s^2-\mathbb E X_0^2<\infty.}
$$

This uniform bound follows directly from [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md), including the final interval specified by the ceiling.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
