<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On the interval $x>0$ containing the initial point, divide the [linear ordinary differential equation](../../../linear-ordinary-differential-equation-split.md) by $x$ to obtain $y'-2y/x=x$. Its [integrating factor](../../../integrating-factor.md) is $e^{\int-2\,dx/x}=x^{-2}$, giving

$$
\frac{d}{dx}\left(\frac{y}{x^2}\right)=\frac1x,
\qquad y=x^2(\ln x+C).
$$

The initial condition gives $1=C$. Hence

$$
\boxed{y(x)=x^2(1+\ln x),\qquad x>0.}
$$

Direct differentiation gives $y'=x(3+2\ln x)$, so $xy'-2y=x^2$ and $y(1)=1$. The coefficient of $y'$ vanishes at zero; the boxed expression is the solution on the regular initial-value interval, rather than an assertion of unique continuation through zero.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
