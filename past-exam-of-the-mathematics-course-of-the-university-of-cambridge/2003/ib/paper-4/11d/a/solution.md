<h1 id="11d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [separation of variables](../../../../../../separation-of-variables.md), $\phi=R(r)\Theta(\theta)$. After multiplying the [Laplace equation](../../../../../../laplace-equation.md) by $r^2/(R\Theta)$, the two separated equations are

$$
\Theta''+\lambda\Theta=0,\qquad r^2R''+rR'-\lambda R=0.
$$

Single-valuedness requires $2\pi$-periodicity. Thus the nonconstant angular modes have $\lambda=n^2$, $n=1,2,\ldots$, and angular factors $\cos n\theta,\sin n\theta$. Their radial factors are $r^n,r^{-n}$. The zero mode has constant angular factor and radial solution $A+B\log r$; a term proportional to $\theta$ would be multivalued.

Finiteness at the origin removes the logarithm and negative powers. In the [disk](../../../../../../disk-mathematics.md) the general regular harmonic expansion is

$$
\boxed{\phi=A_0+\sum_{n\ge1}r^n(A_n\cos n\theta+B_n\sin n\theta)}.
$$

For the exterior, regularity at every finite radius allows

$$
\boxed{\phi=C_0+D_0\log r+\sum_{n\ge1}\big[(C_nr^n+D_nr^{-n})\cos n\theta+(E_nr^n+F_nr^{-n})\sin n\theta\big]}.
$$

Coefficients must give convergent harmonic expansions on the domain and the intended boundary regularity at $r=a$. If “finite” is intended to mean bounded as $r\to\infty$, then $D_0=C_n=E_n=0$ and only the constant and decaying modes remain. Infinity is not included in the printed interval; moreover part (b)'s uniform background flow necessarily has an unbounded potential. Stating both interpretations avoids discarding that background mode.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11D](../../11d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
