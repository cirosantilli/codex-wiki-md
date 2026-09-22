# Bernoulli polarization martingale

↑ **Parent:** [Martingale](martingale-split.md)

Let $0<\alpha<1$, $X_0=x\in[0,1]$, and let $B_{n+1}$ be a binary [random variable](random-variable-split.md) satisfying $\mathbb E[B_{n+1}\mid\mathcal F_n]=X_n$. Suppose $X_n$ is $\mathcal F_n$-[measurable](measurability.md) and $B_{n+1}$ is $\mathcal F_{n+1}$-[measurable](measurability.md). The update

$$
X_{n+1}=(1-\alpha)X_n+\alpha B_{n+1}
$$

remains in $[0,1]$ and defines a bounded [martingale](martingale-split.md). For example, take [independent](independent-random-variables.md) [uniform random variables](uniform-random-variable.md) $U_{n+1}$ independent of the current [filtration](filtration-probability-theory.md) and set $B_{n+1}=\mathbf1_{\{U_{n+1}\leq X_n\}}$.

The binary identity $B_{n+1}^2=B_{n+1}$ gives

$$
\mathbb E[(X_{n+1}-X_n)^2\mid\mathcal F_n]
=\alpha^2X_n(1-X_n),
$$

and hence

$$
\mathbb E[X_{n+1}(1-X_{n+1})\mid\mathcal F_n]
=(1-\alpha^2)X_n(1-X_n).
$$

The [L2-bounded martingale convergence theorem](l2-bounded-martingale-convergence-theorem.md) gives a terminal [random variable](random-variable-split.md) $X_\infty$ with [almost sure convergence](almost-sure-convergence.md) and [convergence in L2](convergence-in-l2.md). Iteration followed by the [bounded convergence theorem](bounded-convergence-theorem.md) yields

$$
\mathbb E[X_\infty(1-X_\infty)]
=\lim_n x(1-x)(1-\alpha^2)^n=0.
$$

Thus $X_\infty$ takes only $0$ and $1$, and preservation of its [expected value](expected-value-split.md) gives a [Bernoulli distribution](bernoulli-distribution.md) with parameter $x$. The terminal [conditional expectation](conditional-expectation.md) representation gives the exact [mean squared error](mean-squared-error.md)

$$
\mathbb E[(X_\infty-X_n)^2]=x(1-x)(1-\alpha^2)^n.
$$

The finite-time paths can stay strictly inside $(0,1)$ while their limit lies entirely at the endpoints. The positive conditional [variance](variance-split.md) in the interior makes permanent convergence to an interior value impossible.

## ↑ Ancestors (6)

1. [Martingale](martingale-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2009/a/2/b/i/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2009/a/2/b/ii/solution.md)
- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/1/b/iv/solution.md)
