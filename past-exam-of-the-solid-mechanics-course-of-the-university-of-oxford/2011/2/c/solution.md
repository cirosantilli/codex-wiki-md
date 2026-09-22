<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $R=|x|>0$, $DR=\theta$ and $D\theta=(I-\theta\otimes\theta)/R$. Differentiating the [spherically symmetric deformation](../../../../spherically-symmetric-deformation.md) gives

$$
\boxed{F=r'(R)\theta\otimes\theta+\frac{r(R)}R(I-\theta\otimes\theta).}
$$

For an orientation-preserving [spherically symmetric deformation](../../../../spherically-symmetric-deformation.md) with positive radius, $r>0$ and $r'>0$. The radial direction and its perpendicular plane are [eigenspaces](../../../../eigenspace.md) of this positive [symmetric matrix](../../../../symmetric-matrix.md), so

$$
\boxed{\lambda_1=r'(R),\qquad\lambda_2=\lambda_3=r(R)/R.}
$$

At a positive [diagonal matrix](../../../../diagonal-matrix.md) $D$, every diagonal [rotation](../../../../rotation-mathematics.md) with two minus signs commutes with $D$. The supplied equivariance relation therefore forces $\widehat T(D)$ to be a [diagonal matrix](../../../../diagonal-matrix.md): each off-diagonal entry changes sign under one such [rotation](../../../../rotation-mathematics.md) while $D$ stays fixed. Varying a positive diagonal entry shows that the diagonal entries of $\widehat T(D)$ are $\Phi_{,j}$. [Permutation](../../../../permutation.md) [symmetry](../../../../symmetry-physics.md) of $\Phi$ implies $\Phi_{,2}=\Phi_{,3}$ when $\lambda_2=\lambda_3$.

Choose a [rotation](../../../../rotation-mathematics.md) whose first column is $\theta$. Applying equivariance to $F=QDQ^T$ now gives

$$
\boxed{T=\Phi_{,1}\theta\otimes\theta+\Phi_{,2}(I-\theta\otimes\theta),}
$$

with the [derivatives](../../../../derivative.md) evaluated at $(r',r/R,r/R)$. Thus the [stress](../../../../stress.md) has one radial and one repeated tangential principal value, independently of the choice of tangent basis.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
