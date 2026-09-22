<h1 id="section-b/10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**Point-charge field and superposition**. [Coulomb's law](../../../../coulomb-s-law.md) gives the [Coulomb force](../../../../coulomb-force.md) on a test [electric charge](../../../../electric-charge-split.md) $q_t$ a displacement $\mathbf R$ from a source [point charge](../../../../point-charge.md) $Q$:

$$
\mathbf F=\frac{Qq_t}{4\pi\epsilon_0}\frac{\mathbf R}{R^3}.
$$

The [electric field](../../../../electric-field-split.md) is force per infinitesimal test charge, so

$$
\boxed{\mathbf E=\frac{\mathbf F}{q_t}
=\frac{Q}{4\pi\epsilon_0R^2}\hat{\mathbf R}.}
$$

It points outward for positive $Q$ and inward for negative $Q$. For several [point charges](../../../../point-charge.md), the [superposition principle](../../../../superposition-principle.md) adds their fields as [vectors](../../../../vector.md):

$$
\mathbf E(\mathbf r)=\frac1{4\pi\epsilon_0}\sum_i
q_i\frac{\mathbf r-\mathbf r_i}{|\mathbf r-\mathbf r_i|^3}.
$$

This formula excludes the source points themselves, where the ideal point-charge field is singular.

**Exact field components of the pair**. Put

$$
R_+=\sqrt{(x-a)^2+y^2},\qquad
R_-=\sqrt{(x+a)^2+y^2}.
$$

The displacement vectors from the positive and negative charges to the observation point are $(x-a)\hat{\mathbf i}+y\hat{\mathbf j}$ and $(x+a)\hat{\mathbf i}+y\hat{\mathbf j}$. Including the signs of the charges gives

$$
\mathbf E(x,y)=\frac q{4\pi\epsilon_0}
\left[\frac{(x-a)\hat{\mathbf i}+y\hat{\mathbf j}}{R_+^3}
-\frac{(x+a)\hat{\mathbf i}+y\hat{\mathbf j}}{R_-^3}\right].
$$

Reading off both components,

$$
\boxed{E_x=\frac q{4\pi\epsilon_0}
\left[\frac{x-a}{((x-a)^2+y^2)^{3/2}}
-\frac{x+a}{((x+a)^2+y^2)^{3/2}}\right],}
$$



$$
\boxed{E_y=\frac{qy}{4\pi\epsilon_0}
\left[\frac1{((x-a)^2+y^2)^{3/2}}
-\frac1{((x+a)^2+y^2)^{3/2}}\right].}
$$

For example, on the perpendicular bisector $x=0$, the two $y$ components cancel and the $x$ components add toward the negative charge, checking both relative signs.

**Far-field polar components**. The pair's [electric dipole moment](../../../../electric-dipole-moment.md) points from negative to positive charge:

$$
\mathbf p=2qa\hat{\mathbf i},\qquad p=2qa.
$$

Use [polar coordinates](../../../../polar-coordinates.md) $x=r\cos\theta$, $y=r\sin\theta$, with $\theta$ measured from that positive dipole axis. The supplied leading [electric dipole field](../../../../electric-dipole-field.md) becomes

$$
E_x=\frac{p}{4\pi\epsilon_0r^3}(3\cos^2\theta-1),\qquad
E_y=\frac{p}{4\pi\epsilon_0r^3}(3\cos\theta\sin\theta).
$$

Taking the [dot products](../../../../dot-product.md) with the radial and angular unit vectors gives

$$
\begin{aligned}
E_r&=E_x\cos\theta+E_y\sin\theta
=\frac p{4\pi\epsilon_0r^3}\left[3\cos\theta(\cos^2\theta+\sin^2\theta)-\cos\theta\right],\\
E_\theta&=-E_x\sin\theta+E_y\cos\theta
=\frac p{4\pi\epsilon_0r^3}\sin\theta.
\end{aligned}
$$

Therefore

$$
\boxed{E_r=\frac{2p\cos\theta}{4\pi\epsilon_0r^3},\qquad
E_\theta=\frac{p\sin\theta}{4\pi\epsilon_0r^3}.}
$$

The unit vectors for [polar coordinates](../../../../polar-coordinates.md) are orthonormal, so the magnitude is

$$
\boxed{|\mathbf E(r,\theta)|=\sqrt{E_r^2+E_\theta^2}
=\frac{p}{4\pi\epsilon_0r^3}\sqrt{1+3\cos^2\theta},\qquad r\gg a.}
$$

The units are $\mathrm{N\,C^{-1}}$, since the [electric dipole moment](../../../../electric-dipole-moment.md) has units $\mathrm{C\,m}$.

**Angular sketch and comparison**. At fixed large $r$, the magnitude has period $\pi$. It is largest on the dipole axis, $\theta=0,\pi$, with value $2p/(4\pi\epsilon_0r^3)$, and smallest on the perpendicular directions, $\theta=\pi/2,3\pi/2$, with value $p/(4\pi\epsilon_0r^3)$. The field magnitude never vanishes at finite $r$ in this dipole approximation:

<a id="section-b/10/image-the-angular-dependence-of-the-far-field-electric-dipole-magnitude-at-a-fixed-radius"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019-ia-physics-q10-dipole-angular-field.png)

**[Figure 6](#section-b/10/image-the-angular-dependence-of-the-far-field-electric-dipole-magnitude-at-a-fixed-radius). The angular dependence of the far-field electric dipole magnitude at a fixed radius**.

The neutral charge pair has no net [electric charge](../../../../electric-charge-split.md), so its leading far field falls as $r^{-3}$ and depends on direction. An isolated nonzero [point charge](../../../../point-charge.md) has an $r^{-2}$ field whose magnitude is isotropic, with purely radial direction. The dipole also generally has a nonzero $E_\theta$ component.

A molecular example is the interaction between permanent [electric dipoles](../../../../electric-dipole.md) of [hydrogen chloride](../../../../hydrogen-chloride.md) molecules, whose unequal charge distributions give each molecule a nonzero [electric dipole moment](../../../../electric-dipole-moment.md). The [electric dipole-dipole interaction](../../../../electric-dipole-dipole-interaction.md) depends on their relative orientations:

$$
U=\frac{\mathbf p_1\cdot\mathbf p_2
-3(\mathbf p_1\cdot\hat{\mathbf r})(\mathbf p_2\cdot\hat{\mathbf r})}
{4\pi\epsilon_0r^3}.
$$

For two parallel dipoles pointing along their line of separation, $U=-2p_1p_2/(4\pi\epsilon_0r^3)<0$, illustrating an attractive molecular configuration.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
