<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $R$ be a second [cubic spline](../../../../../cubic-spline.md) matching the same values and endpoint [derivatives](../../../../../derivative.md). The [minimum roughness property of a clamped cubic spline](../../../../../minimum-roughness-property-of-a-clamped-cubic-spline.md) applied with $S$ as the minimizing [cubic spline](../../../../../cubic-spline.md) gives $J(R)\geq J(S)$, where $J(u)=\int_{x_0}^{x_n}(u'')^2\,dx$. Applying the same argument with their roles exchanged gives $J(S)\geq J(R)$. Hence equality holds, and the exact identity from part (i) yields

$$
\int_{x_0}^{x_n}(R''-S'')^2\,dx=0.
$$

The [integrand](../../../../../integrand.md) is continuous and nonnegative. If it were positive somewhere, it would have a positive [integral](../../../../../integral-split.md) over a small [interval](../../../../../interval-mathematics.md). It follows that $R''=S''$ everywhere. Consequently $R-S$ is an [affine function](../../../../../affine-function.md). Its value and [derivative](../../../../../derivative.md) vanish at $x_0$, so it is identically zero. Thus $R=S$, proving uniqueness of the [clamped cubic spline](../../../../../clamped-cubic-spline.md) with the prescribed data. Existence was assumed in the question; this argument establishes the remaining uniqueness claim.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
