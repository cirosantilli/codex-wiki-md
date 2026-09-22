<h1 id="37a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $U(r)$ be the radial velocity scale. Advection-viscosity balance gives $U^2/r\sim\nu U/\delta^2$, while the conserved momentum flux gives $F\sim U^2r\delta$. Eliminating $U$ yields $\delta/r\sim(\nu^2/F)^{1/3}$, a constant, so $\delta=Cr$ and $U\propto r^{-1}$.

The [streamfunction](../../../../../../stream-function.md) automatically satisfies incompressibility. With the proposed form it gives

$$
u_r=\frac A r f'(\eta),\qquad
u_z=-\frac{AC}{r}[f(\eta)-\eta f'(\eta)],\qquad\eta=z/(Cr),
$$

where $u_r,u_z$ are the two velocity components. Differentiation in the momentum equation cancels the terms proportional to $\eta f'f''$ and leaves

$$
-\frac{A^2}{r^3}(f'^2+ff'')=\frac{\nu A}{C^2r^3}f'''.
$$

Choose $AC^2=\nu$. The momentum integral is $F=A^2C\int f'^2d\eta$, so choosing $A^2C=F$ makes its normalization one. Therefore

$$
\boxed{A=(F^2/\nu)^{1/3},\quad C=(\nu^2/F)^{1/3},\quad
-f'^2-ff''=f''',\quad\int_{-\infty}^{\infty}f'^2d\eta=1.}
$$

Reflection symmetry gives $u_z=0$ and $\partial_zu_r=0$ at zero. Taking the [streamfunction](../../../../../../stream-function.md)'s odd representative makes $f(0)=0$, and symmetry gives $f''(0)=0$; far-field decay gives $f'\to0$. The factor $f$ multiplying $f''$ is present in the original PDF but missing from the TeX aid; the direct substitution confirms the PDF equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
