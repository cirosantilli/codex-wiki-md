<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [integrating factor](../../../integrating-factor.md) for $u'+P(x)u=Q(x)$ is a nonzero function $\mu(x)=\exp(\int P(x)dx)$, chosen so that $(\mu u)'=\mu Q$. Integrating this total derivative reduces the first-order [linear ordinary differential equation](../../../linear-ordinary-differential-equation-split.md) to one quadrature.

For the given nonlinear equation, let $u=y^2$, so $u'=2yy'$. Multiplication by $2y$ gives $u'+u=x^2+2x$. Using the [integrating factor](../../../integrating-factor.md) $e^x$, or recognizing the particular solution $u=x^2$, yields $u=x^2+Ce^{-x}$. The initial value gives $C=1$ and selects the positive branch:

$$
\boxed{y(x)=\sqrt{x^2+e^{-x}}.}
$$

The radicand is strictly positive for every real $x$. This solution never reaches the singular denominator $y=0$ of the original equation, so multiplication by $y$ has introduced no forbidden crossing. The negative branch would violate $y(0)=1$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2017](../../2017-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
