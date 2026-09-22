<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $A$ is a real [symmetric matrix](../../../../../../symmetric-matrix.md), the [spectral theorem](../../../../../../spectral-theorem.md) gives $\|A\|_2=\rho(A)$. For $\beta\rho<1$, the [Neumann series](../../../../../../neumann-series.md) satisfies

$$
R=(I-\beta A)^{-1}=\sum_{k=0}^\infty(\beta A)^k,
\qquad \|R\|_2\leq\frac1{1-\beta\rho}.
$$

Let $m=\sum_iX_i(0)$ be the initial infected count. Since its entries are [indicator random variables](../../../../../../indicator-random-variable.md), $\|X(0)\|_2=\sqrt m$, while $\|\mathbf1\|_2=\sqrt n$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [operator norm](../../../../../../operator-norm.md) bound yield

$$
\boxed{\mathbb E Z\leq
\frac{\sqrt{nm}}{1-\beta\rho}}.
$$

Thus a sufficient asymptotic condition for a small outbreak is

$$
\boxed{\frac{\sqrt{m/n}}{1-\beta\rho}\longrightarrow0}.
$$

For example, it holds when $m=o(n)$ and $\beta\rho\leq1-\eta$ for a fixed $\eta>0$. For any fixed $\delta>0$, the [Markov inequality](../../../../../../markov-inequality.md) then gives

$$
\mathbb P(Z\geq\delta n)\leq
\frac{\sqrt{m/n}}{\delta(1-\beta\rho)}\longrightarrow0.
$$

This is the [spectral condition for a small discrete SIR outbreak](../../../../../../spectral-condition-for-a-small-discrete-sir-outbreak.md). A uniform gap and few initial infections are needed for this conclusion; the finite-population condition $\beta\rho<1$ alone does not control an asymptotically vanishing gap or an initially macroscopic infected set.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
