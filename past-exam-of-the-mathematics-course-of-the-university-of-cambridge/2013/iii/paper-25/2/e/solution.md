<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set $Z_t=\mathbb E[\phi'(W_T)\mid\mathcal F_t]$. The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) applied to the bounded terminal variable $\phi'(W_T)$ supplies a continuous adapted version of $Z$, so it is [predictable](../../../../../../predictable-process.md). Hence

$$
\gamma_t=Z_t\mathbf1_{\{t\le T\}}
$$

is predictable and satisfies $\mathbb E\int\gamma_t^2dt\le T\|\phi'\|_\infty^2$. For every square-integrable [predictable process](../../../../../../predictable-process.md) $\alpha$, conditioning at each deterministic time and using [Fubini theorem](../../../../../../fubini-s-theorem.md) gives

$$
\mathbb E\int_0^T\phi'(W_T)\alpha_t\,dt=\mathbb E\int_0^T Z_t\alpha_t\,dt.
$$

Thus part (d) says $\mathbb E\int(\beta_t-\gamma_t)\alpha_tdt=0$. Taking $\alpha=\beta-\gamma$, which is an allowed predictable square-integrable process, makes its squared norm zero. We conclude

$$
\boxed{\beta_t=\mathbb E[\phi'(W_T)\mid\mathcal F_t]\mathbf1_{\{t\le T\}}\quad d\mathbb P\,dt\text{-almost everywhere}.}
$$

This is the [Clark-Ocone formula for a smooth Brownian terminal payoff](../../../../../../clark-ocone-formula-for-a-smooth-brownian-terminal-payoff.md), with exactly the uniqueness established in part (c).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
