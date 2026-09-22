# Quadratic expansion of a cumulant-generating function

↑ **Parent:** [Cumulant-generating function](cumulant-generating-function.md)

Suppose the [moment-generating function](moment-generating-function.md) $M_X$ is finite on an open [interval](interval-mathematics.md) around zero. Its [cumulant-generating function](cumulant-generating-function.md) $K_X=\log M_X$ satisfies $K_X(0)=0$, $K_X'(0)=\mathbb E X=\mu$ and $K_X''(0)=\operatorname{Var}(X)=\sigma^2$. Indeed,

$$
K_X'=\frac{M_X'}{M_X},\qquad K_X''=\frac{M_X''}{M_X}-\left(\frac{M_X'}{M_X}\right)^2,
$$

and $M_X(0)=1$. The [Taylor expansion](taylor-expansion.md) gives the displayed formula, with [little o notation](little-o-notation.md) describing the remainder. Finiteness in a neighborhood justifies differentiation: polynomial factors times $e^{tX}$ are dominated on a smaller interval by constants times two slightly larger [exponential moments](exponential-moment.md).

## ↑ Ancestors (8)

1. [Cumulant-generating function](cumulant-generating-function.md)
2. [Moment-generating function](moment-generating-function.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2017/2/b/i/solution.md)
- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2017/2/b/iii/solution.md)
- [Weighted central limit theorem with negligible maximum weight](weighted-central-limit-theorem-with-negligible-maximum-weight.md)
