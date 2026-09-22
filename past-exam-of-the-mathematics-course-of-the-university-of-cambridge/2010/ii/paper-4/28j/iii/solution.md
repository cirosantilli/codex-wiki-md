<h1 id="28j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the interior stationary candidate, let $\gamma=1/(\alpha+\beta-1)$. Its formal relation $\ell=1-\beta c/\alpha$ gives

$$
\dot x-rx=1-\frac{\alpha+\beta}{\alpha}Ce^{-\gamma rt}.
$$

Integration therefore gives $x=Ae^{rt}+Be^{-\gamma rt}-1/r$. Imposing $x(0)=x_0$ and $x(T)=0$ yields

$$
A=\frac{1-e^{-\gamma rT}(1+rx_0)}{r(e^{rT}-e^{-\gamma rT})},\qquad
B=\frac{(1+rx_0)e^{rT}-1}{r(e^{rT}-e^{-\gamma rT})}.
$$

This recovers the printed expression algebraically, but **does not turn its stationary control into an optimum**; it may also violate $\ell\ge0$.

The actual globally optimal wealth from part (ii) is

$$
\boxed{x(t)=
\begin{cases}
(x_0+r^{-1})e^{rt}-r^{-1},&0\le t\le t_*,\\[2mm]
Ce^{rt}\dfrac{e^{aT}-e^{at}}a,&t_*\le t\le T,
\end{cases}\qquad a=\frac{r\alpha}{1-\alpha}.}
$$

The budget equation makes the two branches agree at the switch. Direct differentiation gives $\dot x=rx+\ell-c$ on both branches, and $x(T)=0$. This solution remains nonnegative throughout, even though only the terminal nonnegativity constraint was imposed. It provides the complete corrected solution for $\alpha+\beta>1$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
