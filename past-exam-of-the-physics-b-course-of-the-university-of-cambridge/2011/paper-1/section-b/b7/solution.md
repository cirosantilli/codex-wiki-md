<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

The microscopic magnetic response becomes a macroscopic field problem through the [magnetization](../../../../../magnetization.md) $\mathbf M$, the [magnetic dipole moment](../../../../../magnetic-dipole-moment.md) per unit [volume](../../../../../volume.md). Define

$$
\mathbf B=\mu_0(\mathbf H+\mathbf M),\qquad
\nabla\cdot\mathbf B=0,\qquad \nabla\times\mathbf H=\mathbf J_{\rm free}
$$

in magnetostatics. Bound currents are represented by $\mathbf J_b=\nabla\times\mathbf M$ and surface current $\mathbf K_b=\mathbf M\times\hat{\mathbf n}$. Normal $B$ is continuous across an interface, while $\hat{\mathbf n}\times(\mathbf H_2-\mathbf H_1)=\mathbf K_{\rm free}$. It is generally incorrect to impose continuity of every component of both fields. A linear isotropic material has $\mathbf M=\chi\mathbf H$ and $\mu_r=1+\chi$, but a ferromagnet usually requires a nonlinear, history-dependent constitutive relation.

Internal field differs from externally applied field. For uniform [magnetization](../../../../../magnetization.md) along a [principal axis](../../../../../principal-axis.md) of an ellipsoid, the [demagnetizing field](../../../../../demagnetizing-field.md) is $-N_dM$ and $H_{\rm int}=H_{\rm applied}-N_dM$. A linear specimen therefore has apparent susceptibility $\chi/(1+N_d\chi)$ relative to the applied field. Shape is especially important for large susceptibility. A long closed [magnetic circuit](../../../../../magnetic-circuit.md) reduces stray fields; a bar magnet still has [demagnetizing fields](../../../../../demagnetizing-field.md) despite the absence of magnetic monopoles. Equivalent magnetic-pole descriptions are bookkeeping for [magnetization](../../../../../magnetization.md) [divergence](../../../../../divergence.md), not free magnetic charge.[Equations (699)–(706): magnetization, scalar potential and effective pole density](../../../../../classical-electromagnetism-by-richard-fitzpatrick/permanent-ferromagnets.md)

In [paramagnetism](../../../../../paramagnetism.md), permanent localized moments are preferentially aligned by the field, against thermal disorder. For independent spin-one-half moments with projections $\pm\mu$, the two [Zeeman energies](../../../../../zeeman-energy.md) give

$$
Z_1=2\cosh\left(\frac{\mu B}{k_BT}\right),\qquad
M=n\mu\tanh\left(\frac{\mu B}{k_BT}\right),\qquad
\chi\simeq\frac{\mu_0n\mu^2}{k_BT}>0
$$

in the dilute weak-field limit with $B\simeq\mu_0H$. This is a [Curie law](../../../../../curie-s-law.md); the response saturates at $n\mu$ when alignment dominates. More generally, [spin](../../../../../spin.md) $J$ gives $\chi=\mu_0n(g\mu_B)^2J(J+1)/(3k_BT)$. Interactions can produce a Curie–Weiss response $C/(T-\Theta)$ over a suitable range. Conduction-electron [Pauli paramagnetism](../../../../../pauli-paramagnetism.md) need not show the localized-moment $1/T$ law.

In [diamagnetism](../../../../../diamagnetism.md), the field induces a [magnetic moment](../../../../../magnetic-dipole-moment.md) opposing it, so the linear susceptibility is negative. The microscopic cause is the change in orbital electronic motion, and a closed-shell insulating material has no permanent atomic moment to orient. This weak response is often only mildly [temperature](../../../../../temperature-split.md) dependent away from other transitions. It also exists as a background in materials with a stronger positive response. Perfect flux expulsion in a superconductor is a distinct collective phenomenon and should not be identified with ordinary weak atomic [diamagnetism](../../../../../diamagnetism.md).

In [ferromagnetism](../../../../../ferromagnetism.md), [exchange interactions](../../../../../exchange-interaction.md) stabilize spontaneous magnetic order below the [Curie temperature](../../../../../curie-temperature.md). A specimen can have zero net moment while its [magnetic domains](../../../../../magnetic-domain.md) remain locally magnetized in different directions. Domain-wall motion and moment rotation produce a large response; anisotropy and pinning lead to [remanence](../../../../../remanent-magnetization.md), coercivity and [hysteresis](../../../../../hysteresis.md). Increasing field eventually approaches saturation. Heating above the ordering transition removes spontaneous order, although an applied field still induces a response. Soft magnetic cores favor easy reversal and small cyclic loss; hard permanent-magnet materials favor retained [magnetization](../../../../../magnetization.md) and resistance to reversal. These properties concern collective order and barriers, not merely independent moments all following a weak field.[§12.7, Magnetism in Matter: susceptibility, magnetic domains, Curie temperature and hysteresis](../../../../../university-physics-volume-2-by-samuel-j-ling-and-others.md)

A practical distinction requires a controlled field sweep and a separate magnetic readout. A toroidal core with drive winding $N_1$, path [length](../../../../../length.md) $l$ and current $I$ has approximately $H=N_1I/l$. A pickup winding measures $\mathcal E_2=-N_2A\,dB/dt$; integrating after calibration gives $B$, and $M=B/\mu_0-H$. Reversing the sweep reveals a loop whose positive loss [area](../../../../../surface-area.md) per [volume](../../../../../volume.md) is $\oint H\,dB$. An air-core/empty-holder reference, known geometry and turn count, offset correction, [temperature](../../../../../temperature-split.md) control and slower sweeps test background, heating and rate-dependent eddy-current losses. A single [force](../../../../../force-split.md) or susceptibility reading cannot establish spontaneous order or [hysteresis](../../../../../hysteresis.md). The original curves below are illustrative responses, not measured material data.

<a id="section-b/b7/image-magnetic-response-and-hysteresis"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1-magnetic-response.png)

**[Figure 2](#section-b/b7/image-magnetic-response-and-hysteresis). Magnetic response and hysteresis**.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
