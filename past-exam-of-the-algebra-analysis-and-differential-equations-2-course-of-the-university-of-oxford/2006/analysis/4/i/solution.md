<h1 id="analysis/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A function is [holomorphic](../../../../../holomorphic-function-split.md) on an [open set](../../../../../open-set.md) if it is [complex differentiable](../../../../../complex-differentiability.md) at every point of that set. At $z_0=x_0+iy_0$, take difference quotients first along real increments. Their limit is $f'(z_0)$, so $u_x=\operatorname{Re}f'(z_0)$ and $v_x=\operatorname{Im}f'(z_0)$. Along imaginary increments,

$$
\frac{f(z_0+ih)-f(z_0)}h\longrightarrow if'(z_0),
$$

so $u_y=-\operatorname{Im}f'(z_0)$ and $v_y=\operatorname{Re}f'(z_0)$. These limits prove existence of all four [partial derivatives](../../../../../partial-derivative.md) and the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) $u_x=v_y$, $u_y=-v_x$.

For the first example, the identity function and the reciprocal function are [holomorphic](../../../../../holomorphic-function-split.md) away from zero, so **$f$ is [holomorphic](../../../../../holomorphic-function-split.md) on the given domain**, with

$$
\boxed{f'(z)=1-z^{-2}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [Analysis](../../../analysis.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
