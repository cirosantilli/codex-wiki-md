<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $z$ increasing upwards and write $s=\phi/\phi_{\max}$. The particles have downward [settling velocity](../../../../../../settling-velocity.md); their upward [volume flux](../../../../../../volumetric-flow-rate.md) is $\phi V$. Conservation of particle volume in any interval gives

$$
\frac{d}{dt}\int_{z_1}^{z_2}\phi\,dz=\phi V(z_1,t)-\phi V(z_2,t).
$$

Thus the [kinematic sedimentation](../../../../../../kinematic-sedimentation.md) equation and its [characteristic speed](../../../../../../characteristic-speed.md) are

$$
\boxed{s_t+\partial_zf(s)=0,\qquad f(s)=-V_0s(1-s)^\alpha,}
$$



$$
a(s)=f'(s)=-V_0(1-s)^{\alpha-1}\bigl[1-(\alpha+1)s\bigr].
$$

For $0<s<1$ this is a scalar [hyperbolic partial differential equation](../../../../../../hyperbolic-partial-differential-equation.md): its one [characteristic speed](../../../../../../characteristic-speed.md) is real. The [method of characteristics](../../../../../../method-of-characteristics.md) gives $ds/dt=0$ and $dz/dt=a(s)$. A [concentration](../../../../../../concentration.md) disturbance need not descend at the particle [settling velocity](../../../../../../settling-velocity.md); $a(s)$ is the [derivative](../../../../../../derivative.md) of the transported flux, not $V(s)$. In particular $a(s)$ can be positive even though every particle settles downwards. At $\alpha=0$, $a=-V_0$ and the equation is ordinary translation. At the packing endpoint $s=1$ the differentiability of the chosen constitutive law depends on $\alpha$; none of the initial values used below is at that endpoint.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
