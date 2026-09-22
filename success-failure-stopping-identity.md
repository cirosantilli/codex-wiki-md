# Success-failure stopping identity

↑ **Parent:** [Negative binomial stopping argument](negative-binomial-stopping-argument.md)

In independent [Bernoulli trials](bernoulli-trial.md) with success [probability](probability.md) $p$ and failure [probability](probability.md) $q=1-p$, let $T_n$ be the trial of success $n$ and $U_m$ the trial of failure $m$, for positive integers $n,m$. If success $n$ occurs after $k<m$ failures, its final trial is a success and the preceding trials have $n-1$ successes and $k$ failures. The [negative binomial stopping argument](negative-binomial-stopping-argument.md) therefore gives the title sum.

Put $F=n+m$. By trial $F-1$, at least one target must have been reached, so the same [event](event.md) is that a [binomial distribution](binomial-distribution.md) with $F-1$ trials has at least $n$ successes. Conditioning instead on the final trial of a block of $F$ trials gives

$$
\sum_{k=0}^{m-1}\binom{n-1+k}{k}p^nq^k
=\binom{F-1}{n}p^nq^{F-n}
+\sum_{k=n+1}^{F}\binom Fk p^kq^{F-k}.
$$

Indeed, more than $n$ successes in the full block guarantee the success target won; with exactly $n$ successes it won only when the final trial was a failure. These disjoint cases explain the extra boundary term. A zero success target wins immediately; a zero failure target has already been reached. To include $n=0$ in the displayed finite sum requires the explicit generalized convention $\binom{-1}{0}=1$; an upper summation limit of $-1$ denotes an [empty sum](empty-sum.md).

## ↑ Ancestors (9)

1. [Negative binomial stopping argument](negative-binomial-stopping-argument.md)
2. [Negative binomial distribution](negative-binomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/12/f/solution.md)
