# Geometric partition bounds for a power-law improper integral

↑ **Parent:** [Riemann sum](riemann-sum.md)

On the [geometric progression](geometric-progression.md) $x_i=(1+\epsilon)^i$, with $\epsilon>0$, the interval widths are $\epsilon(1+\epsilon)^i$. The left-endpoint [Riemann sum](riemann-sum.md) for the decreasing integrand $x^{-1-\alpha}$ is the [geometric series](geometric-series.md)

$$
U_\epsilon=\sum_{i=0}^\infty\epsilon(1+\epsilon)^{-\alpha i}
=\frac{\epsilon}{1-(1+\epsilon)^{-\alpha}}.
$$

The right-endpoint sum is $L_\epsilon=(1+\epsilon)^{-1-\alpha}U_\epsilon$. Integral comparison on each interval gives $L_\epsilon\leq I\leq U_\epsilon$. Both bounds tend to $1/\alpha$ as $\epsilon\to0^+$, proving the [improper integral](improper-integral.md) by the [squeeze theorem](squeeze-theorem.md). Although the largest interval width is unbounded on the infinite domain, these explicit upper and lower bounds justify the limit without incorrectly applying a finite-interval mesh argument to the entire half-line.

## ↑ Ancestors (7)

1. [Riemann sum](riemann-sum.md)
2. [Riemann integration](riemann-integration.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/18/a/iii/solution.md)
