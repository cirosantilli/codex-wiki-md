<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Let the uniform [mass density](../../../../../density.md) be $\rho=3M/(4\pi a^3)$. In [spherical polar coordinates](../../../../../spherical-coordinate-system.md) about the rotation axis, the perpendicular distance is $r\sin\theta$ and the volume element is $r^2\sin\theta\,dr\,d\theta\,d\phi$. The [moment of inertia](../../../../../moment-of-inertia.md) is therefore

$$
I=\rho\int_0^a r^4\,dr\int_0^\pi\sin^3\theta\,d\theta\int_0^{2\pi}d\phi=\frac{8\pi\rho a^5}{15}=\boxed{\frac25Ma^2}.
$$

In the given [rigid body](../../../../../rigid-body-dynamics.md) [kinetic energy](../../../../../kinetic-energy.md) decomposition, $\tfrac12M|\dot{\mathbf R}|^2$ is the translational [kinetic energy](../../../../../kinetic-energy.md) of the whole mass moving at its [center of mass](../../../../../center-of-mass.md) velocity. The term $\tfrac12I\omega^2$ is the rotational [kinetic energy](../../../../../kinetic-energy.md) about the [center of mass](../../../../../center-of-mass.md). The mixed term vanishes because the mass-weighted relative positions sum to zero.

For [rolling without slipping](../../../../../rolling-without-slipping.md), the point of contact has zero instantaneous velocity relative to the stationary surface. Its rotational velocity is opposite the [center of mass](../../../../../center-of-mass.md) velocity and has magnitude $a|\omega|$. Hence $V=a|\omega|$. Substituting this and the [moment of inertia of a uniform solid sphere](../../../../../moment-of-inertia-of-a-uniform-solid-sphere.md) gives

$$
\boxed{T=\frac12MV^2+\frac12\left(\frac25Ma^2\right)\frac{V^2}{a^2}=\frac7{10}MV^2.}
$$

The rotational axis is through the [center of mass](../../../../../center-of-mass.md) and parallel to the surface, perpendicular to the direction of rolling.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
