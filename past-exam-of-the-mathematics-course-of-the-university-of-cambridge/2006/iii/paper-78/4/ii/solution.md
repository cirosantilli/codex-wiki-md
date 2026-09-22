<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Axisymmetric rotation about the offset axis gives wall [velocity](../../../../../../velocity.md) $v_\varphi=a\Omega\sin\theta$. Its azimuthal [Couette flow](../../../../../../couette-flow.md) has no pressure-driving divergence, so [pressure](../../../../../../pressure.md) remains constant. The fluid-on-inner-sphere tangential [traction](../../../../../../traction.md) is $-\mu a\Omega\sin\theta/h$. Multiply it by the moment arm $a\sin\theta$ and integrate:

$$
G_z=-\frac{2\pi\mu\Omega a^4}{\Delta}\int_{-1}^1\frac{1-z^2}{1-\alpha z}\,dz.
$$

Putting $t=\alpha z$ and using the second supplied identity with its generic parameter equal to $\alpha$ gives the [axial rotational resistance of eccentric nested spheres](../../../../../../axial-rotational-resistance-of-eccentric-nested-spheres.md):

$$
\boxed{G_z=-\frac{2\pi\mu\Omega a^4}{\Delta\alpha^3}\left[2\alpha+(1-\alpha^2)\log\frac{1-\alpha}{1+\alpha}\right].}
$$

The continuous limit at $\alpha=0$ is $-8\pi\mu\Omega a^4/(3\Delta)$, consistent with a concentric narrow spherical shell. At $\alpha\to1$, the [torque](../../../../../../torque.md) tends to $-4\pi\mu\Omega a^4/\Delta$: it remains finite because the rotational wall speed vanishes at the closest pole.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
