<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

In [plane polar coordinates](../../../../../plane-polar-coordinates.md), use $\mathbf e_r=(\cos\theta,\sin\theta)$ and $\mathbf e_\theta=(-\sin\theta,\cos\theta)$. Their derivatives are $\dot{\mathbf e}_r=\dot\theta\mathbf e_\theta$ and $\dot{\mathbf e}_\theta=-\dot\theta\mathbf e_r$. Differentiating $\mathbf r=r\mathbf e_r$ gives the velocity and [acceleration in polar coordinates](../../../../../acceleration-in-polar-coordinates.md):

$$
\boxed{\mathbf v=\dot r\mathbf e_r+r\dot\theta\mathbf e_\theta,\qquad \mathbf a=(\ddot r-r\dot\theta^2)\mathbf e_r+(r\ddot\theta+2\dot r\dot\theta)\mathbf e_\theta.}
$$

Both the electrostatic [inverse-square force](../../../../../inverse-square-force.md) and the drag point radially, so the [torque](../../../../../torque.md) about the origin is zero even though the force depends on radial velocity. The vector [angular momentum](../../../../../angular-momentum.md) $\mathbf h=\mathbf r\times\dot{\mathbf r}$ is constant. For $\mathbf h\ne0$, every position lies in the fixed plane perpendicular to it; if $\mathbf h=0$, the trajectory is radial and still lies in a plane. In the nonzero case the transverse equation is $r\ddot\theta+2\dot r\dot\theta=0$, giving

$$
\boxed{h=r^2\dot\theta=\text{constant}.}
$$

The signed $h$ depends on the plane orientation. The stipulated ratio $k/|h|$ requires $h\ne0$.

Set $u=1/r$ and use primes for differentiation with respect to $\theta$. Then $\dot\theta=hu^2$, $\dot r=-hu'$ and $\ddot r=-h^2u^2u''$. The radial equation is $\ddot r-r\dot\theta^2=-p/r^2-k\dot r/r^2$, so

$$
-h^2u^2(u''+u)=-pu^2+khu^2u',\qquad \boxed{u''+\frac kh u'+u=\frac p{h^2}.}
$$

This [damped Binet equation](../../../../../damped-binet-equation.md) has the general solution, for $k/|h|<2$,

$$
\boxed{u(\theta)=\frac p{h^2}+e^{-k(\theta-\theta_0)/(2h)}\left[C\cos\!\big(\omega(\theta-\theta_0)\big)+D\sin\!\big(\omega(\theta-\theta_0)\big)\right],\quad \omega=\sqrt{1-\frac{k^2}{4h^2}}.}
$$

It is used on the physical interval where $u>0$. For either sign of $h$, introduce the forward angular distance $\phi=\operatorname{sgn}(h)(\theta-\theta_0)$; then the exponential is $e^{-k\phi/(2|h|)}$. Thus damping acts forward in time for both orientations, not just when $h>0$.

For unit mass, the [kinetic energy](../../../../../kinetic-energy.md) is $\tfrac12(\dot r^2+r^2\dot\theta^2)$ and the electrostatic [potential energy](../../../../../potential-energy.md) is $-p/r$. Therefore

$$
\boxed{E=\frac{h^2}{2}(u'^2+u^2)-pu.}
$$

Using the [damped Binet equation](../../../../../damped-binet-equation.md),

$$
\frac{dE}{d\theta}=h^2u'\left(u''+u-\frac p{h^2}\right)=-khu'^2,
$$

and multiplication by $\dot\theta=hu^2$ gives

$$
\boxed{\frac{dE}{dt}=-kh^2u^2u'^2=-\frac{k\dot r^2}{r^2}\le0.}
$$

This is also the drag force times the radial speed. **Energy is nonincreasing in time**, strictly decreasing while radial motion occurs; a circular trajectory already has constant energy. The sign of $dE/d\theta$ alone would be misleading for negative $h$.

To justify [circularization under radial inverse-square drag](../../../../../circularization-under-radial-inverse-square-drag.md), suppose the forward trajectory remains bounded, $r\le R_*$. Since $E\le E(0)$ and the effective radial [potential energy](../../../../../potential-energy.md) $h^2/(2r^2)-p/r$ tends to $+\infty$ as $r\to0$, the radius is also bounded away from zero. Velocity then stays bounded, so the solution continues for all forward time without collision. Moreover $\dot\phi=|h|/r^2\ge|h|/R_*^2$, so $\phi\to\infty$. The decaying general solution gives $u\to p/h^2$ and $u'\to0$. Consequently

$$
\boxed{r\to\frac{h^2}{p},\qquad\dot r\to0,\qquad E\to-\frac{p^2}{2h^2}.}
$$

The tangential motion remains, so the limiting orbit is circular. The convergence is asymptotic; boundedness is needed because a physical solution could otherwise reach $u=0$ and escape rather than complete indefinitely many turns.

<a id="11c/image-bounded-inverse-square-orbit-with-radial-drag-approaching-a-circular-orbit-with-nonincreasing-energy-converging-to-the-circular-orbit-value"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4-radial-drag.png)

**[Figure 1](#11c/image-bounded-inverse-square-orbit-with-radial-drag-approaching-a-circular-orbit-with-nonincreasing-energy-converging-to-the-circular-orbit-value). Bounded inverse-square orbit with radial drag approaching a circular orbit, with nonincreasing energy converging to the circular-orbit value**.

The example uses $p=h=1$, $k=0.6$ and $u(\theta)=1+0.35e^{-0.3\theta}\cos(\sqrt{0.91}\theta)$, which stays positive. Radial oscillations decay while [angular momentum](../../../../../angular-momentum.md) stays fixed.

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
