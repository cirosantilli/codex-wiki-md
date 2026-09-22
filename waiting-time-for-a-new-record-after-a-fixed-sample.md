# Waiting time for a new record after a fixed sample

↑ **Parent:** [Order statistic](order-statistic.md)

For independent identically distributed observations with continuous [cumulative distribution function](cumulative-distribution-function.md) $F$, fix the maximum $Y_n$ of the first $n\geq1$ observations and let $\tau$ be the first subsequent observation exceeding it. The [probability integral transform](probability-integral-transform.md) gives $U=F(Y_n)$ density $nu^{n-1}$ on $(0,1)$. Conditional on $U=u$, $\tau$ has a [geometric distribution](geometric-distribution.md) of parameter $1-u$. Therefore

$$
P(\tau=k)=n\int_0^1u^{n+k-2}(1-u)\,du
=\frac n{(n+k-1)(n+k)},\qquad
P(\tau>k)=\frac n{n+k}.
$$

The masses sum to one, so the waiting time is finite almost surely, but the [tail-sum formula for expectation](tail-sum-formula-for-expectation.md) gives $E\tau=\infty$. These conclusions require only continuity of $F$, not a density or a strictly increasing distribution function.

## ↑ Ancestors (6)

1. [Order statistic](order-statistic.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/10f/d/solution.md)
