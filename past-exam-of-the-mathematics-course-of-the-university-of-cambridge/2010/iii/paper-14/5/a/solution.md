<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The forcing is perpendicular to velocity, so

$$
\frac d{dt}|\dot\gamma|^2=2f\langle i\dot\gamma,\dot\gamma\rangle=0.
$$

Starting at unit speed therefore keeps the motion in $SM$. The horizontal part is the geodesic transport $X$, while the acceleration rotates the unit velocity at angular speed $f$. Thus the [magnetic flow](../../../../../../magnetic-flow-on-a-riemannian-surface.md) generator is $F=X+(f\circ\pi)V$.

For the [canonical coframe of a surface unit tangent bundle](../../../../../../canonical-coframe-of-a-surface-unit-tangent-bundle.md), set $\mu=\alpha\wedge\theta\wedge\omega$. Its [interior product of a differential form](../../../../../../interior-product.md) with the two relevant fields is

$$
\iota_X\mu=\theta\wedge\omega,\qquad
\iota_V\mu=\alpha\wedge\theta.
$$

The structure equations give

$$
d(\theta\wedge\omega)=d\theta\wedge\omega-\theta\wedge d\omega=0,
\qquad d(\alpha\wedge\theta)=0.
$$

The [Cartan formula for the Lie derivative](../../../../../../cartan-s-magic-formula.md) consequently gives $\mathcal L_X\mu=\mathcal L_V\mu=0$. For the variable vertical coefficient, use the full product rule:

$$
\mathcal L_{fV}\mu=d(f\iota_V\mu)
=df\wedge\alpha\wedge\theta+f\,d(\alpha\wedge\theta)=0.
$$

Indeed $f$ is pulled back from the base, so $Vf=0$ and $df$ has only $\alpha,\theta$ components. Hence

$$
\boxed{\mathcal L_F\mu=0,\qquad \phi_t^*\mu=\mu}.
$$

The [Liouville volume of a surface geodesic flow](../../../../../../liouville-volume-of-a-surface-geodesic-flow.md) is therefore preserved by this magnetic modification for every smooth $f$, without requiring the Anosov property.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
