<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [filtration](../../../../../../filtration-probability-theory.md) $(\mathcal F_n)_{n\geq0}$ on a [probability space](../../../../../../probability-space.md) is an increasing sequence of [sigma-algebras](../../../../../../sigma-algebra.md) contained in $\mathcal F$: $\mathcal F_n\subseteq\mathcal F_{n+1}$. A real [stochastic process](../../../../../../stochastic-process-split.md) $(X_n)$ is a [martingale](../../../../../../martingale-split.md) for this [filtration](../../../../../../filtration-probability-theory.md) if $X_n$ is $\mathcal F_n$-measurable, $\mathbb E|X_n|<\infty$, and

$$
\boxed{\mathbb E[X_{n+1}\mid\mathcal F_n]=X_n\quad\text{almost surely for every }n.}
$$

The first condition is [adaptedness](../../../../../../adapted-process.md); the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) then gives $\mathbb E[X_n\mid\mathcal F_m]=X_m$ whenever $m\leq n$.

The almost-sure [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) states that if a real [martingale](../../../../../../martingale-split.md) satisfies $\sup_n\mathbb E|X_n|<\infty$, then some integrable [random variable](../../../../../../random-variable-split.md) $X_\infty$ satisfies $X_n\to X_\infty$ [almost surely](../../../../../../almost-sure-convergence.md). The more general [almost sure submartingale convergence theorem](../../../../../../almost-sure-submartingale-convergence-theorem.md) needs only $\sup_n\mathbb E[X_n^+]<\infty$ for a [submartingale](../../../../../../submartingale.md). In particular, a nonnegative [martingale](../../../../../../martingale-split.md) converges to a finite integrable limit [almost surely](../../../../../../almost-sure-convergence.md), because its [expected value](../../../../../../expected-value.md) is constant. Mere boundedness in the [L1 norm](../../../../../../l1-norm.md) does not imply [convergence in L1](../../../../../../convergence-in-l1.md). The stronger [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) gives both almost-sure convergence and [convergence in L1](../../../../../../convergence-in-l1.md) when the [martingale](../../../../../../martingale-split.md) is [uniformly integrable](../../../../../../uniform-integrability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
