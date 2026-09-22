<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $s_{ij}=M_{ij}^2$ and factor the three-body [phase space](../../../../lorentz-invariant-phase-space.md) through the pair $q=p_1+p_3$, with $s=q^2$:

$$
d\Phi_3=\frac{ds}{2\pi}\,d\Phi_2(P;q,p_2)\,d\Phi_2(q;p_1,p_3).
$$

A [scalar parent](../../../../scalar-particle.md) permits integration over the [overall orientation](../../../../rotation-mathematics.md). In its rest frame let the pair have [momentum](../../../../momentum-split.md) magnitude $p$, and in the pair rest frame let particle 3 have magnitude $p^*$. After integrating the azimuth of its direction, the two-body factors give

$$
d\Phi_3=\frac{p\,p^*}{64\pi^3M_0\sqrt{s}}\,ds\,d\cos\theta^*.
$$

In that pair rest frame, particle 2 has [momentum](../../../../momentum-split.md) magnitude $M_0p/\sqrt{s}$, so $|ds_{23}/d\cos\theta^*|=2M_0pp^*/\sqrt{s}$. The [Jacobian](../../../../jacobian-determinant.md) cancels both [momentum](../../../../momentum-split.md) factors, leaving

$$
\boxed{d\Phi_3=\frac{ds_{13}\,ds_{23}}{128\pi^3M_0^2},\qquad
\frac{d^2\Gamma}{ds_{13}ds_{23}}=\frac{|\mathcal M(s_{13},s_{23})|^2}{256\pi^3M_0^3}.}
$$

The physical domain is bounded by the requirement that the relative cosine lie between $-1$ and $1$. **The [phase-space](../../../../lorentz-invariant-phase-space.md) density is uniform within that domain; the event density is uniform only for a constant [squared amplitude](../../../../probability-amplitude.md).** [Scalar parent](../../../../scalar-particle.md) [spin](../../../../spin.md) alone does not forbid resonance-dependent [amplitudes](../../../../probability-amplitude.md). A factor $1/(s_{13}-m_R^2+im_R\Gamma_R)$ is a concrete nonuniform example. For two identical [pions](../../../../pion.md), a conventional overall $1/2!$ compensates integration over both labelings without changing the local flatness of [phase space](../../../../lorentz-invariant-phase-space.md).[Kinematics, equations (49.22)–(49.23): three-body Dalitz density and its bounds](../../../../review-of-particle-physics-by-particle-data-group-2022.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
