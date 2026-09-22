<h1 id="10b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiplying the tangential [equation of motion](../../../../../../equation-of-motion.md) by $r$ gives

$$
\frac d{dt}(r^2\dot\theta)=r^2\ddot\theta+2r\dot r\dot\theta=0.
$$

Therefore $h=r^2\dot\theta$ is constant. It is the signed [specific angular momentum](../../../../../../specific-angular-momentum.md); reverse the angular orientation if necessary to take $h>0$ for a nonradial [orbit](../../../../../../orbit-dynamical-system.md). Set $u=1/r$ and denote differentiation with respect to $\theta$ by a prime. Then

$$
\dot\theta=hu^2,\qquad \dot r=-hu',\qquad \ddot r=-h^2u^2u'',\qquad r\dot\theta^2=h^2u^3.
$$

Substitution into the radial [equation of motion](../../../../../../equation-of-motion.md) and division by $-h^2u^2$ give the [Binet equation](../../../../../../binet-equation.md)

$$
u''+u=\frac{GM}{h^2}.
$$

Its general solution is $u=GM/h^2+A\cos\theta+B\sin\theta$. Write $A=(GM/h^2)e\cos\theta_0$ and $B=(GM/h^2)e\sin\theta_0$, where $e\geq0$. This produces the [Kepler orbit](../../../../../../kepler-orbit.md)

$$
\boxed{\frac{h^2u}{GM}=1+e\cos(\theta-\theta_0).}
$$

Here $e$ is the [orbital eccentricity](../../../../../../orbital-eccentricity.md), and $\theta_0$ points toward [periapsis](../../../../../../periapsis.md) when $e>0$. Only portions with $u>0$ describe positive radial distances. The expression assumes $h\ne0$; a zero-[angular momentum](../../../../../../angular-momentum.md) trajectory is radial and must be treated separately.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
