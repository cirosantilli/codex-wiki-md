<h1 id="8c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial point has $H=1/4$. On the branch leaving $(1/2,0)$ toward negative $y$,

$$
x^2=\frac14-y^2+y^4=\left(\frac12-y^2\right)^2,
\qquad x=\frac12-y^2.
$$

Since $\dot y=-x$, the required scalar equation is

$$
\dot y=y^2-\frac12,
\qquad y(0)=0.
$$

Its solution is

$$
\boxed{y(t)=-\frac1{\sqrt2}\tanh\left(\frac{t}{\sqrt2}\right)}.
$$

At $(x,y)=(1/4,-1/2)$, this requires $\tanh(t/\sqrt2)=1/\sqrt2$. Using the [inverse hyperbolic tangent](../../../../../../inverse-hyperbolic-tangent.md),

$$
\boxed{t=\sqrt2\,\operatorname{artanh}\frac1{\sqrt2}
=\sqrt2\log(1+\sqrt2)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8C](../../8c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
