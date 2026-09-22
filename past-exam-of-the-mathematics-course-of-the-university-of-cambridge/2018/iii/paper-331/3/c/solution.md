<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $U=U_0$ and $\beta=0$, the [Orr-Sommerfeld equation](../../../../../../orr-sommerfeld-equation.md) factors into constant-coefficient operators:

$$
(D^2-\alpha^2)(D^2-\gamma^2)\widehat v=0,\qquad
\boxed{\gamma^2=\alpha^2+iRe(\alpha U_0-\omega).}
$$

For distinct nonzero characteristic roots, the general solution is

$$
\boxed{\widehat v=a_1e^{\alpha y}+a_2e^{-\alpha y}+a_3e^{\gamma y}+a_4e^{-\gamma y}.}
$$

Either square-root choice for $\gamma$ gives the same solution space. The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) and impermeability impose $\widehat v=D\widehat v=0$ at each wall.

The displayed exponential basis needs the usual repeated-root qualification. If $\gamma^2=\alpha^2\ne0$, replace it by $(a_1+a_2y)e^{\alpha y}+(a_3+a_4y)e^{-\alpha y}$. If just one root pair is zero, that pair contributes $1,y$; if both pairs are zero, the basis is $1,y,y^2,y^3$. These are the complete limiting cases, not four independent copies of a repeated exponential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
