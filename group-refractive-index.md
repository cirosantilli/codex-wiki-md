# Group refractive index

↑ **Parent:** [Optical path length](optical-path-length.md)

The [group refractive index](group-refractive-index.md) is $n_g=c/v_g$ for a transparent [isotropic](isotropy.md) propagation branch with forward [group velocity](group-velocity.md) $v_g=d\omega/dk>0$. Differentiating the local [wavenumber](wavenumber.md) $k=n(\omega)\omega/c$ gives

$$
n_g=n+\omega\frac{\partial n}{\partial\omega}=n-\lambda_0\frac{\partial n}{\partial\lambda_0},\qquad
\tau_g=\frac{\partial\phi_{\mathrm{prop}}}{\partial\omega}=\frac1c\int_\gamma n_g(\mathbf r,\omega)\,ds.
$$

The last formula gives the propagation [group delay](group-delay.md) along a path whose geometry is fixed as [frequency](frequency.md) varies; additional apparatus [wave phases](phase-waves.md) require their own [frequency](frequency.md) derivatives. For a narrow [wave packet](wave-packet.md) with little loss and negligible reshaping, it approximates the transit of its [wave envelope](envelope-waves.md). In the nondispersive case $\partial_\omega n=0$, it reduces to $\operatorname{OPL}/c$. An [optical path length](optical-path-length.md) at one [frequency](frequency.md) contains no information about $\partial_\omega n$, so in a medium with [optical dispersion](dispersion-optics.md) it cannot by itself determine the [group delay](group-delay.md). [Group Index](rp-photonics-encyclopedia-by-rudiger-paschotta/group-index.md)

For an original local model near $\omega_*$, choose two equal geometric paths of length $L$, with $n_A(\omega)=3/2$ and $n_B(\omega)=3/2+(\omega-\omega_*)/(10\omega_*)$. At $\omega_*$ both [optical path lengths](optical-path-length.md) equal $3L/2$, and matched launch and interface references give equal carrier [wave phases](phase-waves.md). But $n_{g,A}=3/2$ and $n_{g,B}=8/5$, so their [group delays](group-delay.md) differ by $L/(10c)$. This local stipulated model is a counterexample to identifying equal [wave phase](phase-waves.md) with equal pulse arrival; it asserts no material response outside the narrow band considered. Strong loss or pulse reshaping requires a fuller propagation model, and [group delay](group-delay.md) need not time the earliest causal response.

**Table of contents**

- [Group delay](group-delay.md)

## ↑ Ancestors (7)

1. [Optical path length](optical-path-length.md)
2. [Wavefront](wavefront.md)
3. [Physical optics](physical-optics.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Group refractive index](group-refractive-index.md)
