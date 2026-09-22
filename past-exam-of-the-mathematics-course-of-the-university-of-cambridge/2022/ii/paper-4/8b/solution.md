<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Taking downward distance as positive, the [Lagrangian](../../../../../lagrangian.md) is

$$
\boxed{
L
=\frac12(3m)\dot z_1^2+\frac12(2m)\dot z_2^2
-\frac k2(z_1-l)^2
-\frac k2(z_2-z_1-l)^2
+3mgz_1+2mgz_2
}.
$$

At equilibrium the lower spring supports only the lower mass, while the upper spring supports both masses:

$$
k(z_2-z_1-l)=2mg,
\qquad
k(z_1-l)=5mg.
$$

Hence

$$
\boxed{
z_1^{(0)}=l+\frac{5mg}{k},
\qquad
z_2^{(0)}=2l+\frac{7mg}{k}
}.
$$

Let $q_i=z_i-z_i^{(0)}$. The linear terms cancel by the equilibrium equations, and the quadratic Lagrangian is

$$
L
=\frac12\dot{\mathbf q}^{\,T}T\dot{\mathbf q}
-\frac12\mathbf q^TV\mathbf q+\text{constant},
$$

with the [small-oscillation mass and stiffness matrices](../../../../../small-oscillation-mass-and-stiffness-matrices.md)

$$
\boxed{
T=m\begin{pmatrix}3&0\\0&2\end{pmatrix},
\qquad
V=k\begin{pmatrix}2&-1\\-1&1\end{pmatrix}
}.
$$

The [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md) is

$$
(V-\omega^2T)\mathbf a=0.
$$

Its characteristic equation is

$$
\det(V-\omega^2T)
=k^2-7km\omega^2+6m^2\omega^4=0,
$$

so

$$
\boxed{
\omega_1=\sqrt{\frac{k}{6m}},
\qquad
\omega_2=\sqrt{\frac{k}{m}}
}.
$$

Corresponding displacement eigenvectors are

$$
\boxed{
\mathbf a_1=(2,3)^T,
\qquad
\mathbf a_2=(1,-1)^T
}.
$$

They are not orthogonal in the ordinary Euclidean inner product. They are orthogonal in the kinetic-energy, or mass-matrix, inner product:

$$
\boxed{
\mathbf a_1^TT\mathbf a_2
=(2,3)
m\begin{pmatrix}3&0\\0&2\end{pmatrix}
\binom{1}{-1}
=0
}.
$$

This is [mass-matrix orthogonality of normal modes](../../../../../mass-matrix-orthogonality-of-normal-modes.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
