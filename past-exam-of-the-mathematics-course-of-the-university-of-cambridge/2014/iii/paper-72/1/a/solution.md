<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the time dependence $e^{-i\omega t}$ and measure distances in background-wavenumber units. Thus $L_0=\Delta+1$, the [incident field](../../../../../../incident-wave.md) satisfies $L_0\psi_i=0$, and the [scattering potential](../../../../../../scattering-potential.md) convention is $V=n^2-1$, giving $L_0\psi=-V\psi$. To match the minus sign in the paper's integral, take the outgoing [Green function](../../../../../../green-s-function.md) to satisfy $L_0G=\delta$. This is the negative of the frequently used outgoing [Helmholtz equation](../../../../../../helmholtz-equation.md) fundamental solution satisfying $L_0G=-\delta$. In physical coordinates one restores $k_0^2$ in the [scattering potential](../../../../../../scattering-potential.md), or absorbs it in the integral kernel; the sign convention must remain consistent.

On a region where the incident and total fields are nonzero, introduce the [logarithmic wave perturbation](../../../../../../logarithmic-wave-perturbation.md)

$$
\psi=\psi_i e^\chi,\qquad \chi=\log(\psi/\psi_i).
$$

Choose a continuous logarithm branch connected to the unperturbed field. Substitution into the [Helmholtz equation](../../../../../../helmholtz-equation.md) gives

$$
\mathcal L_i\chi+\nabla\chi\cdot\nabla\chi=-V,\qquad \mathcal L_i=\Delta+2\frac{\nabla\psi_i}{\psi_i}\cdot\nabla.
$$

The quadratic term uses the complex bilinear dot product, not the squared modulus of the gradient. Write $V=\varepsilon V_1$ and $\chi=\varepsilon\chi^{[1]}+\cdots$. The first-order [Rytov approximation](../../../../../../rytov-approximation.md) discards that quadratic term. Since $L_0(\psi_i\chi)=\psi_i\mathcal L_i\chi$, the outgoing first correction is

$$
\chi_1(\mathbf r)=-\frac1{\psi_i(\mathbf r)}\int G(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r',
$$

and hence

$$
\boxed{\psi_1^{(R)}(\mathbf r)=\psi_i(\mathbf r)\exp\left[-\frac1{\psi_i(\mathbf r)}\int G(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r'\right].}
$$

The [validity of the first Rytov approximation](../../../../../../validity-of-the-first-rytov-approximation.md) concerns the omitted logarithmic correction. Its next contribution satisfies $\mathcal L_i\chi_2=-\nabla\chi_1\cdot\nabla\chi_1$, so a useful explicit criterion is that the outgoing solution $\chi_2$ be small in the region of interest. Weak [refractive index](../../../../../../refractive-index.md) contrast and small [wave phase](../../../../../../phase-waves.md) gradients on a wavelength scale provide the usual perturbative regime, with weak [amplitude](../../../../../../wave-amplitude.md) fluctuations and no strong focusing or zeros that destroy the logarithm. A sufficient local source comparison is $|\nabla\chi_1\cdot\nabla\chi_1|\ll|V|$ where the [scattering potential](../../../../../../scattering-potential.md) is nonzero, together with control of propagation of that error. This is not a universal pointwise test at zeros of $V$.

**Small accumulated [wave phase](../../../../../../phase-waves.md) is not required in the same way as in a linear field approximation**: the exponential retains that [wave phase](../../../../../../phase-waves.md) accumulation. Large gradients, strong multiple-scattering [amplitude](../../../../../../wave-amplitude.md) effects or field zeros can still invalidate the [Rytov approximation](../../../../../../rytov-approximation.md). The integrals also require a finite scattering region or appropriate convergence conditions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
