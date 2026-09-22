<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [integrating factor](../../../../../../integrating-factor.md) for this [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md) is $\mu(x)=e^{x^3/3}$. Multiplication gives an exact [derivative](../../../../../../derivative.md):

$$
\frac{d}{dx}\left(e^{x^3/3}y\right)=x^2e^{x^3/3}=\frac{d}{dx}e^{x^3/3}.
$$

Consequently $y=1+Ce^{-x^3/3}$. The [initial condition](../../../../../../initial-condition.md) $y(1)=2$ gives $C=e^{1/3}$, so the [initial value problem](../../../../../../initial-value-problem.md) has solution

$$
\boxed{y(x)=1+\exp\left(\frac{1-x^3}{3}\right),\qquad x\in\mathbb R.}
$$

The [integrating factor](../../../../../../integrating-factor.md) calculation determines every solution, and the [initial condition](../../../../../../initial-condition.md) fixes its remaining [constant of integration](../../../../../../constant-of-integration.md) uniquely.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
