<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrate axial force balance $\nabla\cdot\sigma=0$ over the fluid between the two remote tube sections, excluding the particle. The wall's axial [traction](../../../../../../traction.md) contributes

$$
a\int_{x_1}^{x_2}\int_0^{2\pi}\sigma_{rx}(a,\theta,x)d\theta dx.
$$

At each remote section the [Hagen-Poiseuille flow](../../../../../../hagen-poiseuille-equation.md) has $u_x$ independent of $x$, so $\sigma_{xx}=-p$. The downstream and upstream caps therefore contribute $-\pi a^2p(x_2)+\pi a^2p(x_1)$. The particle contributes zero net axial force because it is [force-free](../../../../../../force-free.md). Adding the three contributions proves the [wall-shear and pressure-drop balance in a tube](../../../../../../wall-shear-and-pressure-drop-balance-in-a-tube.md):

$$
\boxed{a\int_{x_1}^{x_2}\int_0^{2\pi}\sigma_{rx}(a,\theta,x)d\theta dx
=\pi a^2[p(x_2)-p(x_1)].}
$$

Here $p$ is the physical pressure. The sign follows from the outward normals on the two caps; no convention for a positive pressure-drop magnitude has yet been introduced.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
