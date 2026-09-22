<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [isotropic tensor](../../../../isotropic-tensor.md) has unchanged components under every rotation of the Cartesian axes. Under proper rotations in three dimensions, rank one has **no nonzero isotropic tensor**, rank two has $\boxed{T_{ij}=A\delta_{ij}}$, and rank three has $\boxed{T_{ijk}=B\epsilon_{ijk}}$. Here $\delta$ is the [Kronecker delta](../../../../kronecker-delta.md) and $\epsilon$ the [Levi-Civita symbol](../../../../levi-civita-symbol.md). If invariance under reflections is also required for a true tensor, the rank-three case vanishes; $\epsilon$ is then a pseudotensor.

The [velocity gradient tensor](../../../../velocity-gradient-tensor.md) for the given field is

$$
D_{ik}=\frac{\partial u_i}{\partial x_k}=\begin{pmatrix}x_2^2&2x_1x_2&0\\0&x_3^2&2x_2x_3\\2x_1x_3&0&x_1^2\end{pmatrix}.
$$

Its symmetric part, the [strain-rate tensor](../../../../strain-rate-tensor.md) if $\mathbf u$ is interpreted as a velocity, is

$$
\boxed{e=\frac{D+D^T}{2}=\begin{pmatrix}x_2^2&x_1x_2&x_1x_3\\x_1x_2&x_3^2&x_2x_3\\x_1x_3&x_2x_3&x_1^2\end{pmatrix}.}
$$

The antisymmetric part has the specified ordering $D_{ik}-e_{ik}=\epsilon_{ijk}\omega_j$, with

$$
\boxed{\boldsymbol\omega=\tfrac12\nabla\times\mathbf u=(-x_2x_3,-x_1x_3,-x_1x_2).}
$$

The index ordering matters for this sign; it agrees with a local rotation velocity $\boldsymbol\omega\times\mathbf x$. This is the axial part of the [scalar, symmetric-traceless and axial tensor decomposition](../../../../scalar-symmetric-traceless-and-axial-tensor-decomposition.md), retaining the trace inside the symmetric part here.

At the specified point, $e=\begin{pmatrix}9&6&0\\6&0&0\\0&0&4\end{pmatrix}$. The upper block has characteristic polynomial $\lambda^2-9\lambda-36=(\lambda-12)(\lambda+3)$. Thus the principal values and unit [eigenvectors](../../../../eigenvector.md) are

$$
\boxed{12:\ \frac{(2,1,0)}{\sqrt5};\qquad -3:\ \frac{(1,-2,0)}{\sqrt5};\qquad 4:\ (0,0,1).}
$$

These mutually orthogonal directions are the [principal strain rates](../../../../principal-strain-rates.md)' axes for this local field; reversing an eigenvector does not change its axis.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
