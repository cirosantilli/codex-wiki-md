<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) states that if $E$ is a [Banach space](../../../../../../banach-space-split.md) and a family of [bounded linear operators](../../../../../../continuous-linear-operator.md) $S_\alpha:E\to Y$ is pointwise bounded, then $\sup_\alpha\lVert S_\alpha\rVert<\infty$.

Suppose $x_n\rightharpoonup x$ in the [normed vector space](../../../../../../normed-vector-space.md) $X$. For each $n$, define the evaluation functional

$$
J_n:X^*\longrightarrow\mathbb K,
\qquad J_n(f)=f(x_n).
$$

The [completeness of the dual space](../../../../../../completeness-of-the-dual-space.md) says that $X^*$ is Banach even when $X$ is not. For each $f\in X^*$, the scalar sequence $J_n(f)=f(x_n)$ converges to $f(x)$ and is therefore bounded. Uniform boundedness gives

$$
\sup_n\lVert J_n\rVert<\infty.
$$

By the [canonical embedding into the bidual](../../../../../../canonical-embedding-into-the-bidual.md) and the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md), $\lVert J_n\rVert=\lVert x_n\rVert$. Hence

$$
\boxed{\sup_n\lVert x_n\rVert<\infty,}
$$

which proves that a [weakly convergent sequence is bounded](../../../../../../weakly-convergent-sequence-is-bounded.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
