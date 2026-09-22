<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

For static fields, the [Maxwell equations](../../../../../maxwell-equations.md) give $\nabla\times B=\mu_0J$ and $\nabla\cdot B=0$. Write $B=\nabla\times A$. A [gauge transformation](../../../../../gauge-transformation.md) $A\mapsto A+\nabla\chi$ leaves $B$ unchanged; choose $\Delta\chi=-\nabla\cdot A$ to impose the [Coulomb gauge](../../../../../coulomb-gauge.md). Then

$$
\nabla\times(\nabla\times A)=\nabla(\nabla\cdot A)-\Delta A=\mu_0J,
\qquad \boxed{-\Delta A=\mu_0J.}
$$

For a localized conserved current with the potential chosen to vanish at infinity, the supplied fundamental solution gives the [magnetic vector potential](../../../../../magnetic-vector-potential.md)

$$
A(x)=\frac{\mu_0}{4\pi}\int\frac{J(r)}{|x-r|}\,d^3r.
$$

Its divergence vanishes by integration by parts and $\nabla\cdot J=0$. For a filamentary loop the current integral becomes $I\oint_Ldr$, so

$$
\boxed{A(x)=\frac{\mu_0I}{4\pi}\oint_L\frac{dr}{|x-r|}.}
$$

For $R=|x|$ much larger than the fixed loop size, expand $|x-r|^{-1}=R^{-1}+(x\cdot r)R^{-3}+O(R^{-3})$. The leading constant term integrates to zero because $\oint dr=0$. Therefore

$$
A(x)=\frac{\mu_0I}{4\pi R^3}\oint(x\cdot r)\,dr+O(R^{-3}).
$$

The vector triple-product identity gives $x\times(r\times dr)=r(x\cdot dr)-(x\cdot r)dr$. Integrating the derivative of $(x\cdot r)r$ around the closed loop shows $\oint r(x\cdot dr)=-\oint(x\cdot r)dr$. Consequently

$$
\boxed{A(x)=-\frac{\mu_0I}{4\pi R^3}\oint\frac12x\times(r\times dr)+O(R^{-3}).}
$$

Equivalently, $A=\mu_0m\times x/(4\pi R^3)+O(R^{-3})$, where $m=(I/2)\oint r\times dr$ is the [magnetic dipole moment](../../../../../magnetic-dipole-moment.md). The leading displayed potential is of order $R^{-2}$; the remainder is smaller by a factor $R^{-1}$.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
