<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here $F=\mathbf1_A$ is bounded and hence lies in $L^2$ as well as $L^1$. Conditional expectation on a sub-[sigma-algebra](../../../../../../sigma-algebra.md) is the [orthogonal projection](../../../../../../orthogonal-projection.md) in $L^2$ onto its measurable subspace. We can use these projections to justify both limits without any symmetry assumption on the [probability measure](../../../../../../probability-measure.md).

The increasing coordinate sigma-algebras $\mathcal E_n$ generate the whole [product sigma-algebra](../../../../../../product-sigma-algebra.md) $\mathcal F$. Functions depending on finitely many coordinates are dense in $L^2(\mathcal F)$: their cylinder indicators generate $\mathcal F$, and the usual monotone-class approximation proves density of their linear span. If a cylinder function $V$ is $\mathcal E_N$-measurable, then for $n\geq N$ the $L^2$ projection contraction gives

$$
\|F-\mathbb E[F\mid\mathcal E_n]\|_2
\leq\|F-V\|_2+\|\mathbb E[V-F\mid\mathcal E_n]\|_2
\leq2\|F-V\|_2.
$$

Approximate $F$ arbitrarily well by such $V$ to prove the first $L^2$ limit.

For the decreasing tail sigma-algebras $\mathcal G_n$, put $Y_n=\mathbb E[F\mid\mathcal G_n]$. If $m\geq n$, the tower property gives $\mathbb E[Y_n\mid\mathcal G_m]=Y_m$. Projection orthogonality therefore yields

$$
\|Y_n-Y_m\|_2^2=\|Y_n\|_2^2-\|Y_m\|_2^2.
$$

The norms on the right decrease and are nonnegative, so $(Y_n)$ is Cauchy in $L^2$ and has a limit $Y$. Choose an almost-surely convergent subsequence and take its pointwise upper limit. For every fixed $n$ its tail consists of $\mathcal G_n$-measurable functions, so this supplies a version of $Y$ measurable with respect to every $\mathcal G_n$, hence to $\mathcal G=\bigcap_n\mathcal G_n$. For any $C\in\mathcal G$, $\mathbb E[Y_n\mathbf1_C]=\mathbb E[F\mathbf1_C]$; passing to the limit identifies $Y=\mathbb E[F\mid\mathcal G]$.

Finally $\|W\|_1\leq\|W\|_2$ on a [probability space](../../../../../../probability-space.md), by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Thus

$$
\boxed{\mathbb E[F\mid\mathcal E_n]\longrightarrow F,\qquad
\mathbb E[F\mid\mathcal G_n]\longrightarrow\mathbb E[F\mid\mathcal G]\quad\text{in }L^1.}
$$

These are the increasing-filtration and [reverse martingale convergence theorem](../../../../../../reverse-martingale-convergence-theorem.md) limits; the argument above establishes the requested norm convergence directly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
