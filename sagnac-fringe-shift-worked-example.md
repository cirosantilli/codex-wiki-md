# Sagnac fringe shift worked example

↑ **Parent:** [Sagnac area law](sagnac-area-law.md)

For a stationary rotating apparatus driven by a source with [optical coherence](optical-coherence.md) and proper [frequency](frequency.md) $\nu_0$, define $\lambda_0=c/\nu_0$. The source [wave phase](phase-waves.md) advances by $2\pi\nu_0\Delta\tau$ between the emission times of the two contributions that meet at one readout [spacetime event](event-relativity.md). Define the signed phase lag $\Delta\phi$ of the $+$ contribution and the corresponding displacement $N$ in units of one [interference fringe](interference-fringe.md) by

$$
\Delta\phi=2\pi\nu_0\Delta\tau,\qquad
N=\frac{\Delta\phi}{2\pi}\simeq\frac{4\boldsymbol\Omega\cdot\mathbf A}{c\lambda_0}.
$$

The sign of a photographed spatial displacement also depends on the imposed fringe orientation; this definition fixes the theoretical sign through the delayed beam. In an equal-amplitude output, a representative [light intensity](light-intensity.md) is $I(x)=I_{\max}[1+\cos(Kx-\Delta\phi)]/2$, where $K$ sets the chosen spatial [interference fringe spacing](interference-fringe-spacing.md) $2\pi/K$. Moving $\Delta\phi$ by $2\pi$ shifts the pattern by one fringe. A fixed output exactly at a bright or dark fringe has zero first-order intensity slope, so a known phase bias or a spatial fringe readout is useful for determining a small signed delay.

Choose a square of side $0.30\,\mathrm m$, a rectangle $0.40\,\mathrm m$ by $0.20\,\mathrm m$, $\lambda_0=633\,\mathrm{nm}$ and $\Omega=+10\,\mathrm{rad\,s^{-1}}$, with [angular velocity](angular-velocity.md) parallel to the positive [normal vectors](normal-vector.md). Both perimeters are $1.20\,\mathrm m$, but the [areas](surface-area.md) are $0.090\,\mathrm{m^2}$ and $0.080\,\mathrm{m^2}$. Using $c=299792458\,\mathrm{m\,s^{-1}}$, the leading predictions are

$$
\begin{aligned}
\Delta t_{\rm square}&\simeq4.006\times10^{-17}\,\mathrm s,&N_{\rm square}&\simeq0.0189705,\\
\Delta t_{\rm rectangle}&\simeq3.560\times10^{-17}\,\mathrm s,&N_{\rm rectangle}&\simeq0.0168626.
\end{aligned}
$$

These are original model choices and predictions, not measured points. The square has $9/8$ times the response despite the equal path lengths. Reversing from $+\Omega$ to $-\Omega$ gives $N(-\Omega)-N(+\Omega)=-2N(+\Omega)$: the displacement magnitude between opposite rotations is twice the displacement magnitude from rest. Confusing these two comparisons introduces a factor-of-two error.

<a id="image-sagnac-area-law-fringe-model"></a>
![](sagnac-area-law-fringe-model.png)

**[Figure 11](#image-sagnac-area-law-fringe-model). Independent path-segment calculation of the predicted fringe displacement for two equal-perimeter loops**. The generator sums $(\boldsymbol\Omega\times\mathbf r)\cdot d\mathbf r$ along each straight segment, rather than inserting the enclosed [area](surface-area.md) into the answer. Both loops are oriented counterclockwise. Lines and marked values are leading-order vacuum model predictions; no historical measurements are plotted.

## ↑ Ancestors (6)

1. [Sagnac area law](sagnac-area-law.md)
2. [Sagnac effect](sagnac-effect.md)
3. [Special relativity](special-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
