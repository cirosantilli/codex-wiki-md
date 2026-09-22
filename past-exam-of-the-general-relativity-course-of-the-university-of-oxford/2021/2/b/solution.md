<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [metric signature](../../../../metric-signature.md) $-+++$ and [transverse-traceless gauge](../../../../transverse-traceless-gauge.md), $g_{ij}=\delta_{ij}+h_{ij}^{\rm TT}$. To resolve the source's origin ambiguity, put the detector centre at $z=0$ and the source centre at $z=-r_0$, so the [gravitational wave](../../../../gravitational-wave-split.md) travels in the positive $z$ direction. Reversing that direction replaces $z$ by $-z$. Work in the [weak-field approximation](../../../../weak-field-approximation.md), with $\omega l\ll c$, $r_0\gg l,c/\omega$, and detector size $a\ll c/\omega,r_0$. The [radiation reaction](../../../../radiation-reaction.md) is neglected, so the rod maintains the prescribed steady motion.

At the retarded source time $u=t-(r_0+z)/c$, take the source positions as $\mathbf x_\pm=\pm l(\cos(\omega u+\beta),\sin(\omega u+\beta),0)$. The arbitrary constant $\beta$ specifies the initial source phase. The [second mass moment tensor](../../../../second-mass-moment-tensor.md) $I_{ij}=\sum_A Mx_{Ai}x_{Aj}$ obeys

$$
I_{xx}=Ml^2[1+\cos\Phi],\quad I_{yy}=Ml^2[1-\cos\Phi],\quad
I_{xy}=I_{yx}=Ml^2\sin\Phi,\qquad
\Phi=2\omega\left(t-\frac{r_0+z}{c}\right)+2\beta.
$$

The [quadrupole formula](../../../../quadrupole-formula.md) $h_{ij}^{\rm TT}=2G\ddot I_{ij}^{\rm TT}/(c^4r_0)$ projects away the transverse trace, which is already constant here. Differentiating twice therefore gives

$$
\boxed{h_{xx}=-H\cos\Phi,\qquad h_{yy}=H\cos\Phi,\qquad
h_{xy}=h_{yx}=-H\sin\Phi,\qquad
H=\frac{8GMl^2\omega^2}{c^4r_0}.}
$$

All time and longitudinal [metric perturbation](../../../../linearized-gravity-split.md) components vanish in [transverse-traceless gauge](../../../../transverse-traceless-gauge.md). The [gravitational-wave frequency](../../../../gravitational-wave-frequency.md) is $2\omega$ in angular units; $M$ is each source [mass](../../../../mass.md), not their sum, and the detector [mass](../../../../mass.md) $m$ does not enter the strain. The [plane wave](../../../../plane-wave.md) approximation holds the amplitude fixed at $r_0$; retaining spherical spreading replaces its denominator by $r_0+z$ near the axis. The retarded [quadrupole formula](../../../../quadrupole-formula.md) and the distinction between source and wave [frequency](../../../../frequency.md) are derived in [Sections 5.3.1–5.3.2, retarded source solution and circular binary](../../../../general-relativity-by-david-tong.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
