<h1 id="section-b/unnumbered-electrostatics-question/solution">Solution</h1>

↑ **Parent:** [Unnumbered electrostatics question](../unnumbered-electrostatics-question.md)

The original PDF places this complete question before B6 without a visible question number. It is included here under a descriptive heading.

**Why images work.** In the [method of images](../../../../../method-of-images.md), place fictitious [image charges](../../../../../image-charge.md) outside the region where the physical [electric field](../../../../../electric-field-split.md) is required. Choose them so that the combined [electric potential](../../../../../electric-potential.md) satisfies the conductor [boundary conditions](../../../../../boundary-condition.md). The [Uniqueness of the Dirichlet problem](../../../../../uniqueness-of-the-dirichlet-problem.md) then proves that this construction gives the physical exterior field. The images do not describe the actual surface-charge locations.

Two examples are a charge $q$ above a grounded conducting plane, represented by $-q$ at the mirror point, and the [image charge for a grounded conducting sphere](../../../../../image-charge-for-a-grounded-conducting-sphere.md) used below. In each case the image lies inside the excluded conductor and makes its surface an equipotential of the required value.

**Potential of the two charges.** By the [law of cosines](../../../../../law-of-cosines.md), the distances from the observation point to charges at $x_j$ are $s_j=(r^2+x_j^2-2rx_j\cos\theta)^{1/2}$. The [superposition principle](../../../../../superposition-principle.md) and [Coulomb's law](../../../../../coulomb-s-law.md) therefore give

$$
\boxed{\phi(r,\theta)=\frac{q}{4\pi\varepsilon_0}
\left[\frac1{\sqrt{r^2+x_2^2-2rx_2\cos\theta}}
-\frac{\alpha}{\sqrt{r^2+x_1^2-2rx_1\cos\theta}}\right].}
$$

**The grounded sphere.** Set $r=a$ and require $s_1=\alpha s_2$ at every polar angle. Matching the coefficients of $\cos\theta$ and the constant terms gives

$$
x_1=\alpha^2x_2,\qquad a^2+x_1^2=\alpha^2(a^2+x_2^2).
$$

The useful noncoincident solution is

$$
\boxed{x_1=\frac{a^2}{x_2},\qquad \alpha=\frac a{x_2},\qquad
q'=-\frac{aq}{x_2}.}
$$

Indeed $s_1=(a/x_2)s_2$ on the sphere, so the two potential terms cancel there. A [Gaussian surface](../../../../../gaussian-surface.md) enclosing the sphere but not the external charge measures the total image charge in the exterior representation. Thus the physical induced net charge is

$$
\boxed{Q_{\rm sphere}=-\frac{aq}{x_2}.}
$$

**An isolated neutral sphere.** The grounded image would give nonzero net charge. Add a central image $q_0=+aq/x_2$ to cancel it. A central image changes the surface potential by a constant, preserving the equipotential condition, whereas an arbitrary off-centre image would generally spoil it. The [image charges for a neutral conducting sphere](../../../../../image-charges-for-a-neutral-conducting-sphere.md) give

$$
\boxed{q_0=\frac{aq}{x_2},\qquad
\phi_{\rm sphere}=\frac{q_0}{4\pi\varepsilon_0a}
=\frac{q}{4\pi\varepsilon_0x_2}.}
$$

The potential is measured relative to zero at infinity for each finite $x_2$.

**Fixed applied field and dipole moment.** For positive $q$ on the positive $x$ axis, the applied central field is $\mathbf E_0=-q\widehat{\mathbf x}/(4\pi\varepsilon_0x_2^2)$. The central image contributes no [electric dipole moment](../../../../../electric-dipole-moment.md), so

$$
\mathbf p=q'x_1\widehat{\mathbf x}
=-\frac{qa^3}{x_2^2}\widehat{\mathbf x}
=\boxed{4\pi\varepsilon_0a^3\mathbf E_0.}
$$

Its units are coulomb metres. Keeping $E_0$ fixed makes $q/x_2^2$ constant, so this induced moment is independent of the distance.

**The distant-charge limit.** As $x_2\to\infty$ with $q/x_2^2$ fixed, the applied field becomes uniform over any fixed neighbourhood of the sphere. The neutral pair of opposite images approaches a point dipole of the finite moment above. The external potential contains a growing spatial constant $q/(4\pi\varepsilon_0x_2)$, so the infinity-referenced conductor potential does not have a finite limit. Subtracting this irrelevant constant gives the usual [induced charge on a conducting sphere in a uniform electric field](../../../../../induced-charge-on-a-conducting-sphere-in-a-uniform-electric-field.md); the exterior potential becomes

$$
\boxed{\phi=-\mathbf E_0\cdot\mathbf r
+\frac{a^3\,\mathbf E_0\cdot\mathbf r}{r^3},\qquad r\ge a.}
$$

This has zero potential on the sphere, but a uniform applied field cannot simultaneously have its potential vanish at spatial infinity.

## ↑ Ancestors (14)

1. [Unnumbered electrostatics question](../unnumbered-electrostatics-question.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
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
