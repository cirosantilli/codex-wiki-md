<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $x^\mu=(t,x)$ and [Minkowski metric](../../../../minkowski-metric.md) $\eta^{\mu\nu}=\operatorname{diag}(1,-1)$, with the wave speed equal to one. Regarding $\phi$ as a [scalar field](../../../../scalar-field.md), the symmetric [canonical stress-energy tensor](../../../../canonical-stress-energy-tensor.md) is

$$
T^{\mu\nu}=\partial^\mu\phi\,\partial^\nu\phi-\eta^{\mu\nu}\mathcal L
=\begin{pmatrix}\mathcal E&p\\p&\mathcal E\end{pmatrix},\qquad
\mathcal E=\frac12(\phi_t^2+\phi_x^2),\quad p=-\phi_t\phi_x.
$$

It obeys $\partial_\mu T^{\mu\nu}=0$ on the [wave equation](../../../../wave-equation-split.md). For a [scalar field](../../../../scalar-field.md) the intrinsic spin current vanishes. The total orbital [Lorentz current](../../../../lorentz-current.md) and its integrated angular-momentum tensor are

$$
\boxed{\mathcal J^{\lambda\mu\nu}=x^\mu T^{\lambda\nu}-x^\nu T^{\lambda\mu},\qquad
J^{\mu\nu}(t)=\int_{\mathbb R}\mathcal J^{0\mu\nu}\,dx.}
$$

Because there is only one spatial dimension, its only independent possibly nonzero component is

$$
\boxed{J^{01}=\int_{\mathbb R}(t p-x\mathcal E)\,dx=tP-\int_{\mathbb R}x\mathcal E\,dx,\qquad J^{10}=-J^{01},}
$$

where $P=\int p\,dx$. The corresponding flux is $\mathcal J^{101}=t\mathcal E-xp$. Symmetry and conservation of $T$ give

$$
\partial_\lambda\mathcal J^{\lambda\mu\nu}=T^{\mu\nu}-T^{\nu\mu}=0.
$$

Thus $J^{01}$ is conserved provided the boundary flux vanishes and the integrals exist. For example, localized wave packets on an infinite line have this property. One can also check directly that $d\int x\mathcal E\,dx/dt=P$, so the two terms in $J^{01}$ have cancelling derivatives.

The significance is the [boost charge of a one-dimensional scalar field](../../../../boost-charge-of-a-one-dimensional-scalar-field.md). There is no independent spatial rotation or ordinary spatial angular-momentum component in one dimension. Instead, the action has the mathematical [Lorentz invariance](../../../../lorentz-invariance.md) of a massless wave field with invariant speed $c_s=1$, and $J^{01}$ generates its boost. Its conservation says that the center of energy moves uniformly. This is a symmetry of the ideal wave-field model, rather than an assertion of fundamental vacuum Lorentz symmetry for a material rod. Fixed boundaries can break it, and a general solution with nonvanishing boundary flux need not conserve the integrated charge.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
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
