<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For unforced [incompressible flow](../../../../../../incompressible-flow.md), multiply the [vorticity equation](../../../../../../vorticity-equation.md) by $\omega_i$. The antisymmetric part of the [velocity gradient tensor](../../../../../../velocity-gradient-tensor.md) drops out of $\omega_i\omega_j\partial_j u_i$, leaving

$$
\frac{D}{Dt}\frac{\omega^2}{2}=\omega_i\omega_jS_{ij}+\nu\omega_i\nabla^2\omega_i.
$$

[Statistical homogeneity](../../../../../../statistical-homogeneity.md) removes mean divergences. [Integration by parts](../../../../../../integration-by-parts.md), together with $\nabla\cdot\boldsymbol\omega=0$, gives

$$
\boxed{\frac{d}{dt}\frac{\langle\omega^2\rangle}{2}
=\langle\omega_i\omega_jS_{ij}\rangle-\nu\langle|\nabla\boldsymbol\omega|^2\rangle
=\langle\omega_i\omega_jS_{ij}\rangle-\nu\langle|\nabla\times\boldsymbol\omega|^2\rangle}.
$$

The last equality holds for the averages, not pointwise. It follows from the usual [curl](../../../../../../curl.md)/divergence identity after the divergence terms have averaged to zero. [Vortex stretching](../../../../../../vortex-stretching.md) produces [enstrophy](../../../../../../enstrophy.md), while viscous diffusion destroys it.

Let $T=\ell/u$, $\epsilon\sim u^3/\ell$, and use the [Kolmogorov microscales](../../../../../../kolmogorov-microscales.md) $\eta=(\nu^3/\epsilon)^{1/4}$ and $\tau_\eta=(\nu/\epsilon)^{1/2}$. Since $\langle\omega^2\rangle=\epsilon/\nu$, a slowly changing mean [enstrophy](../../../../../../enstrophy.md) has a time derivative of order $\epsilon/(\nu T)$. The usual small-scale estimate gives

$$
\nu\langle|\nabla\times\boldsymbol\omega|^2\rangle
\sim\frac{\epsilon}{\eta^2}
=\left(\frac{\epsilon}{\nu}\right)^{3/2}.
$$

The relative imbalance is consequently $\tau_\eta/T\sim(\nu/u\ell)^{1/2}=\mathrm{Re}^{-1/2}$, yielding

$$
\boxed{\langle\omega_i\omega_jS_{ij}\rangle
=\nu\langle|\nabla\times\boldsymbol\omega|^2\rangle[1+O(\mathrm{Re}^{-1/2})]}.
$$

The estimate assumes an established high-Reynolds-number cascade and integral-time evolution of the mean, not a rapid initial transient. In a forced flow the exact balance includes $\langle\boldsymbol\omega\cdot\nabla\times\mathbf f\rangle$; forcing smooth on the [integral scale of turbulence](../../../../../../integral-scale-of-turbulence.md) is smaller than the leading small-scale terms.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
