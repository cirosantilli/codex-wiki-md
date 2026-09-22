<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the angular dependence as $f(\phi)=\sum_{n\ge1}a_n\sin n\phi+\sum_{n\ge0}b_n\cos n\phi$, so $u'=\sin\theta f(\phi)e_\phi$. In the [spherical coordinate system](../../../../../../spherical-coordinate-system.md), $n=e_r$ and $e_r\times e_\phi=-e_\theta$, with

$$
e_\theta=(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\qquad
 dS=a^2\sin\theta\,d\theta\,d\phi.
$$

Thus the integral in the [torque-free rotation of a spherical squirmer](../../../../../../torque-free-rotation-of-a-spherical-squirmer.md) has components

$$
I_x=-a^2\left(\int_0^\pi\sin^2\theta\cos\theta d\theta\right)
\left(\int_0^{2\pi}f(\phi)\cos\phi d\phi\right)=0,
$$



$$
I_y=-a^2\left(\int_0^\pi\sin^2\theta\cos\theta d\theta\right)
\left(\int_0^{2\pi}f(\phi)\sin\phi d\phi\right)=0.
$$

The vanishing follows from north-south cancellation, including the potentially relevant first azimuthal harmonics. In the $z$ direction, [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md) gives

$$
I_z=a^2\int_0^\pi\sin^3\theta d\theta\int_0^{2\pi}f(\phi)d\phi
=a^2\frac43(2\pi b_0)=\frac{8\pi a^2}{3}b_0.
$$

Consequently every rotational component is determined:

$$
\boxed{\Omega_x=0,\qquad\Omega_y=0,\qquad\Omega_z=-\frac{b_0}{a}.}
$$

This assumes an integrable prescribed angular function, with the Fourier series convergent sufficiently to justify the surface integrals; a finite Fourier sum is enough for the construction below. Other harmonics can generate exterior flows even though they contribute no net rotation.

For [flow-free rotation of a spherical squirmer](../../../../../../flow-free-rotation-of-a-spherical-squirmer.md), choose $b_0\ne0$ and set every $a_n$ and every $b_n$ with $n\ge1$ to zero. Then $u'=b_0\sin\theta e_\phi$, while the rigid-rotation velocity is

$$
\Omega\times an=-b_0\sin\theta e_\phi=-u'.
$$

The total laboratory-frame boundary velocity is therefore zero everywhere. With fluid at rest at infinity, [Uniqueness of Stokes flow](../../../../../../uniqueness-of-stokes-flow.md) gives

$$
\boxed{u(r)=0\quad\text{throughout the exterior fluid, although }\Omega_z=-b_0/a\ne0.}
$$

A constant pressure supplies zero resultant force and torque, so this is consistent with free motion. The imposed surface actuation counter-rotates relative to the material sphere; no claim is being made that ordinary no-slip rigid rotation produces zero flow.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
