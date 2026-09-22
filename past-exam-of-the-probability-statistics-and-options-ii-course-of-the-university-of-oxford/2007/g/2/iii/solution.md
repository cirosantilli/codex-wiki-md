<h1 id="g/2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The functional is unbounded above. Let $\ell$ be the positive affine interpolant of the endpoint values and choose a nonnegative, nonzero, continuously differentiable $h$ vanishing at both endpoints. The admissible functions $y_M=\ell+Mh$ satisfy

$$
J[y_M]\ge2\pi\int_{x_1}^{x_2}y_M\,dx\longrightarrow\infty.
$$

This excludes a global maximum, but **does not prove that a stationary curve is a minimum**. The concluding assertion is false without additional conditions.

An explicit counterexample uses $x_1=-2$, $x_2=2$, $y_1=y_2=\cosh2$ and the stationary function $y=\cosh x$. Its [second variation](../../../../../second-variation.md), for a perturbation $h$ vanishing at the endpoints, is

$$
\frac{\delta^2J[h]}{2\pi}
=\int_{-2}^{2}\bigl(2\tanh x\,hh'+\operatorname{sech}^2x\,h'^2\bigr)dx
=\int_{-2}^{2}\operatorname{sech}^2x\,(h'^2-h^2)\,dx.
$$

Choose $h=1-x^2/4$. Since $\operatorname{sech}^2x\le4e^{-2|x|}$, the positive contribution is at most $\int_{\mathbb R}x^2e^{-2|x|}dx=1/2$. On $[-1,1]$, $h^2\ge9/16$, so the magnitude of the negative contribution is at least $(9/8)\tanh1>9/16>1/2$. Thus $\delta^2J[h]<0$. Small perturbations in this direction preserve positivity and the endpoint data while decreasing [surface area](../../../../../surface-area.md). Consequently this [catenoid](../../../../../catenoid.md) is not a local minimum. The valid conclusion from part (ii) is a necessary stationary form; minimization requires a separate stability and existence analysis.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [G](../../../g.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
