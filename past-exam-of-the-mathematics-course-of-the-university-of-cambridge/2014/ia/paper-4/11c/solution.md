<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

The area element in [plane polar coordinates](../../../../../plane-polar-coordinates.md) is $r\,dr\,d\theta$. Thus the axial [moment of inertia](../../../../../moment-of-inertia.md) is

$$
I_0=\int_0^{2\pi}\int_0^a r^2\rho_0(a-r)r\,dr\,d\theta
=2\pi\rho_0\left[\frac{ar^4}{4}-\frac{r^5}{5}\right]_0^a
=\boxed{\frac{\pi\rho_0a^5}{10}}.
$$

For the removed material, the angular width is $2\pi/13$, and

$$
\int_{a/2}^a r^3(a-r)\,dr=\frac{13a^5}{320}.
$$

Its [moment of inertia](../../../../../moment-of-inertia.md) is therefore $I_{\rm cut}=\pi\rho_0a^5/160$, leaving

$$
I=I_0-I_{\rm cut}=\frac{3\pi\rho_0a^5}{32}.
$$

The [torque](../../../../../torque.md) equation $I\dot\Omega=\tau$ gives constant [angular acceleration](../../../../../angular-acceleration.md), so the time to reach the prescribed [angular speed](../../../../../angular-speed.md) from rest is

$$
\boxed{t=\frac{I\Omega}{\tau}=\frac{3\pi\rho_0a^5\Omega}{32\tau}.}
$$

To find the [centre of mass after removing material](../../../../../centre-of-mass-after-removing-material.md), let $\mathbf e_1$ point along the bisector of the missing sector in the disc. The original disc has zero first [mass](../../../../../mass.md) moment about its centre. The missing sector has zero transverse first moment by reflection symmetry, while its component along $\mathbf e_1$ is

$$
Q_{\rm cut}=\rho_0\int_{a/2}^a r^2(a-r)\,dr\int_{-\pi/13}^{\pi/13}\cos\theta\,d\theta
=\frac{11\rho_0a^4}{96}\sin\frac\pi{13},
$$

because the radial integral is $11a^4/192$. The remaining first moment is $-Q_{\rm cut}\mathbf e_1$. Dividing by the given [mass](../../../../../mass.md) $k\rho_0a^3$ gives the body-fixed [centre of mass](../../../../../center-of-mass.md)

$$
\boxed{\mathbf R=-\frac{11a}{96k}\sin\frac\pi{13}\,\mathbf e_1.}
$$

It lies away from the missing sector. In the inertial frame, let $t_*$ be the moment the applied [torque](../../../../../torque.md) stops and let $\psi=\psi_*+\Omega(t-t_*)$ give the orientation of that sector's bisector. Then, with $d=11a\sin(\pi/13)/(96k)$,

$$
\mathbf R(t)=-d(\cos\psi,\sin\psi,0),\qquad\boxed{\ddot{\mathbf R}=-\Omega^2\mathbf R}.
$$

The [centre of mass](../../../../../center-of-mass.md) has inward [centripetal acceleration](../../../../../centripetal-acceleration.md) of magnitude $\Omega^2d$. **The required real [force](../../../../../force.md) is the constraint reaction exerted by the fixed rod and its support**. Its horizontal resultant is $k\rho_0a^3\ddot{\mathbf R}$; a zero applied axial [torque](../../../../../torque.md) does not imply a zero resultant [force](../../../../../force.md).

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
