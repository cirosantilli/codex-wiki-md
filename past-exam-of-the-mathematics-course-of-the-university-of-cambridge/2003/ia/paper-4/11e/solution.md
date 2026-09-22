<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The [parallel axis theorem](../../../../../parallel-axis-theorem.md) states $I_O=I_G+md^2$ for two parallel axes, one through the [centre of mass](../../../../../center-of-mass.md) and the other a perpendicular distance $d$ away. To see this, expand the squared distance to the translated axis in the [mass](../../../../../mass.md) integral; its mixed term vanishes because the centroidal first moment is zero.

For a uniform solid hemisphere, the moment about a diameter in its flat face is half the corresponding full-sphere moment. With full-sphere [mass](../../../../../mass.md) $2m$, it is $\tfrac12[\tfrac25(2m)a^2]=2ma^2/5$. The original PDF gives the centroidal displacement $d=3a/8$; the TeX's $3a/5$ is incorrect. Moving the diameter axis to its parallel centroidal axis therefore yields

$$
\boxed{I_G=\frac25ma^2-m\left(\frac{3a}{8}\right)^2=\frac{83}{320}ma^2}.
$$

This is the [moment of inertia of a uniform solid hemisphere](../../../../../moment-of-inertia-of-a-uniform-solid-hemisphere.md), not that of a thin hemispherical shell.

Take a cross-section perpendicular to the rotation axis. Let $O$ be the underlying sphere centre, $G$ the [centre of mass](../../../../../center-of-mass.md) and $P$ the contact point. During rounded-surface contact, $OP=a$ vertically and $OG=d$ points toward the curved face, with downward component $d\cos\theta$. Therefore

$$
y_G=a-d\cos\theta,\qquad b^2=GP^2=a^2+d^2-2ad\cos\theta.
$$

For [rolling without slipping](../../../../../rolling-without-slipping.md), $P$ is instantaneously at rest and the body rotates about it with angular [speed](../../../../../speed.md) $|\dot\theta|$. Thus **the centroid [speed](../../../../../speed.md) is $b|\dot\theta|$**. Translation and rotation contribute

$$
K=\frac12mb^2\dot\theta^2+\frac12I_G\dot\theta^2=\frac12ma^2\left(\frac75-\frac34\cos\theta\right)\dot\theta^2,\qquad V=mg\left(a-\frac{3a}{8}\cos\theta\right).
$$

The initial vertical base has $\theta=\pi/2$ and $K=0$, so conserved [energy](../../../../../energy.md) is $mga$. Equating the later $K+V$ to this value gives

$$
\boxed{\dot\theta^2=\frac{15g\cos\theta}{a(28-15\cos\theta)}}.
$$

On the initial roll toward the lowest centroid position, $\dot\theta<0$. Static contact friction does no work because the contacting material point is at rest; its coefficient must be large enough for the assumed no-slip motion. The formula describes the rounded-contact phase of the [rolling uniform solid hemisphere](../../../../../rolling-uniform-solid-hemisphere.md) and should not be continued through a change of contact geometry without another model.

<a id="11e/image-rolling-hemisphere-centroid-and-contact-geometry-and-scattering-under-a-repulsive-inverse-cube-force"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4-rolling-and-orbit.png)

**[Figure 1](#11e/image-rolling-hemisphere-centroid-and-contact-geometry-and-scattering-under-a-repulsive-inverse-cube-force). Rolling hemisphere centroid and contact geometry, and scattering under a repulsive inverse-cube force**.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
