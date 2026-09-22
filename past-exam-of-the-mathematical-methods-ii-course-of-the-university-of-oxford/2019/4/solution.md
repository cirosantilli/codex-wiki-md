<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a continuous [random variable](../../../random-variable-split.md) with [probability density function](../../../probability-density-function.md) $f_X$, its [cumulative distribution function](../../../cumulative-distribution-function.md) is

$$
F_X(x)=\Pr(X\leq x)=\int_{-\infty}^{x}f_X(u)\,du.
$$

Consequently $F_X'=f_X$ wherever the density is continuous, and almost everywhere for an absolutely continuous distribution.

Here $Y=X^2\geq0$. Thus $F_Y(y)=0$ for $y<0$. For $y\geq0$, the event $X^2\leq y$ is $-\sqrt y\leq X\leq\sqrt y$. Symmetry of the [Laplace distribution](../../../laplace-distribution.md) gives

$$
F_Y(y)=\int_{-\sqrt y}^{\sqrt y}\frac12e^{-|x|}\,dx
=\int_0^{\sqrt y}e^{-x}\,dx=1-e^{-\sqrt y}.
$$

Therefore the [square of a standard Laplace variable](../../../square-of-a-standard-laplace-variable.md) has [cumulative distribution function](../../../cumulative-distribution-function.md)

$$
\boxed{F_Y(y)=\begin{cases}0,&y<0,\\1-e^{-\sqrt y},&y\geq0.\end{cases}}
$$

It is continuous at zero, so there is no point mass there. As a check, its [probability density function](../../../probability-density-function.md) for $y>0$ is $e^{-\sqrt y}/(2\sqrt y)$, whose integral becomes $\int_0^\infty e^{-u}\,du=1$ after setting $u=\sqrt y$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
