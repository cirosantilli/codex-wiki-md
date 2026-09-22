<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use coordinates $x^0=t$, $x^1=x$ and first compute the mixed [canonical stress-energy tensor](../../../../canonical-stress-energy-tensor.md) supplied by spacetime translations:

$$
T^\mu{}_{\nu}=\sum_{j=1}^2\frac{\partial\mathcal L}{\partial(\partial_\mu\phi_j)}\partial_\nu\phi_j-\delta^\mu{}_{\nu}\mathcal L.
$$

Define the energy density $\mathcal E=\phi_{1,t}\phi_{2,t}+c^2\phi_{1,x}\phi_{2,x}$ and $\mathcal P=\phi_{1,t}\phi_{2,x}+\phi_{2,t}\phi_{1,x}$. Direct substitution gives

$$
\boxed{T^\mu{}_{\nu}=\begin{pmatrix}\mathcal E&\mathcal P\\-c^2\mathcal P&-\mathcal E\end{pmatrix}.}
$$

The two wave equations imply

$$
\partial_t\mathcal E=c^2\partial_x\mathcal P,\qquad\partial_t\mathcal P=\partial_x\mathcal E.
$$

For example, differentiating $\mathcal E$ and replacing each $\phi_{j,tt}$ by $c^2\phi_{j,xx}$ gives exactly $c^2\partial_x\mathcal P$ by the [product rule](../../../../product-rule.md). These are respectively the two component equations $\boxed{\partial_\mu T^\mu{}_{\nu}=0}$, establishing [stress-energy conservation](../../../../stress-energy-conservation.md) explicitly.

If the given metric $g^{\mu\nu}=\operatorname{diag}(1,-1)$ is used to raise the second index in these unrescaled coordinates, the result is $T^{\mu\nu}=\begin{pmatrix}\mathcal E&-\mathcal P\\-c^2\mathcal P&\mathcal E\end{pmatrix}$, still conserved. To display the symmetric relativistic form with light speed $c$, choose $X^0=ct$, $X^1=x$ instead. With $\partial_{X^0}=c^{-1}\partial_t$, the corresponding tensor is

$$
\boxed{\mathcal T^{\mu\nu}=\begin{pmatrix}\mathcal E&-c\mathcal P\\-c\mathcal P&\mathcal E\end{pmatrix},\qquad\partial_{X^\mu}\mathcal T^{\mu\nu}=0.}
$$

This states the coordinate convention explicitly rather than setting $c=1$ in some components but not others.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
