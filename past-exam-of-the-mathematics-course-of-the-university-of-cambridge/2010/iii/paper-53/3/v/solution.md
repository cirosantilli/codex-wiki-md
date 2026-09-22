<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Work in [conformal Newtonian gauge](../../../../../../newtonian-gauge.md), where $\mathcal R=-\phi+\mathcal Hv$. Set

$$
A=4\pi Ga^2(\bar\rho+\bar P)=\mathcal H^2-\mathcal H',
\qquad c_a^2=\frac{\bar P'}{\bar\rho'}.
$$

The momentum equation gives $v=-(\phi'+\mathcal H\phi)/A$, hence

$$
\mathcal R=-\phi-\frac{\mathcal H}{A}(\phi'+\mathcal H\phi).
$$

This assumes nonzero background enthalpy, as required for the matter comoving slicing. Background energy conservation gives $\bar\rho'=-3\mathcal H(\bar\rho+\bar P)$ and thus

$$
\frac{A'}A=2\mathcal H+\frac{\bar\rho'+\bar P'}{\bar\rho+\bar P}
=-\mathcal H(1+3c_a^2).
$$

The density constraint gives $4\pi Ga^2\delta\rho=\nabla^2\phi-3\mathcal H(\phi'+\mathcal H\phi)$. Insert this into the pressure equation to obtain

$$
\phi''+3\mathcal H(1+c_a^2)\phi'
+\bigl[2\mathcal H'+(1+3c_a^2)\mathcal H^2\bigr]\phi
=c_a^2\nabla^2\phi.
$$

Differentiating the expression for $\mathcal R$, using the formula for $A'/A$ and then $A=\mathcal H^2-\mathcal H'$, groups the terms as

$$
-A\mathcal R'=\mathcal H\left\{
\phi''+3\mathcal H(1+c_a^2)\phi'
+\bigl[2\mathcal H'+(1+3c_a^2)\mathcal H^2\bigr]\phi
\right\}.
$$

The preceding equation proves the [gradient evolution identity for comoving curvature](../../../../../../gradient-evolution-identity-for-comoving-curvature.md):

$$
\boxed{-4\pi Ga^2(\bar\rho+\bar P)\mathcal R'
=\mathcal H\,\frac{\bar P'}{\bar\rho'}\,\nabla^2\phi}.
$$

For a Fourier mode, $\nabla^2\phi=-k^2\phi$. On [super-Hubble scales](../../../../../../superhorizon-scale.md), $k/\mathcal H\ll1$, its evolution is gradient-suppressed. With the stated regular adiabatic relation between $\mathcal R$ and $\phi$, **$\mathcal R$ is constant at leading long-wavelength order**. At finite wavelength there are corrections; the conclusion is not an exact claim that the Laplacian vanishes.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
