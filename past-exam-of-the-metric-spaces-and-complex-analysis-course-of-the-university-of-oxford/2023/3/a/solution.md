<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

At every $z=x+iy\in U$, the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) are

$$
\boxed{u_x=v_y,\qquad u_y=-v_x}.
$$

To derive them from [complex differentiability](../../../../complex-differentiability.md), approach $z$ along real increments $h$. The [complex derivative](../../../../complex-derivative.md) gives

$$
f'(z)=\lim_{h\to0}\frac{f(z+h)-f(z)}h=u_x+iv_x.
$$

Approaching along imaginary increments $ih$ instead gives

$$
f'(z)=\lim_{h\to0}\frac{f(z+ih)-f(z)}{ih}=v_y-iu_y.
$$

These limits exist because $f$ is [holomorphic](../../../../holomorphic-function-split.md). Equating their real and imaginary parts proves the equations, together with $f'=u_x+iv_x=v_y-iu_y$.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
