<h1 id="m/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [joint probability density function](../../../../joint-probability-density.md), [independence](../../../../independent-random-variables.md) is equivalent to $f(x,y)=f_X(x)f_Y(y)$ almost everywhere. The displayed density is valid for $|\rho|<1$. Complete the square:

$$
\frac{x^2-2\rho xy+y^2}{1-\rho^2}
=x^2+\frac{(y-\rho x)^2}{1-\rho^2}.
$$

Integrating the second normal factor over $y$ gives

$$
\boxed{f_X(x)=\frac1{\sqrt{2\pi}}e^{-x^2/2}.}
$$

Dividing the [joint probability density function](../../../../joint-probability-density.md) by this marginal yields the conditional law

$$
\boxed{Y\mid X=x\sim N(\rho x,1-\rho^2).}
$$

For $\rho=0$ the [joint probability density function](../../../../joint-probability-density.md) factors and the variables are independent. If $\rho\neq0$, the [conditional mean](../../../../conditional-expectation.md) depends on $x$, so [independence](../../../../independent-random-variables.md) fails; equivalently their [covariance](../../../../covariance.md) is $\rho$.

Define $Z=(Y-\rho X)/\sqrt{1-\rho^2}$. In the change of variables $y=\rho x+\sqrt{1-\rho^2}z$, the Jacobian $\sqrt{1-\rho^2}$ cancels the remaining density factor, leaving the product of two [standard normal](../../../../standard-normal-distribution.md) densities. Thus $Z$ is [standard normal](../../../../standard-normal-distribution.md) and independent of $X$. One choice is

$$
\boxed{a=-\frac{\rho}{\sqrt{1-\rho^2}},\qquad
b=\frac1{\sqrt{1-\rho^2}}.}
$$

Changing both signs gives the other standardized choice. The density transformation proves [independence](../../../../independent-random-variables.md) directly rather than inferring it from zero [covariance](../../../../covariance.md) without a joint-normal justification.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [M](../../m.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
