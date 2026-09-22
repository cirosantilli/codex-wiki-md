<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Particles settle toward the bed under their submerged weight. A concentration increasing downward gives an upward turbulent diffusive flux, which can oppose that settling. If [turbulence](../../../../../../turbulence-split.md) cannot sustain the particles, they enter the weakly mixed near-wall region and can deposit. [Sediment resuspension](../../../../../../sediment-resuspension.md) requires bed forces strong enough to entrain grains, not merely a specified diffusivity far above the bed.

For noncohesive grains, an appropriate criterion uses the [Shields parameter](../../../../../../shields-parameter.md)

$$
\boxed{\Theta=\frac{\tau_d}{(\rho_s-\rho)gd}>\Theta_c,}
$$

where $d$ is grain size, $\rho_s$ its [density](../../../../../../density.md) and $\Theta_c$ the [sediment entrainment threshold](../../../../../../sediment-entrainment-threshold.md) expressed dimensionlessly. The threshold depends on grain geometry, contacts and viscous effects; cohesion changes the criterion. Sustained suspension additionally requires sufficiently vigorous upward turbulent motions relative to $W_s$. Bed motion and well-mixed suspension are therefore not identical conditions.

At sedimentation-resuspension equilibrium, the total vertical particle flux is constant. Set $\kappa_T=Kz$ with $K=C/2$. The stationary equation gives

$$
J=-W_s\phi-Kz\phi_z=\text{constant},
\qquad \phi(z)=A z^{-W_s/K}-\frac{J}{W_s}.
$$

Since $W_s>0$ and $\phi\to0$ at infinity, necessarily $J=0$. Settling and upward diffusion then balance pointwise. Taking a reference height $z_1=1$ in the specified length units gives the [equilibrium settling-diffusion profile](../../../../../../equilibrium-settling-diffusion-profile.md)

$$
\boxed{\phi(z)=\phi_1\left(\frac z{z_1}\right)^{-P},\qquad
P=\frac{W_s}{K}=\frac{2W_s}{\alpha\hat u},\qquad z_1=1.}
$$

It is nonnegative and decays to zero. The profile describes the region $z\gg\delta$; it does not assert that this [power law](../../../../../../power-law.md) continues through the viscous layer down to the physical bed. The supplied reference concentration summarizes the bed exchange and near-wall physics that the outer diffusion closure does not resolve.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
