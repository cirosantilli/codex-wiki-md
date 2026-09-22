<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $a_{\rm ns}$ be the neutron star's distance from the [centre of mass](../../../../../center-of-mass.md). In a circular orbit,

$$
a_{\rm ns}=a\frac{M_{\rm wd}}{M_{\rm ns}+M_{\rm wd}},
\qquad
K=\frac{2\pi a_{\rm ns}}P\sin i.
$$

Combining this with [Kepler third law](../../../../../kepler-s-third-law.md),

$$
\frac{4\pi^2a^3}{P^2}=G(M_{\rm ns}+M_{\rm wd}),
$$

gives the [binary mass function](../../../../../binary-mass-function.md)

$$
\boxed{F\equiv\frac{PK^3}{2\pi G}
=\frac{M_{\rm wd}^3\sin^3i}
{(M_{\rm ns}+M_{\rm wd})^2}}.
$$

Since $\sin i\leq1$ and $(M_{\rm ns}+M_{\rm wd})^2>M_{\rm wd}^2$,

$$
\boxed{F<M_{\rm wd}}.
$$

When a low-mass red giant undergoes stable [Roche-lobe overflow](../../../../../roche-lobe-overflow.md), the neutron star receives matter with substantial [specific angular momentum](../../../../../specific-angular-momentum.md), usually through an [accretion disk](../../../../../accretion-disk.md). The accretion torque spins it up and weakens its external magnetic field, producing a [recycled pulsar](../../../../../recycled-pulsar.md) with a millisecond period. Removal of the donor's envelope exposes its helium core as a low-mass [white dwarf](../../../../../white-dwarf.md).

At detachment, the donor mass and core mass both become $M_{\rm wd}$. Its luminosity is fixed by the red-giant core-mass--luminosity relation, and the supplied radius law therefore makes its final radius $R_L$ a function only of $M_{\rm wd}$. Cubing the Roche-lobe relation gives

$$
\frac{R_L^3}{a^3}
=\frac{M_{\rm wd}}{M_{\rm wd}+M_{\rm ns}}.
$$

Eliminating $a$ with [Kepler third law](../../../../../kepler-s-third-law.md) yields

$$
\boxed{P^2=\frac{4\pi^2R_L(M_{\rm wd})^3}{GM_{\rm wd}}}.
$$

This is the [white-dwarf mass--orbital-period relation](../../../../../white-dwarf-mass-orbital-period-relation.md): dependence on the neutron-star mass cancels.

For randomly oriented binaries, the [isotropic binary inclination distribution](../../../../../isotropic-binary-inclination-distribution.md) is

$$
\boxed{p(i)=\sin i,\qquad0\leq i\leq\frac\pi2}.
$$

The observed period gives $M_{\rm wd}$ from the preceding relation. If $M_{\rm ns}=1.35M_\odot$ is adopted, the measured mass function then gives

$$
\boxed{\sin i=
\left[\frac{F(M_{\rm ns}+M_{\rm wd})^2}
{M_{\rm wd}^3}\right]^{1/3}},
$$

so the inclination is inferred without astrometry.

Two plausible causes of an apparent shortage of edge-on systems are:

- High-inclination radio systems are preferentially obscured or eclipsed by ionized gas near the companion, producing an observational selection effect.
- Accretion makes recycled neutron stars systematically heavier than $1.35M_\odot$. Using too small an assumed $M_{\rm ns}$ makes the inferred $\sin i$ too small and shifts truly high-inclination systems to lower inferred inclinations.

Scatter or bias in the core-mass--period relation can reinforce the second effect.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
