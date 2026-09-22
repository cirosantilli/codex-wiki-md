<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reflection symmetry of the cube in each coordinate plane makes every off-diagonal integral

$$
-\rho\int_Bx_ix_j\,dV\qquad(i\ne j)
$$

vanish because its integrand is [odd](../../../../../../odd-function.md) in one coordinate. Permuting the three coordinate axes leaves the cube unchanged, so its three diagonal moments are equal. Thus its [inertia tensor](../../../../../../inertia-tensor.md) at the centre has the isotropic form

$$
I_{ij}(\mathbf0)=\lambda\delta_{ij}.
$$

For

$$
\mathbf a=\frac\ell2(1,1,0),
\qquad
|\mathbf a|^2=\frac{\ell^2}{2},
$$

part (a) and $\lambda=M\ell^2/6$ give

$$
\boxed{
I(\mathbf a)
=\frac{M\ell^2}{12}
\begin{pmatrix}
5&-3&0\\
-3&5&0\\
0&0&8
\end{pmatrix}}.
$$

The displayed symmetric matrix has orthogonal [eigenvectors](../../../../../../eigenvector.md)

$$
(1,1,0),\qquad(1,-1,0),\qquad(0,0,1)
$$

with corresponding [eigenvalues](../../../../../../eigenvalue.md)

$$
\frac{M\ell^2}{6},
\qquad
\frac{2M\ell^2}{3},
\qquad
\frac{2M\ell^2}{3}.
$$

For a unit angular velocity, $|\mathbf L|=|I\boldsymbol\omega|$ is minimized and maximized along eigenvectors for the smallest and largest eigenvalues. Their ratio is

$$
\boxed{
\frac{|\mathbf L|_{\max}}{|\mathbf L|_{\min}}
=\frac{2M\ell^2/3}{M\ell^2/6}=4}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
