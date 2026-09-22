<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

For a partition $a=x_0<\cdots<x_k=b$ and tags $\xi_j\in[x_{j-1},x_j]$, form the [Riemann sum](../../../../../riemann-sum.md) $\sum_{j=1}^k f(\xi_j)(x_j-x_{j-1})$. The [Riemann integral](../../../../../riemann-integral.md) is the unique real number $I$ such that for every $\varepsilon>0$ there is $\delta>0$ for which every tagged partition with mesh $\max_j(x_j-x_{j-1})<\delta$ has its sum within $\varepsilon$ of $I$. Then $I=\int_a^b f(x)\,dx$. The stated continuity ensures existence, which need not be proved here.

The properties required are linearity, the integral of a constant, and [monotonicity of the Riemann integral](../../../../../monotonicity-of-the-riemann-integral.md). Monotonicity follows directly because a nonnegative function has nonnegative [Riemann sums](../../../../../riemann-sum.md), and therefore a nonnegative integral. Integrating $f-m\ge0$ and $M-f\ge0$ gives

$$
\boxed{m(b-a)\le\int_a^b f(x)\,dx\le M(b-a).}
$$

Since $g\ge0$, multiplication preserves the pointwise inequalities: $mg\le fg\le Mg$. The continuous products are integrable, so the same monotonicity and linearity give

$$
\boxed{m\int_a^b g(x)\,dx\le\int_a^b f(x)g(x)\,dx\le M\int_a^b g(x)\,dx.}
$$

Neither $m$ nor $f$ needs to be nonnegative for this argument.

For the first limit, set $r_n=n^{-1/2}$, $g_n(x)=ne^{-nx}$, and $\varepsilon_n=\max_{0\le x\le r_n}|f(x)-f(0)|$. By [continuity](../../../../../continuous-function.md) at zero, $\varepsilon_n\to0$. On this shrinking interval $f(0)-\varepsilon_n\le f(x)\le f(0)+\varepsilon_n$, and

$$
\int_0^{r_n}g_n(x)\,dx=1-e^{-\sqrt n}.
$$

Applying the weighted bounds just proved gives

$$
(f(0)-\varepsilon_n)(1-e^{-\sqrt n})\le\int_0^{r_n}nf(x)e^{-nx}\,dx\le(f(0)+\varepsilon_n)(1-e^{-\sqrt n}).
$$

Both bounding expressions tend to $f(0)$, so the [squeeze theorem](../../../../../squeeze-theorem.md) proves the first limit.

For the full interval, continuity on $[0,1]$ gives a finite bound $B=\max_{[0,1]}|f|$ by the [extreme value theorem](../../../../../extreme-value-theorem.md). The remaining tail has absolute value at most

$$
\left|\int_{r_n}^1nf(x)e^{-nx}\,dx\right|\le B\int_{r_n}^1ne^{-nx}\,dx=B(e^{-\sqrt n}-e^{-n})\longrightarrow0.
$$

Adding this to the already evaluated near-end integral proves

$$
\boxed{\lim_{n\to\infty}\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx=\lim_{n\to\infty}\int_0^1nf(x)e^{-nx}\,dx=f(0).}
$$

These are instances of a [one-sided exponential approximate identity](../../../../../one-sided-exponential-approximate-identity.md): the positive weight has total mass tending to one, concentrated in a shrinking neighborhood of zero. No interchange of limit and integral has been assumed.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
