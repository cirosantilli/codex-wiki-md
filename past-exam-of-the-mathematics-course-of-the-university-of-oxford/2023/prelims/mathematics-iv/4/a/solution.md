<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Divide [Newton's second law](../../../../../../newton-s-second-law.md) by the [mass](../../../../../../mass.md) and resolve along the radial and transverse unit [vectors](../../../../../../vector.md) in [polar coordinates](../../../../../../polar-coordinates.md). A [central force](../../../../../../central-force.md) has no transverse component, so

$$
\ddot r-r\dot\theta^2=-F(r),\qquad2\dot r\dot\theta+r\ddot\theta=0.
$$

Multiplication of the second equation by $r$ shows that $d(r^2\dot\theta)/dt=0$. Thus

$$
\boxed{\ddot r-r\dot\theta^2=-F(r),\qquad r^2\dot\theta=h,}
$$

where $h$ is the signed [specific angular momentum](../../../../../../specific-angular-momentum.md) perpendicular to the [orbital plane](../../../../../../orbital-plane.md).

If $h\ne0$ and $r>0$, the [polar angle](../../../../../../polar-angle.md) is locally a valid independent variable. For $u=1/r$, use primes for [derivatives](../../../../../../derivative.md) with respect to $\theta$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\dot\theta=hu^2,\qquad\dot r=-hu',\qquad\ddot r=-h^2u^2u'',\qquad r\dot\theta^2=h^2u^3.
$$

Substitution into the radial equation gives the [Binet equation](../../../../../../binet-equation.md)

$$
\boxed{u''+u=\frac{F(1/u)}{h^2u^2}.}
$$

If $h=0$, the [orbit](../../../../../../orbit-dynamical-system.md) is radial and division by $h$ is unavailable; the first radial equation still applies with $\dot\theta=0$ away from the origin.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
