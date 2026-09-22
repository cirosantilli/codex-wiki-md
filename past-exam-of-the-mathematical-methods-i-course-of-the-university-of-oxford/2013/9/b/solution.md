<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [symmetric part](../../../../symmetric-part-of-a-matrix.md) of the displayed matrix is

$$
M=\begin{pmatrix}5&0&2\\0&1&0\\2&0&2\end{pmatrix}.
$$

It equals the matrix of [8](../../8.md) plus $3I$, so the same [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) gives [eigenvalues](../../../../eigenvalue.md) $6,1,1$. In coordinates $u,v,w$ along $\mathbf v_3,\mathbf v_{-2},\mathbf e_2$, respectively, the level set is

$$
6u^2+v^2+w^2=6,\qquad
\boxed{\frac{u^2}{1^2}+\frac{v^2}{(\sqrt6)^2}+\frac{w^2}{(\sqrt6)^2}=1.}
$$

All three [eigenvalues](../../../../eigenvalue.md) are positive, so this is an [ellipsoid](../../../../ellipsoid.md) with semi-axis lengths $1,\sqrt6,\sqrt6$. The short axis is along $(2,0,1)$, and the plane of the longest axes is $2x_1+x_3=0$.

A natural longest-axis direction in the $x_1x_3$ plane is $\mathbf v_{-2}=(1,0,-2)/\sqrt5$. The angle $\eta$ of a unit vector to the plane $x_1=0$ has $\sin\eta=|v_1|$, giving

$$
\boxed{\eta=\arcsin\frac1{\sqrt5}=\arctan\frac12\simeq26.565^\circ}
$$

for that choice. **Degeneracy qualification:** the two longest semi-axes are equal, so “the longest axis” does not specify a unique direction. The equally valid longest axis $\mathbf e_2$ lies in $x_1=0$ and has angle zero. Generally $\mathbf v=\cos\psi\,\mathbf v_{-2}+\sin\psi\,\mathbf e_2$ is a longest-axis unit vector, with

$$
\boxed{\eta(\psi)=\arcsin\left(\frac{|\cos\psi|}{\sqrt5}\right),\qquad
0\le\eta\le\arctan\frac12.}
$$

This is the [principal-axis freedom in a repeated ellipsoid eigenspace](../../../../principal-axis-freedom-in-a-repeated-ellipsoid-eigenspace.md); a unique answer needs an extra axis-selection convention.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
