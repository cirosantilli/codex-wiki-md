<h1 id="m/m1/solution">Solution</h1>

↑ **Parent:** [M1](../m1.md)

A [marginal density](../../../../marginal-density.md) is obtained by integrating out the other variable: $\boxed{f_X(x)=\int_{\mathbb R}f_{X,Y}(x,y)\,dy}$. Here independence gives $f_{X,Y}=e^{-(x^2+y^2)/2}/(2\pi)$.

The polar transformation has absolute [Jacobian determinant](../../../../jacobian-determinant.md) $r$. Consequently

$$
\boxed{f_{R,\Theta}(r,\theta)=\frac r{2\pi}e^{-r^2/2},\quad r\geq0,\ 0\leq\theta<2\pi,}
$$

with [density](../../../../density.md) zero outside this range. Integrating over the angle gives $\boxed{f_R(r)=re^{-r^2/2}}$, the [Rayleigh distribution](../../../../rayleigh-distribution.md) density. Integrating over radius, using $\int_0^\infty re^{-r^2/2}dr=1$, gives $\boxed{f_\Theta(\theta)=1/(2\pi)}$ on the angle interval. The [joint density](../../../../joint-probability-density.md) factors as the product of these marginals, so $\boxed{R\text{ and }\Theta\text{ are independent}}$. The arbitrary angle assigned at $R=0$ is irrelevant because that event has [probability](../../../../probability.md) zero.

## ↑ Ancestors (12)

1. [M1](../m1.md)
2. [M](../../m.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
