<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

On the [Hilbert space](../../../../../../hilbert-space-split.md) $V$, the form $B$ from part b obeys

$$
|B(u,v)|\leq\lVert u\rVert_V\lVert v\rVert_V,
\qquad
B(v,v)=\lVert v\rVert_V^2,
$$

so it is a [bounded bilinear form](../../../../../../bounded-bilinear-form.md) and a [coercive bilinear form](../../../../../../coercive-bilinear-form.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [Poincare inequality with a partial Dirichlet boundary](../../../../../../poincare-inequality-with-a-partial-dirichlet-boundary.md) give

$$
|\ell(v)|
\leq\lVert f\rVert_{L^2(U)}\lVert v\rVert_{L^2(U)}
\leq C_P\lVert f\rVert_{L^2(U)}\lVert v\rVert_V,
$$

so $\ell$ is a bounded [linear functional](../../../../../../linear-functional.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) now gives a unique [weak solution](../../../../../../weak-solution.md) $u\in V$. Taking $v=u$ in the weak identity yields

$$
\lVert u\rVert_V^2
=\ell(u)
\leq C_P\lVert f\rVert_{L^2(U)}\lVert u\rVert_V,
$$

and therefore

$$
\boxed{\lVert u\rVert_V\leq C_P\lVert f\rVert_{L^2(U)}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
