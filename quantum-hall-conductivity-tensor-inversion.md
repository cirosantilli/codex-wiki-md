# Quantum Hall conductivity tensor inversion

↑ **Parent:** [Integer quantum Hall effect](integer-quantum-hall-effect.md)

Choose conventional [surface current density](surface-current-density.md) along $+x$, [magnetic field](magnetic-field-split.md) along $+z$, and negative [electron](electron.md) charge. An isotropic in-plane response has the following [sheet conductivity](surface-conductivity.md) and [sheet resistivity](sheet-resistivity.md) [tensors](tensor.md) for $s\geq0$, $k>0$:

$$
\mathbf K=\frac{e^2}{h}\begin{pmatrix}s&-k\\k&s\end{pmatrix}\mathbf E,
\qquad
\mathbf E=R_K\frac1{s^2+k^2}\begin{pmatrix}s&k\\-k&s\end{pmatrix}\mathbf K.
$$

These are [matrix inverses](matrix-inverse-split.md), rather than componentwise reciprocals. The [sheet conductivity](surface-conductivity.md) has units [siemens](siemens-unit.md), the [sheet resistivity](sheet-resistivity.md) [ohms](ohm.md). With $K_y=0$, the sign is $E_y/K_x<0$, agreeing with the negative [Hall coefficient](hall-coefficient.md) of a single [electron](electron.md) species. Contact polarity can reverse the measured voltage sign, so quote the Hall magnitude. For a homogeneous strip of width $W$ and longitudinal probe separation $L$, $I=WK_x$ gives

$$
\boxed{\frac{|V_H|}{I}=R_K\frac{k}{s^2+k^2},\qquad
\frac{V_{xx}}{I}=R_K\frac{L}{W}\frac{s}{s^2+k^2}.}
$$

At $s=0$, $k=N$, these reduce to $R_K/N$ and zero. A nonzero transverse [sheet resistivity](sheet-resistivity.md) creates no local [Joule heating](joule-heating.md): the antisymmetric contribution cancels in $\mathbf E\cdot\mathbf K=(e^2/h)s|\mathbf E|^2$.

For an original nonideal example, choose $k=2$, $s=0.01$ and $L/W=2$. Then $V_{xx}/I\simeq129.061\,\Omega$, while the Hall magnitude is below $R_K/2$ by the relative amount $s^2/(k^2+s^2)\simeq25.0$ parts per million. An unwanted admixture $0.02V_{xx}$ in the Hall readout would instead introduce approximately $2.58\,\Omega$. The chosen calculation shows why a small intrinsic tensor correction does not by itself guarantee an accurate contact measurement.

## ↑ Ancestors (11)

1. [Integer quantum Hall effect](integer-quantum-hall-effect.md)
2. [Quantum Hall effect](quantum-hall-effect.md)
3. [Hall effect](hall-effect.md)
4. [Lorentz force](lorentz-force.md)
5. [Electromagnetic field tensor](electromagnetic-field-tensor.md)
6. [Electromagnetic four-potential](electromagnetic-four-potential.md)
7. [Relativistic electromagnetism](relativistic-electromagnetism-split.md)
8. [Electromagnetism](electromagnetism-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Fractional quantum Hall effect](fractional-quantum-hall-effect.md)
- [Integer quantum Hall effect](integer-quantum-hall-effect.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-b/b4/d/solution.md)
- [Quantum Hall plateau](quantum-hall-plateau.md)
- [Tsui-Störmer-Gossard fractional Hall experiment](tsui-stormer-gossard-fractional-hall-experiment.md)
