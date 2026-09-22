# Barkhausen pulse area

↑ **Parent:** [Barkhausen effect](barkhausen-effect.md)

Write the [magnetic flux linkage](magnetic-flux-linkage.md) of the stationary [pickup coil](pickup-coil.md) as $\lambda=\sum_{n=1}^N\Phi_n$, in [SI](international-system-of-units.md) units of [weber](weber-unit.md). If every turn links the same [magnetic flux](magnetic-flux.md) $\Phi$, then $\lambda=N\Phi$; the turn count is dimensionless. With a fixed winding and terminal convention, [Faraday's law of induction](faraday-s-law-of-induction.md) gives the induced [electromotive force](electromotive-force.md)

$$
e(t)=-\frac{d\lambda}{dt},\qquad
\int_{t_a}^{t_b}e(t)\,dt=-[\lambda(t_b)-\lambda(t_a)].
$$

This is the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) applied to [magnetic flux linkage](magnetic-flux-linkage.md). Its units are $\mathrm{V\,s}=\mathrm{Wb}$, not [volts](volt.md) alone. Reversing the leads reverses the sign. In a high-input-[electrical resistance](electrical-resistance.md) voltage measurement the input approximately follows this [electromotive force](electromotive-force.md); coil loading and the [frequency response](frequency-response.md) of the electronics require separate calibration.

Separate direct drive linkage from material linkage: $\lambda=\lambda_{\rm drive}+\lambda_{\rm material}$. Even an empty [pickup coil](pickup-coil.md) has $-d\lambda_{\rm drive}/dt$. In an ideal long, uniformly coupled specimen with negligible [demagnetizing field](demagnetizing-field.md) correction and [eddy current](eddy-current.md) shielding, a useful material approximation is

$$
\lambda_{\rm material}=\mu_0 N A_s M,\qquad
\int e_{\rm material}\,dt=-\mu_0 N A_s\Delta M.
$$

Here $A_s$ is specimen cross-sectional [area](surface-area.md), not the larger coil aperture; $\mu_0$ is [vacuum permeability](vacuum-permeability.md) and $M$ the axial [magnetization](magnetization.md) sampled by the coil. The units check directly: $(\mathrm{V\,s/(A\,m)})(\mathrm{m^2})(\mathrm{A/m})=\mathrm{V\,s}$. Finite geometry and nonuniform [magnetization](magnetization.md) generally require a calibrated coupling in place of $\mu_0NA_s$. The exact linkage identity survives that failure of the uniform approximation.

As an original illustrative calculation, stipulate $N=100$, $A_s=10^{-6}\,\mathrm{m^2}$, $\Delta M=10^3\,\mathrm{A/m}$ and rounded $\mu_0=4\pi\times10^{-7}\,\mathrm{V\,s/(A\,m)}$. Then

$$
\Delta\lambda=4\pi\times10^{-8}\,\mathrm{Wb}
\approx0.125664\,\mu\mathrm{Wb},\qquad
\int e_{\rm material}\,dt\approx-0.125664\,\mathrm{mV\,ms}.
$$

A uniform change over $0.10\,\mathrm{ms}$ would give a rectangular pulse of $-1.25664\,\mathrm{mV}$; over $0.20\,\mathrm{ms}$ it gives $-0.628319\,\mathrm{mV}$ with the same area. Thus pulse height mixes change size with change speed. These numbers describe an ideal model, not observed pulses or material constants.

## ↑ Ancestors (8)

1. [Barkhausen effect](barkhausen-effect.md)
2. [Ferromagnetism](ferromagnetism.md)
3. [Magnetization](magnetization.md)
4. [Bound charge and bound current](bound-charge-and-bound-current.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Magnetization](magnetization.md)
