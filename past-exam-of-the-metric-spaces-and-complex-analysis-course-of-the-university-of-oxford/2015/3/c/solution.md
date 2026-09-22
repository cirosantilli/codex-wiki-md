<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

List the [roots](../../../../root-of-a-root-system.md) with their [multiplicities](../../../../multiplicity-mathematics.md). By the [factor theorem](../../../../factor-theorem.md), $Q(z)=a\prod_{k=1}^n(z-\alpha_k)$ with $a\ne0$. The [product rule](../../../../product-rule.md), followed by division where $Q(z)\ne0$, gives its [logarithmic derivative](../../../../logarithmic-derivative.md):

$$
\boxed{\frac{Q'(z)}{Q(z)}=\sum_{k=1}^n\frac1{z-\alpha_k}.}
$$

Let $Q'(\beta)=0$. If $Q(\beta)=0$ too, then $\beta$ is already one of the [roots](../../../../root-of-a-root-system.md), so either desired location conclusion follows immediately. Otherwise the displayed sum vanishes at $\beta$. If all [roots](../../../../root-of-a-root-system.md) have positive [imaginary parts](../../../../imaginary-part.md) but $\operatorname{Im}\beta\leq0$, then

$$
\operatorname{Im}\frac1{\beta-\alpha_k}
=\frac{\operatorname{Im}\alpha_k-\operatorname{Im}\beta}{|\beta-\alpha_k|^2}>0
$$

for every $k$. Their sum cannot be zero. Thus **$\operatorname{Im}\beta>0$**.

For the [unit disk](../../../../unit-disk.md) conclusion, the same sum gives an especially transparent [convex combination](../../../../convex-combination.md). Taking [complex conjugates](../../../../complex-conjugate.md) and setting $w_k=|\beta-\alpha_k|^{-2}>0$ gives

$$
0=\sum_k w_k(\beta-\alpha_k),\qquad
\boxed{\beta=\frac{\sum_k w_k\alpha_k}{\sum_k w_k}.}
$$

Therefore, if every $|\alpha_k|<1$,

$$
|\beta|\leq\frac{\sum_k w_k|\alpha_k|}{\sum_k w_k}<1.
$$

The strict inequality follows because this is a finite weighted average of numbers strictly below one. This also proves the [Gauss-Lucas theorem](../../../../gauss-lucas-theorem.md): every [critical point](../../../../critical-point.md) of a nonconstant [polynomial](../../../../polynomial-split.md) lies in the [convex hull](../../../../convex-hull.md) of its [roots](../../../../root-of-a-root-system.md). The common-root case, handled before division, is essential when [multiplicities](../../../../multiplicity-mathematics.md) occur.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
