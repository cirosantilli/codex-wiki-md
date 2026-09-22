<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose the claimed [Poincare inequality with a partial Dirichlet boundary](../../../../../../poincare-inequality-with-a-partial-dirichlet-boundary.md) fails. There are $v_k\in V$ with

$$
\lVert v_k\rVert_{L^2(U)}>k\lVert\nabla v_k\rVert_{L^2(U)}.
$$

After the normalization $w_k=v_k/\lVert v_k\rVert_{L^2(U)}$,

$$
\lVert w_k\rVert_{L^2(U)}=1,
\qquad
\lVert\nabla w_k\rVert_{L^2(U)}<\frac1k.
$$

Thus $(w_k)$ is bounded in the [Sobolev space](../../../../../../sobolev-space-split.md) $H^1(U)$. The [Rellich-Kondrashov compactness theorem](../../../../../../rellich-kondrashov-compactness-theorem-for-h01.md) and the corresponding compact embedding for a bounded $C^1$ domain give a subsequence that converges strongly in $L^2(U)$ and weakly in $H^1(U)$ to some $w$. The [Sobolev space with a partial Dirichlet condition](../../../../../../sobolev-space-with-a-partial-dirichlet-condition.md) $V$ is a [closed vector subspace](../../../../../../closed-vector-subspace.md), hence weakly closed, so $w\in V$. Moreover $\nabla w=0$, and connectedness of $U$ makes $w$ a [constant function](../../../../../../constant-function.md). Its [trace](../../../../../../sobolev-trace-theorem.md) vanishes on the positive-measure set $\Gamma_1$, so that constant is zero. This contradicts

$$
\lVert w\rVert_{L^2(U)}
=\lim_k\lVert w_k\rVert_{L^2(U)}=1.
$$

Therefore some $C_P$ satisfies

$$
\lVert v\rVert_{L^2(U)}\leq C_P\lVert\nabla v\rVert_{L^2(U)}.
$$

Since the reverse bound $\lVert\nabla v\rVert_2\leq\lVert v\rVert_{H^1}$ is immediate,

$$
\lVert\nabla v\rVert_2
\leq\lVert v\rVert_{H^1}
\leq\sqrt{1+C_P^2}\,\lVert\nabla v\rVert_2.
$$

The gradient seminorm is a norm on $V$ because equality to zero would make $v$ a constant whose trace on $\Gamma_1$ is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
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
