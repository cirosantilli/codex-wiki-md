<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**Inductance and interface conditions.** For a linear coil, [self-inductance](../../../../../self-inductance.md) is the ratio $L=\Lambda/I$ of its own [magnetic flux linkage](../../../../../magnetic-flux-linkage.md) $\Lambda=N\Phi$ to current. Its induced [electromotive force](../../../../../electromotive-force.md) is $-L\,dI/dt$ for fixed $L$. Across an interface with unit normal $\mathbf n$ from medium 1 to 2,

$$
\boxed{\mathbf n\cdot(\mathbf B_2-\mathbf B_1)=0,\qquad
\mathbf n\times(\mathbf H_2-\mathbf H_1)=\mathbf K_f.}
$$

These [electromagnetic boundary conditions](../../../../../electromagnetic-boundary-condition.md) follow from [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) and [Ampère's law](../../../../../ampere-s-circuital-law.md). Here $\mathbf K_f$ is [free surface](../../../../../free-surface.md) current. At the iron–air faces there is no [free surface](../../../../../free-surface.md) current, so normal [magnetic flux density](../../../../../magnetic-field-split.md) and tangential [magnetic field intensity](../../../../../magnetic-field-intensity.md) are continuous. In each isotropic linear medium, $\mathbf B=\mu_0\mu_r\mathbf H$.

**Complete core.** A slender [toroid](../../../../../toroid.md) has approximately uniform $H$ along mean path length $\ell$. [Ampère's law](../../../../../ampere-s-circuital-law.md) gives $H\ell=NI$, so $B=\mu\mu_0NI/\ell$. The flux per turn is $\Phi=BA$, yielding the [inductance of a toroidal winding](../../../../../inductance-of-a-toroidal-winding.md),

$$
\boxed{L_0=\frac{N\Phi}{I}=\frac{\mu\mu_0N^2A}{\ell}.}
$$

This uses constant relative [magnetic permeability](../../../../../permeability-electromagnetism.md) $\mu$ and neglects leakage, fringing and saturation.

**Why the gap lowers inductance.** The gap replaces an easy magnetic path in iron with air. Maintaining the same flux now requires a much larger [magnetic field intensity](../../../../../magnetic-field-intensity.md) in part of the path and therefore more ampere-turns. Equivalently, [magnetic reluctance](../../../../../magnetic-reluctance.md) increases, so the flux linkage for a fixed current and hence [self-inductance](../../../../../self-inductance.md) decrease. A narrow gap can matter greatly because its permeability is smaller by the factor $\mu$.

**Oblique-gap calculation.** In the original diagram $t$ is the perpendicular separation of the cut faces. Let $\mathbf s$ point along the core, and let $\mathbf n,\mathbf q$ be normal and tangential to the gap faces. With the face at angle $\theta$ to the core direction, $\mathbf s=\sin\theta\,\mathbf n+\cos\theta\,\mathbf q$. Write the core flux density as $B\mathbf s$. The boundary conditions give

$$
B_{g,n}=B\sin\theta,\qquad
H_{g,q}=\frac{B\cos\theta}{\mu\mu_0},
$$

so

$$
\mathbf H_g=\frac B{\mu_0}
\left(\sin\theta\,\mathbf n+\frac{\cos\theta}{\mu}\mathbf q\right).
$$

The gap area normal to its nearly normal field is $A/\sin\theta$, not $A$. Its leading reluctance is consequently $t\sin\theta/(\mu_0A)$. Adding the core reluctance gives the [inductance of a toroid with an oblique narrow air gap](../../../../../inductance-of-a-toroid-with-an-oblique-narrow-air-gap.md),

$$
NI\simeq\frac B{\mu_0}
\left(\frac\ell\mu+t\sin\theta\right),
\qquad L\simeq\frac{\mu_0N^2A}{\ell/\mu+t\sin\theta}.
$$

Thus at $\theta=45^\circ$,

$$
\boxed{L\simeq\frac{\mu\mu_0N^2A}{\ell+\mu t/\sqrt2}.}
$$

The approximation retains the possibly order-one ratio $\mu t/\ell$ while neglecting $t/\ell$, fringing and the small tangential gap contribution. More precisely, a local uniform-field path along the core, with missing iron length $t/\sin\theta$ subtracted, gives denominator $\ell/\mu+t\sin\theta(1-1/\mu)$. Its correction is beyond the stipulated large-$\mu$, narrow-gap accuracy; simply neglecting $\mu t$ would not be justified.

**Field in the slot.** The component expression above gives

$$
H_g=\frac B{\mu_0}\sqrt{\sin^2\theta+\frac{\cos^2\theta}{\mu^2}}.
$$

For the $45^\circ$ gap and $\mu\gg1$,

$$
\boxed{H_g\simeq\frac{B}{\sqrt2\mu_0}
\simeq\frac{NI}{t+\sqrt2\ell/\mu}.}
$$

Its units are $\mathrm{A\,m^{-1}}$. The field is almost perpendicular to the cut faces, rather than following the iron direction straight across the cut. Its small angle away from the face normal satisfies $\tan\alpha=1/\mu$ at $45^\circ$; the sense reverses if the current reverses.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
