<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By part (b), $M=S^n/\Gamma$, where the group of [deck transformations](../../../../../../deck-transformation.md) acts freely by round [isometries](../../../../../../isometry.md). Every round [isometry](../../../../../../isometry.md) is the restriction of an [orthogonal transformation](../../../../../../orthogonal-transformation.md) of $\mathbb R^{n+1}$: it preserves the inner product $\langle x,y\rangle=\cos d(x,y)$, so its images of an orthonormal basis determine its linear extension.

Suppose $n$ is even. Every $A\in SO(n+1)$ has eigenvalue one. Indeed, the nonreal [eigenvalues](../../../../../../eigenvalue.md) come in conjugate pairs with product one, while the remaining real eigenvalues are $\pm1$. Their number is odd and their product is one, forcing at least one $+1$. Such a transformation fixes a unit vector. Freeness of the [deck transformation](../../../../../../deck-transformation.md) action consequently implies that the [determinant](../../../../../../determinant.md) map $\Gamma\to\{\pm1\}$ has trivial kernel. Thus $|\Gamma|\leq2$.

If $\Gamma$ is nontrivial with generator $A$, then $A^2=I$. Its eigenvalues are $\pm1$, and freeness excludes the eigenvalue $+1$. Hence $A=-I$, the antipodal [involution](../../../../../../involution.md). We obtain

$$
\boxed{M\cong S^n\quad\text{or}\quad M\cong\mathbb{RP}^n.}
$$

This proves the even-dimensional part of the [classification of complete positive constant-curvature manifolds](../../../../../../classification-of-complete-positive-constant-curvature-manifolds.md).

**The conclusion fails in odd dimensions.** For $n=2m-1\geq3$, identify $S^{2m-1}$ with the unit sphere in $\mathbb C^m$. Scalar multiplication by $\zeta=e^{2\pi i/r}$, with $r\geq3$, generates a freely acting [cyclic group](../../../../../../cyclic-group.md) of [isometries](../../../../../../isometry.md): $\zeta^jz=z$ for nonzero $z$ forces $\zeta^j=1$. The quotient is complete with constant [sectional curvature](../../../../../../sectional-curvature.md) one and has [fundamental group](../../../../../../fundamental-group.md) $C_r$, so it is neither the simply connected [sphere](../../../../../../sphere.md) nor [Real projective space](../../../../../../real-projective-space.md) with fundamental group $C_2$. In particular $S^3/C_3$ is a [lens space](../../../../../../lens-space.md) counterexample.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
