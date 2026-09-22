# Positive difference of independent exponential waiting times

↑ **Parent:** [Competing exponential clocks](competing-exponential-clocks.md)

Let $S,T$ be [independent random variables](independent-random-variables.md) with [exponential distributions](exponential-distribution.md) of respective positive rates $\alpha,\beta$. Condition on $T=t$ and use the [survival function](survival-function.md) of $S$:

$$
P(S-T>u)=\int_0^\infty\beta e^{-\beta t}e^{-\alpha(t+u)}dt
=\frac{\beta}{\alpha+\beta}e^{-\alpha u},\qquad u\geq0.
$$

At $u=0$ this is $P(S>T)$. Dividing by that [probability](probability.md) proves that the positive difference conditional on $S>T$ again has an [exponential distribution](exponential-distribution.md) with rate $\alpha$. The [memorylessness of the exponential distribution](memorylessness-of-the-exponential-distribution.md) persists after an independent competing event has already occurred. Replacing the difference by a negative sentinel when $S\leq T$ adds an [atom of a measure](atom-measure-theory.md) of mass $\alpha/(\alpha+\beta)$ at that sentinel without changing the positive tail.

## ↑ Ancestors (9)

1. [Competing exponential clocks](competing-exponential-clocks.md)
2. [Exponential distribution](exponential-distribution.md)
3. [Continuous probability distribution](continuous-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/12/f/solution.md)
