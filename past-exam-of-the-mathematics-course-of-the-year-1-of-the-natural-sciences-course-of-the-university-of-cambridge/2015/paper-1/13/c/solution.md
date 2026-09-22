<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [heat equation](../../../../../heat-equation.md) is linear and homogeneous in $u$: the operator $L=\partial_t-\lambda\partial_x^2$ satisfies $L(Au_1+Bu_2)=ALu_1+BLu_2$. Thus the [superposition principle](../../../../../superposition-principle.md) applies to its solutions. Spatial translations are also allowed because the coefficients are constant.

Choose $a=1/(4\lambda)$ in part (b) and multiply by $\sqrt a$ to make the initial amplitude one. Taking the two shifts $b=1$ and $b=-1$ then gives

$$
\boxed{u(x,t)=\frac1{\sqrt{1+4\lambda t}}
\left\{\exp\left[-\frac{(x+1)^2}{1+4\lambda t}\right]
+\exp\left[-\frac{(x-1)^2}{1+4\lambda t}\right]\right\}.}
$$

At $t=0$ this reproduces both initial peaks. Each term is an instance of [Gaussian initial data for the heat equation](../../../../../gaussian-initial-data-for-the-heat-equation.md), so their sum satisfies the equation. Its extension to negative times is a real smooth solution precisely on the connected interval

$$
\boxed{-\frac1{4\lambda}<t<0.}
$$

At the lower endpoint the peaks narrow without bound and their heights diverge; there is no finite classical continuation there. For positive times each peak spreads and decreases in height while preserving its integral.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
