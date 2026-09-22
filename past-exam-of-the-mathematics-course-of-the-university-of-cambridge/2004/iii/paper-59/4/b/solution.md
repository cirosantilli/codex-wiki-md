<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $T=\overline T(1+\Theta)$, with $\Theta=\Delta T/\overline T$ at linear order. Since $\overline T\propto a^{-1}$, the background [Planck function](../../../../../../planck-function.md) depends only on comoving momentum. Expanding its temperature-shifted argument gives

$$
f_0\left(\frac{\overline Tq}{T}\right)=f_0(q-q\Theta)+O(\Theta^2),
\qquad\boxed{f_1=-qf_0'(q)\Theta.}
$$

Using $T$ rather than $\overline T$ in the perturbation denominator changes only higher-order terms.

The [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md) is the energy-weighted angular perturbation

$$
\Delta=\frac{\int_0^\infty q^3f_1\,dq}{\int_0^\infty q^3f_0\,dq}.
$$

[Integration by parts](../../../../../../integration-by-parts.md) gives $\int q^4f_0'\,dq=-4\int q^3f_0\,dq$; the boundary term vanishes at both endpoints for a Planck spectrum. Therefore $\Delta=4\Theta$. Multiplying the transport equation by $q^3$ and integrating yields the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md)

$$
\boxed{\Delta'+ik\mu\Delta=-2h'_{ij}\widehat n^i\widehat n^j.}
$$

The PDF's definition is $4\Delta T/T$; the TeX's denominator $\hbar$ is a transcription error.

Expand $\Delta$ in Legendre moments in $\mu$. The monopole is the density/temperature perturbation, and the dipole is the bulk velocity. Before decoupling, rapid [Thomson scattering](../../../../../../thomson-scattering.md) isotropizes photons in the electron rest frame. In the [tight-coupling approximation](../../../../../../tight-coupling-approximation.md), the scattering rate is much larger than $k$ and $\mathcal H$, so the quadrupole and higher moments are suppressed by the mean-free-path parameter, with the quadrupole typically of order $k/\dot\kappa$ times the dipole. To leading order only monopole and dipole are needed. This suppression uses the collision term restored before decoupling; it does not follow from the collisionless equation by itself. Finite quadrupole corrections generate polarization and diffusion damping.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
