<h1 id="25i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $(e_1,e_2)$ of $T_pS$ and write $e(\theta)=\cos\theta\,e_1+\sin\theta\,e_2$. On a punctured disc on which the [exponential map](../../../../../../exponential-map-riemannian-geometry.md) is a [diffeomorphism](../../../../../../diffeomorphism.md), the map

$$
X(r,\theta)=\exp_p\bigl(r e(\theta)\bigr),
\qquad 0<r<\varepsilon,
$$

defines [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) centred at $p$. The curves $r\mapsto X(r,\theta)$ are unit-speed [geodesics](../../../../../../geodesic.md), so the first coefficient of the [first fundamental form](../../../../../../first-fundamental-form.md) is

$$
E=\langle X_r,X_r\rangle=1.
$$

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) says that radial and angular coordinate vectors are orthogonal, hence

$$
F=\langle X_r,X_\theta\rangle=0.
$$

The angular variation $J=X_\theta$ is a [Jacobi field](../../../../../../jacobi-field.md) along each radial geodesic, with initial data

$$
J(0)=0,
\qquad
D_rJ(0)=e'(\theta),
\qquad |e'(\theta)|=1.
$$

Since $G=\langle X_\theta,X_\theta\rangle=|J|^2$, smooth dependence of the [geodesic flow](../../../../../../geodesic-flow.md) gives

$$
\sqrt{G(r,\theta)}=|J(r)|=r+o(r).
$$

Consequently

$$
\lim_{r\to0}G(r,\theta)=0,
\qquad
\lim_{r\to0}(\sqrt G)_r(r,\theta)=1,
$$

as required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
