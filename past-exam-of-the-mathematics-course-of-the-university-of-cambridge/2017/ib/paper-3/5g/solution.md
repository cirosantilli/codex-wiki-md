<h1 id="5g/solution">Solution</h1>

↑ **Parent:** [5G](../5g.md)

Write $w$ for the complex coordinate. The inverse [stereographic projection](../../../../../stereographic-projection.md) is

$$
\pi^{-1}(w)=\frac{(2\operatorname{Re}w,\,2\operatorname{Im}w,\,|w|^2-1)}{1+|w|^2},
$$

with $\infty$ mapped to the north pole. A rotation $R_z(\theta)$ about the third axis sends $w$ to $e^{i\theta}w$, represented by

$$
U_z(\theta)=\begin{pmatrix}e^{i\theta/2}&0\\0&e^{-i\theta/2}\end{pmatrix}\in SU(2).
$$

For the rotation $R_y(\theta):(x,y,z)\mapsto(x\cos\theta+z\sin\theta,y,-x\sin\theta+z\cos\theta)$, substitution in the [stereographic projection](../../../../../stereographic-projection.md) gives

$$
w\longmapsto\frac{cw-s}{sw+c},\qquad
U_y(\theta)=\begin{pmatrix}c&-s\\s&c\end{pmatrix}\in SU(2),\quad
c=\cos(\theta/2),\ s=\sin(\theta/2).
$$

Both displayed matrices are unitary with determinant one, hence belong to the [special unitary group](../../../../../special-unitary-group.md).

Use the rotation-generation result that every $R\in SO(3)$ can be written $R_z(\alpha)R_y(\beta)R_z(\gamma)$, with angles chosen suitably. This is the Euler-angle decomposition, which is allowed here. Composition of [Möbius transformations](../../../../../mobius-transformation.md) corresponds to multiplication of their matrix representatives, so

$$
\boxed{\pi R\pi^{-1}\text{ is represented by }U_z(\alpha)U_y(\beta)U_z(\gamma)\in SU(2).}
$$

The formulas extend at poles in the [Riemann sphere](../../../../../riemann-sphere.md). This realizes [sphere rotations as special-unitary Möbius transformations](../../../../../sphere-rotations-as-special-unitary-mobius-transformations.md). The two representatives $U$ and $-U$ define the same [Möbius transformation](../../../../../mobius-transformation.md), as expected for the double covering of the [special orthogonal group](../../../../../special-orthogonal-group.md).

## ↑ Ancestors (10)

1. [5G](../5g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
