<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To invert the complex [cosine](../../../../cosine.md), let $z=\cos w$ and put $u=e^{iw}$. Since the [exponential function](../../../../exponential-function.md) is nonzero, $u\ne0$, and [Euler's formula](../../../../euler-s-formula.md) gives $2z=u+u^{-1}$. Multiplying by $u$ yields the [quadratic equation](../../../../quadratic-equation.md) $u^2-2zu+1=0$. Thus

$$
u=z\pm\sqrt{z^2-1}=z\pm i\sqrt{1-z^2}.
$$

Choosing either [square root](../../../../square-root.md) of $1-z^2$ merely exchanges the two signs. The two values have product one, so neither vanishes; taking a [complex logarithm](../../../../complex-logarithm.md) is legitimate.

For each choice of sign, all solutions of $e^{iw}=u$ satisfy $iw=\operatorname{Log}u+2\pi in$. Therefore the full inverse relation is

$$
\boxed{w=-i\operatorname{Log}\left(z\pm i\sqrt{1-z^2}\right)+2\pi n,\qquad n\in\mathbb Z.}
$$

Conversely, exponentiating any displayed value recovers one root of the [quadratic equation](../../../../quadratic-equation.md), and hence $(e^{iw}+e^{-iw})/2=z$, proving completeness. With a multivalued [complex logarithm](../../../../complex-logarithm.md), the $2\pi n$ term is already included and this is the source's compact formula for [inverse cosine](../../../../arccosine.md).

The principal [inverse cosine](../../../../arccosine.md) requires compatible choices of [logarithm branch](../../../../branch-of-the-complex-logarithm.md), [square root](../../../../square-root.md) and sign. Both signs cannot represent that same principal function indiscriminately: at $z=0$, the two principal-log values are $\pi/2$ and $-\pi/2$, whereas the principal $\arccos0$ is $\pi/2$. Thus the printed $\pm$ is correct for the inverse relation, not a pair of interchangeable principal-value formulas.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
