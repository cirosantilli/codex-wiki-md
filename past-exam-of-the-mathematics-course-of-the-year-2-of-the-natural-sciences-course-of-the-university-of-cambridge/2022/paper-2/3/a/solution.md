<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Dirichlet Green function](../../../../../dirichlet-green-function.md) with the sign convention

$$
\boxed{\Delta_{\mathbf r}G(\mathbf r,\mathbf r')=\delta(\mathbf r-\mathbf r')\text{ in }V,\qquad G(\mathbf r,\mathbf r')=0\text{ on }S.}
$$

The [normal derivative](../../../../../normal-derivative.md) is taken with respect to the integration variable and the outward normal of $V$. [Green's second identity](../../../../../green-second-identity.md) gives

$$
\int_V\left(u\Delta G-G\Delta u\right)dV
=\oint_S\left(u\partial_nG-G\partial_nu\right)dS.
$$

The [Dirac delta distribution](../../../../../dirac-delta-function.md) evaluates the first volume term at $\mathbf r'$. Substituting $\Delta u=\rho$, $u=f$ on $S$ and $G=0$ there yields

$$
u(\mathbf r')-\int_VG(\mathbf r,\mathbf r')\rho(\mathbf r)\,dV
=\oint_Sf(\mathbf r)\partial_nG(\mathbf r,\mathbf r')\,dS.
$$

Hence

$$
\boxed{u(\mathbf r')=\int_V\rho(\mathbf r)G(\mathbf r,\mathbf r')\,dV+\oint_Sf(\mathbf r)\partial_nG(\mathbf r,\mathbf r')\,dS.}
$$

One can justify applying the identity to the singular [Green function](../../../../../green-s-function-split.md) by removing a small sphere around the source and then taking its radius to zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
