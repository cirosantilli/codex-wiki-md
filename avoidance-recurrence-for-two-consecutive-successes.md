# Avoidance recurrence for two consecutive successes

↑ **Parent:** [Waiting time for two consecutive successes](waiting-time-for-two-consecutive-successes.md)

For [independent and identically distributed](independent-and-identically-distributed-random-variables.md) trials with constant success [probability](probability.md) $0<q<1$, let $p_n$ be the [probability](probability.md) of avoiding two consecutive successes in the first $n$ trials. An acceptable [sequence](sequence.md) starts either with a failure, leaving $n-1$ unrestricted fresh trials to check, or with a success followed by a failure, leaving $n-2$. These disjoint cases prove the recurrence for $n\geq2$.

Its [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md) are

$$
r_\pm=\frac{1-q\pm\sqrt{(1-q)(1+3q)}}2.
$$

They are distinct, and the [initial conditions](initial-condition.md) yield

$$
p_n=\frac{1-r_-}{r_+-r_-}r_+^n+\frac{r_+-1}{r_+-r_-}r_-^n.
$$

If $T$ is the completion time of the first consecutive pair, then $p_n=\mathbb P(T>n)$. The recurrence describes the whole tail distribution rather than only its mean.

## ↑ Ancestors (8)

1. [Waiting time for two consecutive successes](waiting-time-for-two-consecutive-successes.md)
2. [Stopping time](stopping-time.md)
3. [Martingale](martingale-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/8/b/ii/solution.md)
