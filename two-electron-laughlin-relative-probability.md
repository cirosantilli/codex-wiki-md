# Two-electron Laughlin relative probability

↑ **Parent:** [Laughlin wavefunction](laughlin-wavefunction.md)

Consider the original two-[electron](electron.md) example obtained by taking $N=2$ in the [Laughlin wavefunction](laughlin-wavefunction.md), with no additional [polynomial](polynomial-split.md) for the [centre of mass](center-of-mass.md). Introduce $Z=(z_1+z_2)/2$, relative [complex coordinate](complex-coordinate.md) $w=z_1-z_2$, separation $r=|w|$, and dimensionless separation $u=r/\ell_B$. Since $|z_1|^2+|z_2|^2=2|Z|^2+|w|^2/2$, the [probability density](probability-density.md) factorizes:

$$
|\Psi_m|^2\propto e^{-|Z|^2/\ell_B^2}\,r^{2m}e^{-r^2/(4\ell_B^2)}.
$$

Integrating out $Z$ leaves an isotropic relative [probability density](probability-density.md). Define $D_m(u)$ per unit dimensionless [area](surface-area.md) and $p_m(u)$ per unit dimensionless separation:

$$
D_m(u)=\frac{u^{2m}e^{-u^2/4}}{\pi4^{m+1}m!},
\qquad p_m(u)=2\pi uD_m(u),
\qquad \int_0^\infty p_m(u)\,du=1.
$$

The physical areal [probability density](probability-density.md) is $D_m(r/\ell_B)/\ell_B^2$. The probability of a separation between $r$ and $r+dr$ is $p_m(r/\ell_B)\,dr/\ell_B$. The extra $u$ comes from the [Jacobian determinant](jacobian-determinant.md) in [polar coordinates](polar-coordinates.md): a thin annulus has [area](surface-area.md) $2\pi r\,dr$. Omitting that factor changes the question being answered.

<a id="image-pair-avoidance-and-the-annular-jacobian-determinant-in-a-two-electron-laughlin-wavefunction"></a>
![](laughlin-two-electron-separation.png)

**[Figure 11](#image-pair-avoidance-and-the-annular-jacobian-determinant-in-a-two-electron-laughlin-wavefunction). Pair avoidance and the annular Jacobian determinant in a two-electron Laughlin wavefunction**. Original normalized model curves for chosen odd exponents $m=1$ and $m=3$. Left: relative [probability density](probability-density.md) per unit dimensionless [area](surface-area.md). Right: [probability density](probability-density.md) of dimensionless separation, including the annular factor $2\pi u$. Markers identify the respective maxima. These finite two-particle curves are not measured data or the pair distribution of an infinite fluid.

Both [wavefunction normalization](wavefunction-normalization.md) and the peak shift can be checked exactly. The substitution $t=u^2/4$ gives the [Gamma function](gamma-function.md) integral

$$
\int_0^\infty u^{2m+1}e^{-u^2/4}\,du
=2^{2m+1}\int_0^\infty t^me^{-t}\,dt
=2^{2m+1}m!.
$$

For $m>0$, logarithmic differentiation gives

$$
\frac{d}{du}\log D_m=\frac{2m}{u}-\frac u2,
\qquad
\frac{d}{du}\log p_m=\frac{2m+1}{u}-\frac u2.
$$

Consequently the areal maximum lies at $u=2\sqrt m$, while the most probable separation lies farther out, at $u=\sqrt{4m+2}$. For $m=1$ these are $2$ and $\sqrt6\simeq2.449$; for $m=3$, $\sqrt{12}\simeq3.464$ and $\sqrt{14}\simeq3.742$. The same substitution gives $\langle u^2\rangle=4(m+1)$, so the [root mean square](root-mean-square.md) separations are $\sqrt8$ and $4$ respectively. The distinction between a [probability density](probability-density.md) maximum and a radial maximum therefore has a directly calculable geometric origin.

This two-[electron](electron.md) model explains exchange and pair avoidance. It does not establish a nonzero many-particle [spectral gap](spectral-gap.md), an extended [quantum Hall plateau](quantum-hall-plateau.md), or the topological properties of a fluid in the [thermodynamic limit](thermodynamic-limit.md). Those require additional many-[electron](electron.md) reasoning and experimental tests.

## ↑ Ancestors (12)

1. [Laughlin wavefunction](laughlin-wavefunction.md)
2. [Fractional quantum Hall effect](fractional-quantum-hall-effect.md)
3. [Quantum Hall effect](quantum-hall-effect.md)
4. [Hall effect](hall-effect.md)
5. [Lorentz force](lorentz-force.md)
6. [Electromagnetic field tensor](electromagnetic-field-tensor.md)
7. [Electromagnetic four-potential](electromagnetic-four-potential.md)
8. [Relativistic electromagnetism](relativistic-electromagnetism-split.md)
9. [Electromagnetism](electromagnetism-split.md)
10. [Branches of physics](branches-of-physics.md)
11. [Physics](physics-split.md)
12. [Codex Wiki](split.md)
