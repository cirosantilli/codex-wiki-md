<h1 id="14e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For equal masses and springs,

$$
L_1=\ell+\frac{2mg}{k},\qquad L_2=\ell+\frac{mg}{k}.
$$

A small horizontal displacement $x_1$ changes each spring direction to first order. The equilibrium tensions $2mg$ and $mg$ give transverse restoring stiffness

$$
K_x=\frac{2mg}{L_1}+\frac{mg}{L_2}.
$$

Therefore

$$
\omega_1^2=\frac{K_x}{m}
=\frac{k}{m}\left(
2-\frac1{1+2mg/(k\ell)}
-\frac1{1+mg/(k\ell)}
\right),
$$

as required.

The other motions are vertical. If $\eta_1,\eta_2$ are downward displacements from equilibrium, their linearized equations are

$$
m\begin{pmatrix}\ddot\eta_1\\\ddot\eta_2\end{pmatrix}
=-k\begin{pmatrix}2&-1\\-1&1\end{pmatrix}
\begin{pmatrix}\eta_1\\\eta_2\end{pmatrix}.
$$

The [vertical normal modes of two equal suspended masses](../../../../../../vertical-normal-modes-of-two-equal-suspended-masses.md) are

$$
\boxed{\omega_\pm^2=\frac{k}{2m}(3\pm\sqrt5)},
\qquad
\boxed{(\eta_1,\eta_2)\propto
\left(1,\frac{1\mp\sqrt5}{2}\right)}.
$$

Neither frequency contains $g$: gravity only shifted the equilibrium lengths.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14E](../../14e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
