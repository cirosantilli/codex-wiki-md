<h1 id="section-b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Only the $1/r$ fields transport a nonzero outgoing [power](../../../../../power.md) to infinity. Retain those terms from the [Hertzian dipole](../../../../../hertzian-dipole.md) fields:

$$
E_\theta^{\rm rad}=\frac{\sin\theta}{4\pi\epsilon_0c^2r}[\ddot p],\qquad
B_\phi^{\rm rad}=\frac{\mu_0\sin\theta}{4\pi cr}[\ddot p]
=\frac{E_\theta^{\rm rad}}c.
$$

The brackets mean evaluation at the [retarded time](../../../../../retarded-time.md),

$$
[\ddot p]\equiv\ddot p(t-r/c),
$$

for a point source at the origin in [vacuum](../../../../../vacuum.md). They are not a time average. The radial [Poynting vector](../../../../../poynting-vector.md) in the [radiation zone](../../../../../radiation-zone.md) is

$$
S_r=\frac1{\mu_0}E_\theta^{\rm rad}B_\phi^{\rm rad}
=\frac{\mu_0}{16\pi^2cr^2}[\ddot p]^2\sin^2\theta.
$$

Integrating over a [sphere](../../../../../sphere.md) uses

$$
\int\sin^2\theta\,d\Omega=2\pi\int_0^\pi\sin^3\theta\,d\theta=\frac{8\pi}3.
$$

Therefore

$$
\boxed{P(t,r)=\int r^2S_r\,d\Omega=\frac{\mu_0}{6\pi c}[\ddot p]^2.}
$$

Near-field terms either give inverse powers of $r$ after the surface integral or describe reversible exchange with the near field. The emitted [power](../../../../../power.md) labelled by source time $t_{\rm src}$ is $\mu_0\ddot p(t_{\rm src})^2/(6\pi c)$; the enclosing surface receives it one light-travel time later. For a changing dipole orientation, the general form is $P=\mu_0|\ddot{\mathbf p}|^2/(6\pi c)$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
