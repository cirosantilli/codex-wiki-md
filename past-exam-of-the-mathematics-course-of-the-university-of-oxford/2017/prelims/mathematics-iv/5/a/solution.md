<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Write $\mu=GM$. In [polar coordinates](../../../../../../polar-coordinates.md), [Newton's second law](../../../../../../newton-s-second-law.md) per unit [mass](../../../../../../mass.md) gives the radial and transverse [equations of motion](../../../../../../equation-of-motion.md)

$$
\ddot r-r\dot\theta^2=-\frac\mu{r^2},\qquad
r\ddot\theta+2\dot r\dot\theta=0.
$$

The transverse [equation](../../../../../../equation.md) implies

$$
\frac d{dt}(r^2\dot\theta)=r(r\ddot\theta+2\dot r\dot\theta)=0,
\qquad\boxed{h=r^2\dot\theta\text{ is constant}.}
$$

This is [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) per unit [mass](../../../../../../mass.md). For the nonradial [trajectory](../../../../../../trajectory.md) in the next part, choose [orientation](../../../../../../orientation-of-a-simplex.md) so $h>0$. With $u=1/r$ and primes denoting [derivatives](../../../../../../derivative.md) with respect to $\theta$, the [chain rule](../../../../../../chain-rule.md) gives

$$
\dot\theta=hu^2,\qquad \dot r=-hu',\qquad \ddot r=-h^2u^2u''.
$$

Substituting into the radial [equation](../../../../../../equation.md) yields $-h^2u^2(u''+u)=-\mu u^2$, hence

$$
\boxed{u''+u=\frac{GM}{h^2}.}
$$

The change of independent variable requires $h\ne0$; a purely radial [trajectory](../../../../../../trajectory.md) instead has constant $\theta$.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [5](../../5.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
