<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

For a fixed central gravitational source, the radial and transverse components of [Newton's second law](../../../../../newton-s-second-law.md) in [polar coordinates](../../../../../polar-coordinates.md) are

$$
\ddot r-r\dot\theta^2=-\frac{GM}{r^2},\qquad
r\ddot\theta+2\dot r\dot\theta=0.
$$

The second equation gives $r^2\dot\theta=h$, the constant specific [angular momentum](../../../../../angular-momentum.md). Take $h>0$ by choosing the orientation of $\theta$, and put $u=1/r$. Writing $u'$ and $u''$ for [derivatives](../../../../../derivative.md) with respect to $\theta$,

$$
\dot r=-hu',\qquad\ddot r=-h^2u^2u'',\qquad
r\dot\theta^2=h^2u^3.
$$

Substituting into the radial equation and dividing by $-h^2u^2$ proves the [Binet equation](../../../../../binet-equation.md)

$$
\boxed{u''+u=\frac{GM}{h^2}=k.}
$$

At perihelion the [velocity](../../../../../velocity.md) is tangential. The [escape velocity](../../../../../escape-velocity.md) is $v_0=\sqrt{2GM/r_0}$, so $h=r_0v_0$ and $h^2=2GMr_0$. Consequently $k=1/(2r_0)$. The initial conditions are $u(0)=1/r_0$ and $u'(0)=0$. Solving the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) gives the [parabolic Kepler orbit](../../../../../parabolic-trajectory.md)

$$
\boxed{u(\theta)=\frac{1+\cos\theta}{2r_0}
=\frac1{r_0}\cos^2(\theta/2),\qquad
r=r_0\sec^2(\theta/2).}
$$

Using [angular momentum](../../../../../angular-momentum.md) conservation again,

$$
\dot\theta=\frac h{r^2}=\frac h{r_0^2}\cos^4(\theta/2),
\qquad\boxed{\sec^4(\theta/2)\dot\theta=\frac h{r_0^2}.}
$$

On the outgoing branch $r=2r_0$ is first reached at $\theta=\pi/2$. Integrate from release at perihelion, using $w=\tan(\theta/2)$:

$$
t=\frac{r_0^2}{h}\int_0^{\pi/2}\sec^4(\theta/2)d\theta
=\frac{2r_0^2}{h}\int_0^1(1+w^2)dw
=\boxed{\frac{8r_0^2}{3h}.}
$$

More generally the same integral gives $t=(2r_0^2/h)(w+w^3/3)$, the [Barker equation](../../../../../barker-equation.md) for this parabolic orbit.

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
