<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real solutions work on $x>-1$. Dividing by $2(1+x)$ puts the [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md) into the form

$$
y'+\left(-1+\frac1{2(1+x)}\right)y=\frac{x^2}{2\sqrt{1+x}}.
$$

Its [integrating factor](../../../../integrating-factor.md) is

$$
\mu(x)=\exp\left(-x+\frac12\ln(1+x)\right)=e^{-x}\sqrt{1+x}.
$$

The [product rule](../../../../product-rule.md) therefore gives

$$
(\mu y)'=\frac12x^2e^{-x}.
$$

Twice using [integration by parts](../../../../integration-by-parts.md), or differentiating the proposed antiderivative, gives $\int x^2e^{-x}\,dx=-e^{-x}(x^2+2x+2)$. Hence

$$
\boxed{y(x)=\frac{Ce^x-\tfrac12(x^2+2x+2)}{\sqrt{1+x}},\qquad x>-1.}
$$

The endpoint $x=-1$ is singular. A finite continuous extension would require $C=e/2$, but then, with $h=x+1\downarrow0$, $y=\tfrac12\sqrt h+O(h^{3/2})$. Its derivative diverges, so even this choice has no differentiable extension to that endpoint.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
