<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [logarithm](../../../../../logarithm.md) requires $y>0$, and $x>0$ is given. Set $z=\log(y/x)$, so $y=xe^z$ and the [chain rule](../../../../../chain-rule.md) yields $xy'/y=1+xz'$. Dividing the [ordinary differential equation](../../../../../ordinary-differential-equation.md) by $y$ therefore gives

$$
1+xz'=1+z,\qquad xz'=z.
$$

Since $(z/x)'=(xz'-z)/x^2=0$, we obtain $z=Cx$, including the case $z=0$. Thus the general positive solution is $y=xe^{Cx}$. The [initial condition](../../../../../initial-condition.md) $y(1)=e$ gives $C=1$:

$$
\boxed{y(x)=xe^x.}
$$

For the separate decay requirement, $xe^{Cx}\to0$ precisely when $C<0$: if $C=0$, the result is $x$, and if $C>0$, it grows. Consequently the full family with the stated [limit](../../../../../limit-of-a-function.md) is

$$
\boxed{y(x)=xe^{-ax},\qquad a>0,\quad x>0.}
$$

This latter family does not also satisfy $y(1)=e$; the solution selected by that [initial condition](../../../../../initial-condition.md) grows. The identically zero [function](../../../../../function-split.md) is excluded by the original [logarithm](../../../../../logarithm.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
