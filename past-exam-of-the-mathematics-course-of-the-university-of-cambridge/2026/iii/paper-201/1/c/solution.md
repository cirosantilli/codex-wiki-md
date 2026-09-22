<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $A\in\mathcal F_n$, the defining identity for $X_{n+1}$ gives

$$
\mathbb E[X_{n+1}\mathbf1_A]=\mathbb E[X\mathbf1_A]
=\mathbb E[X_n\mathbf1_A].
$$

Part (b) therefore identifies $X_n$ with $\mathbb E[X_{n+1}\mid\mathcal F_n]$, so $(X_n,\mathcal F_n)$ is a [martingale](../../../../../../martingale-split.md).

The atom formula also proves

$$
|X_n|\leq\mathbb E[|X|\mid\mathcal F_n].
$$

Let $B_{n,K}=\{|X_n|>K\}$. Then $\mathbb P(B_{n,K})\leq\mathbb E|X|/K$ by [Markov inequality](../../../../../../markov-inequality.md), while

$$
\mathbb E[|X_n|\mathbf1_{B_{n,K}}]
\leq\mathbb E[|X|\mathbf1_{B_{n,K}}].
$$

The [uniform absolute continuity for a finite measure](../../../../../../uniform-absolute-continuity-for-a-finite-measure.md) makes the right-hand side uniformly small as $K\to\infty$. Thus $(X_n)$ is [uniformly integrable](../../../../../../uniform-integrability.md). The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) now supplies an integrable random variable $Y$ such that $X_n\to Y$ both [almost surely](../../../../../../almost-sure-convergence.md) and in $L^1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
