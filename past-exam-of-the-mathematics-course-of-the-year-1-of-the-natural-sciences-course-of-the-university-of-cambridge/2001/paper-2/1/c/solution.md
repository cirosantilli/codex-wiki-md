<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For this [homogeneous first-order differential equation](../../../../../homogeneous-first-order-differential-equation.md), set $v=y/x$, with $x\ne0$. The [product rule](../../../../../product-rule.md) gives $y'=v+xv'$, and substitution simplifies the equation to

$$
(1+2ve^v)xv'=2(1-v^2e^v).
$$

The useful further substitution is $w=e^{-v}-v^2$. Its [chain rule](../../../../../chain-rule.md) [derivative](../../../../../derivative.md) satisfies

$$
x\frac{dw}{dx}=-(e^{-v}+2v)xv'=-2(e^{-v}-v^2)=-2w.
$$

Thus $(x^2w)'=0$. Replacing $v$ and $w$ gives the [implicit solution](../../../../../implicit-solution.md)

$$
\boxed{x^2e^{-y/x}-y^2=C,\qquad x\ne0.}
$$

No division by $w$ was needed, so the level $C=0$ is included. A direct verification also identifies the [integrating factor for a differential one-form](../../../../../integrating-factor-for-a-differential-one-form.md):

$$
d\bigl(x^2e^{-y/x}-y^2\bigr)=e^{-y/x}(2x+y)\,dx-(xe^{-y/x}+2y)\,dy.
$$

Setting this [exact differential](../../../../../exact-differential.md) to zero recovers precisely the original equation after multiplication by the nonzero factor $e^{y/x}$. The coefficient $1+2ve^v$ never vanishes for real $v$, since $ve^v\geq-1/e$ implies $1+2ve^v\geq1-2/e>0$. Hence these [level sets](../../../../../level-set.md) give local [function graphs](../../../../../graph-of-a-function.md) $y(x)$ everywhere with $x\ne0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
