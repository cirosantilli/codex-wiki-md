# Attosecond streaking

↑ **Parent:** [Attosecond physics](attosecond-physics.md)

[Attosecond streaking](attosecond-streaking.md) uses a synchronized reference [electric field](electric-field-split.md) to change a [photoelectron](photoelectron.md)'s outgoing [momentum](momentum-split.md). Scanning relative delay produces an [energy](energy-split.md)-versus-delay distribution. A short emission interval samples only a small part of the reference cycle; a longer interval samples a range of kicks and can broaden or reshape the distribution.

For an explicit classical limit, use the [electric dipole](electric-dipole.md) approximation and choose the [magnetic vector potential](magnetic-vector-potential.md) $A(t)$ along the detection axis with $E(t)=-dA/dt$ and $A(\infty)=0$. Neglect the residual [ion](ion.md)'s [Coulomb force](coulomb-force.md). An [electron](electron.md) released at $t_i$ with mechanical [momentum](momentum-split.md) $p_0$ obeys

$$
p_f=p_0-eA(t_i),\qquad
K_f=\frac{[p_0-eA(t_i)]^2}{2m}.
$$

Indeed, integrating $\dot p=-eE=e\dot A$ from release to the end of the field gives the stated minus sign. The useful clock variable here is $A$, rather than the instantaneous $E$ itself. If $A$ is nearly linear across a narrow emission window with temporal [standard deviation](standard-deviation.md) $\sigma_t$, and initial [momentum](momentum-split.md) is sharp, then

$$
\sigma_p\simeq e|E(t_i)|\sigma_t.
$$

This local mapping fails near a zero of $E$, where first-order timing sensitivity vanishes. A real inversion must include the incident bandwidth, initial [photoelectron](photoelectron.md) distribution, collection angles and target–field response.

For an original dimensionless example in [atomic units](atomic-units.md), choose $p_0=2$, $m=e=1$ and $A(t_i)=0.10$. Then $p_f=1.9$ and $K_f=1.805$, compared with initial [kinetic energy](kinetic-energy.md) $2$. Reversing $A$ gives $K_f=2.205$: the shifts are asymmetric because of the $A^2/2$ term. A measurement that keeps only the term linear in $A$ would miss $0.005$ in both cases.

**Table of contents**

- [2001 isolated attosecond pulse experiment](2001-isolated-attosecond-pulse-experiment.md)

## ↑ Ancestors (6)

1. [Attosecond physics](attosecond-physics.md)
2. [Laser](laser-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [2001 isolated attosecond pulse experiment](2001-isolated-attosecond-pulse-experiment.md)
- [Attosecond physics](attosecond-physics.md)
- [Attosecond streaking](attosecond-streaking.md)
