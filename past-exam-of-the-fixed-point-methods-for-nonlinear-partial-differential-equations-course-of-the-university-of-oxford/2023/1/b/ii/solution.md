<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [radial retraction of a punctured ball](../../../../../radial-retraction-of-a-punctured-ball.md) gives a [retraction](../../../../../retraction.md): project away from the removed interior point until reaching the [unit sphere](../../../../../unit-sphere.md). Write $a=x_0$, $v=x-a\ne0$, and set

$$
\tau(x)=\frac{-a\cdot v+\sqrt{(a\cdot v)^2+(1-|a|^2)|v|^2}}{|v|^2},
\qquad
\boxed{r(x)=a+\tau(x)(x-a).}
$$

The equation $|a+tv|^2=1$ is the [quadratic equation](../../../../../quadratic-equation.md)

$$
|v|^2t^2+2(a\cdot v)t+|a|^2-1=0.
$$

Its constant term is negative, so it has exactly one positive root, namely $\tau(x)$. Since $|a+v|=|x|\leq1$, that positive root satisfies $\tau(x)\geq1$. Thus $r(x)\in\partial\mathbb B^n$ for every $x\ne a$ in the [closed unit ball](../../../../../closed-unit-ball.md).

The displayed expression is a [continuous map](../../../../../continuous-map.md) on the punctured [closed unit ball](../../../../../closed-unit-ball.md): its denominator is nonzero there, and its [square root](../../../../../square-root.md) has strictly positive argument. If $|x|=1$, $t=1$ is the unique positive root, so $r(x)=x$. These are exactly the requirements for a [retraction](../../../../../retraction.md). The missing interior point is essential: the formula need not extend continuously to $a$, in agreement with the [no-retraction theorem](../../../../../no-retraction-theorem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
