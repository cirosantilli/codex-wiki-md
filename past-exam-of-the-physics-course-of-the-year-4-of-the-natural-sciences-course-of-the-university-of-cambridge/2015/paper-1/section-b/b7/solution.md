<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

A [magnetic dipole](../../../../../magnetic-dipole.md) is the leading magnetic source moment of a localized steady current distribution. For a small planar loop, $\mathbf m=I\mathbf A$ with area orientation set by the right-hand rule. A fixed permanent moment in a slowly varying external field has [energy](../../../../../energy-split.md) $U=-\mathbf m\cdot\mathbf B$ and [force](../../../../../force-split.md) $\mathbf F=\nabla(\mathbf m\cdot\mathbf B)$.

For the given purely azimuthal vector potential, the spherical curl gives

$$
B_r=\frac1{r\sin\theta}\frac\partial{\partial\theta}(A_\phi\sin\theta)
=\frac{\mu_0}{4\pi}\frac{2m\cos\theta}{r^3},
\qquad
B_\theta=-\frac1r\frac\partial{\partial r}(rA_\phi)
=\frac{\mu_0}{4\pi}\frac{m\sin\theta}{r^3},\qquad B_\phi=0.
$$

These are the [magnetic dipole field](../../../../../magnetic-dipole-field.md) components outside the localized source.

The conducting shell has $Q=4\pi\epsilon_0aV$ and [surface charge density](../../../../../surface-charge-density.md) $\sigma=Q/(4\pi a^2)$. A latitude strip of area $2\pi a^2\sin\theta\,d\theta$ carries current $dI=\sigma\omega a^2\sin\theta\,d\theta$. Its loop area is $\pi a^2\sin^2\theta$, giving

$$
m=\pi\sigma\omega a^4\int_0^\pi\sin^3\theta\,d\theta
=\frac{Q\omega a^2}{3}.
$$

In vector form the [magnetic moment of a rotating charged spherical shell](../../../../../magnetic-moment-of-a-rotating-charged-spherical-shell.md) is

$$
\boxed{\mathbf m=\frac{Qa^2}{3}\boldsymbol\omega
=\frac{4\pi}{3}\epsilon_0a^3V\boldsymbol\omega.}
$$

The positive-z expression in the question takes $\boldsymbol\omega=\omega\hat{\mathbf z}$. “Clockwise” needs a viewing direction: this rotation looks clockwise when viewed looking along $+z$ from below, and counterclockwise when viewed from the positive-z side. Looking from the other end reverses the verbal label, not the vector relation.

Since the positive charge and the loop current circulate in the same stated sense, their dipole moments are parallel when judged from a common viewpoint. At $h\gg R$, the loop's axial field magnitude is $B\simeq\mu_0IR^2/(2h^3)$. With the sphere small compared with that variation scale,

$$
\boxed{F_z=m\frac{dB}{dh}=-\frac{3\mu_0IR^2m}{2h^4}
=-\frac{2\pi\mu_0\epsilon_0IR^2a^3\omega V}{h^4}.}
$$

**The magnetic [force](../../../../../force-split.md) is attractive**, pulling the sphere toward the loop. Reversing only one circulation would reverse that magnetic [force](../../../../../force-split.md). The calculation treats the rotating charge as a prescribed moment and uses the stated separated length scales; it does not add unrelated induction or electric interactions to the dipole model.

## ↑ Ancestors (13)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
