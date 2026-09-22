<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The solenoidal constraint on the [magnetic field](../../../../../../magnetic-field.md) reduces to $\partial_xB_x+\partial_zB_z=0$. Locally, or globally in a simply connected cross-section, it permits a [Cartesian magnetic flux function](../../../../../../cartesian-magnetic-flux-function.md) satisfying

$$
B_x=-\psi_z,\qquad B_z=\psi_x,\qquad
\boxed{\mathbf B=\nabla\times(\psi\mathbf e_y)+B_y\mathbf e_y.}
$$

The transverse [magnetic field lines](../../../../../../magnetic-field-line.md) are contours of $\psi$, because $\mathbf B\cdot\nabla\psi=0$. The independent component $B_y$ supplies the twist of the [flux tube](../../../../../../flux-tube.md); it is not restricted by the solenoidal constraint.

For the [Lorentz force](../../../../../../lorentz-force.md), take the [curl](../../../../../../curl.md) explicitly:

$$
\nabla\times\mathbf B
=(-B_{y,z},-\nabla^2\psi,B_{y,x}).
$$

Its [cross product](../../../../../../cross-product.md) with $\mathbf B$ has transverse components $-(\nabla^2\psi)\nabla\psi-B_y\nabla B_y$ and $y$ component $\psi_xB_{y,z}-\psi_zB_{y,x}$. Consequently

$$
\boxed{\mathbf f_L=
-\frac1{\mu_0}\left[
(\nabla^2\psi)\nabla\psi+B_y\nabla B_y+
\nabla\psi\times\nabla B_y\right].}
$$

The term $-B_y\nabla B_y/\mu_0$ is the transverse gradient of the [magnetic pressure](../../../../../../magnetic-pressure.md) associated with the axial field, while the other terms include [magnetic tension](../../../../../../magnetic-tension.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
