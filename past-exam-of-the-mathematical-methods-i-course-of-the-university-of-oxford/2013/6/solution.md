<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Here the dependent variable is $x$ and the independent variable is $y$. Multiplying the equation by $2x$ and setting $q=x^2$ gives a linear equation:

$$
\frac{dq}{dy}-\frac4yq=2y.
$$

An [integrating factor](../../../integrating-factor.md) is $y^{-4}$, so

$$
\frac d{dy}(q y^{-4})=2y^{-3},\qquad
q y^{-4}=-y^{-2}+C.
$$

Thus $x^2=Cy^4-y^2$. The initial point $(x,y)=(1,1)$ fixes $C=2$, and the positive branch through that point is

$$
\boxed{x(y)=y\sqrt{2y^2-1},\qquad y>\frac1{\sqrt2}.}
$$

Equivalently, inverting this branch gives

$$
\boxed{y(x)=\frac12\sqrt{1+\sqrt{1+8x^2}},\qquad x>0.}
$$

The source equation contains $xy$ in the denominator. The endpoint with $x=0$ is therefore excluded even though the inverse expression has a finite limit there. A negative-$x$ branch cannot be joined through that endpoint to produce a solution $x(y)$ of the original equation. The interval shown is the maximal real positive branch containing the initial point.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2013](../../2013-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
