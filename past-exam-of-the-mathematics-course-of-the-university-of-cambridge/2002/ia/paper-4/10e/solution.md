<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A [central force](../../../../../central-force.md) has zero [torque](../../../../../torque.md), so $h=r^2\dot\theta$ is constant and the [angular momentum](../../../../../angular-momentum.md) is $mh$. The [areal velocity](../../../../../areal-velocity.md) is $h/2$. Put $u=1/r$ and let primes denote angular [derivatives](../../../../../derivative.md). Then $\dot r=-hu'$, $\ddot r=-h^2u^2u''$, and $r\dot\theta^2=h^2u^3$. The radial equation with inward force magnitude $f(u)$ is $m(\ddot r-r\dot\theta^2)=-f(u)$, giving the [Binet equation](../../../../../binet-equation.md)

$$
\boxed{u''+u=\frac{f(u)}{mh^2u^2}}.
$$

Choose the angular origin along a diameter of a radius-$R$ circle through $O$. Its polar equation is $r=2R\cos\theta$, so $u=(2R)^{-1}\sec\theta$ on $-\pi/2<\theta<\pi/2$. Since $(\sec\theta)''+\sec\theta=2\sec^3\theta$, substitution gives $u''+u=8R^2u^3$ and hence

$$
\boxed{f(u)=cu^5,\qquad c=8mh^2R^2>0}.
$$

The force is **attractive**. For fixed force coefficient $c$ and mass, $R|mh|=\sqrt{mc/8}$, so $R$ is inversely proportional to the magnitude of the [angular momentum](../../../../../angular-momentum.md). The time along the circle is

$$
\boxed{T=\int_{-\pi/2}^{\pi/2}\frac{r^2}{|h|}\,d\theta=\frac{2\pi R^2}{|h|}=4\sqrt2\,\pi\sqrt{\frac mc}R^3}.
$$

This [circular orbit through an inverse-fifth-power singularity](../../../../../circular-orbit-through-an-inverse-fifth-power-singularity.md) reaches the force center at the two endpoints of this angular interval. The integral is finite; continuation through the singular collision is not specified by the force law alone.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
