<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $x\ne\pm1$, write the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) as

$$
y'+\frac{2x}{1-x^2}y=\frac{x(1-x)}{1-x^2}.
$$

An [integrating factor](../../../../../integrating-factor.md) on each interval avoiding $\pm1$ is $\mu(x)=1/(1-x^2)$; multiplication by a nonzero constant, including a sign, is immaterial. Therefore

$$
\left(\frac{y}{1-x^2}\right)'
=\frac{x(1-x)}{(1-x^2)^2}
=\frac{x}{(1-x)(1+x)^2}.
$$

The [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is

$$
\frac{x}{(1-x)(1+x)^2}
=\frac{1}{4(1-x)}+\frac{1}{4(1+x)}-\frac{1}{2(1+x)^2}.
$$

Integrating gives the [general solution](../../../../../general-solution.md)

$$
\boxed{y(x)=\frac{1-x}{2}+
(1-x^2)\left(C+\frac14\log\left|\frac{1+x}{1-x}\right|\right),
\qquad x\ne\pm1.}
$$

The constant is independent on each connected interval of definition. At the singular points the undivided [differential equation](../../../../../differential-equation-split.md) forces $y(1)=0$ and $y(-1)=1$. The displayed family tends to these values, but its [derivative](../../../../../derivative.md) has a logarithmic divergence there, so no member extends as a [differentiable function](../../../../../differentiable-function.md) through either singular point.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
