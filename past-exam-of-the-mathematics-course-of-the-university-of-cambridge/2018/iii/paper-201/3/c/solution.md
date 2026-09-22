<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [sigma-algebras](../../../../../../sigma-algebra.md) $\mathcal G_n=\sigma(S_n,S_{n+1},\ldots)$ decrease with $n$, and (b) gives $S_n/n=\mathbb E[X_1\mid\mathcal G_n]$. The permitted [reverse martingale convergence theorem](../../../../../../reverse-martingale-convergence-theorem.md) therefore gives an [integrable random variable](../../../../../../integrable-random-variable.md) $L$ such that $S_n/n\to L$ [almost surely](../../../../../../almost-sure-convergence.md) and with [convergence in L1](../../../../../../convergence-in-l1.md). In particular,

$$
\mathbb EL=\lim_n\mathbb E[S_n/n]=m.
$$

It remains to prove that $L$ is constant. We must not assume that $\bigcap_n\mathcal G_n$ is the [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) of the $X_j$; instead use [tail measurability of limits of sample averages](../../../../../../tail-measurability-of-limits-of-sample-averages.md) directly. Define the [random variable](../../../../../../random-variable-split.md) valued in the [extended real numbers](../../../../../../extended-real-number-line.md) $L^*=\limsup_n S_n/n$. For every fixed $N$,

$$
L^*=\limsup_{n\to\infty}\frac{X_{N+1}+\cdots+X_n}{n},
$$

because $S_N/n\to0$ pointwise. Thus $L^*$ is measurable with respect to $\sigma(X_{N+1},X_{N+2},\ldots)$ for every $N$, and hence to the [tail sigma-algebra](../../../../../../tail-sigma-algebra.md). Also $L^*=L$ [almost surely](../../../../../../almost-sure-convergence.md).

By the [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md), each [tail event](../../../../../../tail-event.md) $\{L^*\leq q\}$, for a [rational number](../../../../../../rational-number.md) $q$, has probability zero or one. Since $L^*$ is finite [almost surely](../../../../../../almost-sure-convergence.md), its [distribution function](../../../../../../cumulative-distribution-function.md) can only be that of a constant $c$: taking $c=\inf\{q\in\mathbb Q:\mathbb P(L^*\leq q)=1\}$ and using the [density of the rational numbers](../../../../../../density-of-the-rational-numbers.md) gives $L^*=c$ [almost surely](../../../../../../almost-sure-convergence.md). Its [expected value](../../../../../../expected-value.md) identifies $c=m$. This proves the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md):

$$
\boxed{\frac{S_n}{n}\longrightarrow m\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
