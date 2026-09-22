<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

In a vacuum with no charge or current, the [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot E=0,
\qquad
\nabla\cdot B=0,
\qquad
\nabla\times E=-\frac{\partial B}{\partial t},
\qquad
\nabla\times B=\frac1{c^2}\frac{\partial E}{\partial t}.
$$

For the proposed [plane electromagnetic wave](../../../../../plane-electromagnetic-wave.md), $\nabla\cdot B=0$ gives

$$
k\cdot B_0=0.
$$

The [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) gives

$$
E_0=-\frac{c^2}{\omega}\,k\times B_0,
$$

and substituting this into [Faraday's law](../../../../../faraday-s-law-of-induction.md) gives the [dispersion relation](../../../../../dispersion-relation.md)

$$
\omega^2=c^2|k|^2.
$$

Thus both fields have [transverse polarization](../../../../../transverse-polarization.md) relative to $k$, and the corresponding real electric field is

$$
\boxed{E(x,t)=\operatorname{Re}\left[-\frac{c^2}{\omega}
(k\times B_0)e^{i(k\cdot x-\omega t)}\right]}.
$$

For incidence in the positive $x$-direction, choose the incident fields

$$
B_i=B_0\cos(kx-\omega t)e_z,
\qquad
E_i=cB_0\cos(kx-\omega t)e_y.
$$

The [perfect conductor](../../../../../perfect-conductor.md) requires the tangential electric field to vanish at $x=0$. The reflected wave therefore has

$$
B_r=B_0\cos(kx+\omega t)e_z,
\qquad
E_r=-cB_0\cos(kx+\omega t)e_y.
$$

This is [normal reflection of an electromagnetic wave from a perfect conductor](../../../../../normal-reflection-of-an-electromagnetic-wave-from-a-perfect-conductor.md). The magnetic field in $x\leq0$ is

$$
B=B_i+B_r
=2B_0\cos(kx)\cos(\omega t)e_z,
$$

so its tangential value at the surface is

$$
\boxed{B_{\rm tangential}(0,t)=2B_0\cos(\omega t)e_z}.
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
