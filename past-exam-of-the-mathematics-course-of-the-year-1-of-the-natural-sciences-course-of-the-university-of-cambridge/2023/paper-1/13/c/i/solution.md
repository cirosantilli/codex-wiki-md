<h1 id="13/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the substitution $v=y/x$ for a [homogeneous first-order differential equation](../../../../../../homogeneous-first-order-differential-equation.md). Since $y'=v+xv'$, it gives

$$
xv'=\tan v.
$$

Where $\sin v\ne0$, this [separable differential equation](../../../../../../separable-differential-equation.md) integrates to $\ln|\sin v|=\ln|x|+C$, hence $\sin v=C_1x$. One can obtain the same relation without division by $\sin v$: the equation gives $(\sin v)'=(\sin v)/x$, so $\sin v=C_1x$, including $\sin v\equiv0$.

All real branches of the [inverse sine](../../../../../../inverse-sine.md) are captured by

$$
\boxed{y(x)=x\left[k\pi+(-1)^k\arcsin(Cx)\right],\qquad C\in\mathbb R,\quad k\in\mathbb Z.}
$$

Each branch is used on an [interval](../../../../../../interval-mathematics.md) with $x\ne0$ and $|Cx|<1$, with fixed $k$. The strict inequality excludes zeros of $\cos(y/x)$, where the original [tangent](../../../../../../tangent.md) is undefined. When $C=0$, the formula includes all straight-line solutions $y=k\pi x$. Keeping both families of [inverse sine](../../../../../../inverse-sine.md) branches is essential for the two different [initial conditions](../../../../../../initial-condition.md) below.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [13](../../../13.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
