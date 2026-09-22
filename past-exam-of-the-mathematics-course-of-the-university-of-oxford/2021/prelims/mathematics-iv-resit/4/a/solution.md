<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [polar coordinates](../../../../../../polar-coordinates.md), the rotating [unit vectors](../../../../../../unit-vector.md) satisfy $\dot{\mathbf e}_r=\dot\theta\mathbf e_\theta$ and $\dot{\mathbf e}_\theta=-\dot\theta\mathbf e_r$. Applying the [product rule](../../../../../../product-rule.md) twice to $\mathbf r=r\mathbf e_r$ gives the [velocity](../../../../../../velocity.md) and [acceleration](../../../../../../acceleration.md)

$$
\dot{\mathbf r}=\dot r\mathbf e_r+r\dot\theta\mathbf e_\theta,\qquad \ddot{\mathbf r}=(\ddot r-r\dot\theta^2)\mathbf e_r+(r\ddot\theta+2\dot r\dot\theta)\mathbf e_\theta.
$$

[Newton's second law](../../../../../../newton-s-second-law.md) for a [central force](../../../../../../central-force.md) now gives

$$
m(\ddot r-r\dot\theta^2)=F(r),\qquad m(r\ddot\theta+2\dot r\dot\theta)=0.
$$

Multiplying the azimuthal [force](../../../../../../force-split.md) equation by $r/m$ yields

$$
\frac{d}{dt}(r^2\dot\theta)=0,\qquad \boxed{r^2\dot\theta=h.}
$$

This is conservation of [specific angular momentum](../../../../../../specific-angular-momentum.md). Here $F(r)$ is the signed radial component of the [force](../../../../../../force-split.md); a negative value points inward.

When $h\ne0$, $\theta$ is a valid local parameter along the [trajectory](../../../../../../trajectory.md). Put $u=1/r$ and let primes denote [derivatives](../../../../../../derivative.md) with respect to $\theta$. The [chain rule](../../../../../../chain-rule.md) yields

$$
\dot\theta=hu^2,\qquad \dot r=-\frac{u'}{u^2}\dot\theta=-hu',\qquad \ddot r=-h^2u^2u'',\qquad r\dot\theta^2=h^2u^3.
$$

Substituting into the radial [Newton's second law](../../../../../../newton-s-second-law.md) equation and dividing by $-mh^2u^2$ proves the [Binet equation](../../../../../../binet-equation.md):

$$
\boxed{u''+u=-\frac{F(1/u)}{mh^2u^2}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
