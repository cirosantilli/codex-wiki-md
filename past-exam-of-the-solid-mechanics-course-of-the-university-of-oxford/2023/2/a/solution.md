<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [radial unit vector in spherical coordinates](../../../../radial-unit-vector-in-spherical-coordinates.md) is $\mathbf e_R=\mathbf X/R$, so $\mathbf X\otimes\mathbf X/R^2=\mathbf e_R\otimes\mathbf e_R$. The [identity matrix](../../../../identity-matrix.md) is the sum of the three basis [outer products](../../../../outer-product.md). Substitution in the given [deformation gradient](../../../../deformation-gradient.md) gives

$$
\mathbf F=f'(R)\mathbf e_R\otimes\mathbf e_R
+\frac{f(R)}R\left(\mathbf e_\Theta\otimes\mathbf e_\Theta
+\mathbf e_\Phi\otimes\mathbf e_\Phi\right)
=\operatorname{diag}\left(f'(R),\frac{f(R)}R,\frac{f(R)}R\right).
$$

The reference and current radial directions coincide for this [spherically symmetric deformation](../../../../spherically-symmetric-deformation.md). The positive [principal stretches](../../../../principal-stretch.md) are therefore $\lambda_r=f'(R)$ and $\lambda_\theta=\lambda_\phi=f(R)/R$. [Incompressibility](../../../../incompressible-flow.md) imposes

$$
f'(R)\frac{f(R)^2}{R^2}=1,
\qquad \frac{d}{dR}f(R)^3=3R^2.
$$

Integrating and using $f(A)=a$ gives

$$
\boxed{r=f(R)=\left(R^3+a^3-A^3\right)^{1/3},\qquad
b^3=B^3+a^3-A^3.}
$$

In particular $b^3-a^3=B^3-A^3$, expressing conservation of shell [volume](../../../../volume.md). Writing $\lambda=r/R$ also gives $\lambda_r=\lambda^{-2}$ and $\lambda_\theta=\lambda_\phi=\lambda$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
