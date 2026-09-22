<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At each finite [stopping time](../../../../../../stopping-time.md) $\sigma_a^k$, the [Strong Markov property](../../../../../../strong-markov-property.md) says that $B_{\sigma_a^k+t}-B_{\sigma_a^k}$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) independent of the past [sigma-algebra](../../../../../../sigma-algebra.md). Its exit time from $(-a,a)$ is exactly $\sigma_a^{k+1}-\sigma_a^k$. By induction the [stopping times](../../../../../../stopping-time.md) are finite almost surely, and these durations are independent with common law $\sigma_a$, not merely identically distributed. This is the [Brownian exit-time skeleton](../../../../../../brownian-exit-time-skeleton.md).

Put $v=\operatorname{Var}(\sigma_1)<\infty$, which follows from the moment estimate. [Brownian scaling](../../../../../../brownian-scaling.md) gives $\operatorname{Var}(\sigma_a)=a^4v$. For

$$
\tau_n=\sigma_{2^{-n}}^{2^{2n}},
$$

there are $2^{2n}$ independent durations of mean $C2^{-2n}$ and [variance](../../../../../../variance-split.md) $v2^{-4n}$. Consequently

$$
\mathbb E\tau_n=C,\qquad\operatorname{Var}(\tau_n)=v2^{-2n}.
$$

For each $\varepsilon>0$, [Chebyshev's inequality](../../../../../../chebyshev-inequality.md) gives

$$
\sum_{n\geq0}\mathbb P(|\tau_n-C|>\varepsilon)
\leq\frac v{\varepsilon^2}\sum_{n\geq0}2^{-2n}<\infty.
$$

Apply the [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md) for a countable sequence of positive errors tending to zero. We obtain the [Brownian exit-skeleton clock convergence](../../../../../../brownian-exit-skeleton-clock-convergence.md):

$$
\boxed{\sigma_{2^{-n}}^{2^{2n}}\longrightarrow C\quad\text{almost surely}.}
$$

No [independence](../../../../../../independent-random-variables.md) between the clocks for different values of $n$ is required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
