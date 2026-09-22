<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write each [polynomial](../../../../../../polynomial-split.md) of [degree](../../../../../../degree-of-a-polynomial.md) at most $n$ as $T\mathbf a$ and define

$$
F(\mathbf a)=\lVert T\mathbf a-f\rVert_\infty.
$$

This is a [continuous function](../../../../../../continuous-function.md), and the reverse [triangle inequality](../../../../../../triangle-inequality.md) together with part (a) gives

$$
F(\mathbf a)\geq \lVert T\mathbf a\rVert_\infty-\lVert f\rVert_\infty
\geq\delta\lVert\mathbf a\rVert_2-\lVert f\rVert_\infty.
$$

Consequently $F$ is a [coercive function](../../../../../../coercive-function.md). Choose $R$ so large that $F(\mathbf a)>F(\mathbf0)$ outside the closed [Euclidean ball](../../../../../../euclidean-ball.md) of radius $R$. That ball is [compact](../../../../../../compact-space.md), so the [extreme value theorem](../../../../../../extreme-value-theorem.md) supplies a minimizer $\mathbf a_*$ there. Then $P=T\mathbf a_*$ is a [best uniform approximation](../../../../../../best-uniform-approximation.md) to $f$ among polynomials of degree at most $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
