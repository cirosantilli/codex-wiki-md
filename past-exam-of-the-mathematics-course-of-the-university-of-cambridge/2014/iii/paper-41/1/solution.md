<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [Lie bracket](../../../../../lie-bracket.md) over $\mathbb R$ or $\mathbb C$, [antisymmetry of a Lie bracket](../../../../../antisymmetry-of-a-lie-bracket.md) means $[x,y]=-[y,x]$. In particular $[x,x]=0$ in these characteristic-zero fields. The [Jacobi identity](../../../../../jacobi-identity.md) is

$$
\boxed{[x,[y,z]]+[y,[z,x]]+[z,[x,y]]=0.}
$$

It expresses compatibility of the bracket with its own adjoint action. Bilinearity must hold over the chosen base field, and the bracket must take its values in the same [vector space](../../../../../vector-space-split.md).

For the [matrix](../../../../../matrix.md) [commutator](../../../../../commutator.md), bilinearity and antisymmetry follow directly from distributivity. Associativity of [matrix](../../../../../matrix.md) multiplication gives

$$
[A,[B,C]]=ABC-ACB-BCA+CBA;
$$

adding the two cyclic permutations cancels every monomial. Thus the [Jacobi identity](../../../../../jacobi-identity.md) holds in the entire [matrix](../../../../../matrix.md) algebra. For a specified linear subspace, the only additional bracket condition is **closure: $AB-BA$ must belong to the subspace whenever $A,B$ do**. It is unnecessary to require closure under the separate products $AB$ and $BA$.

To determine the [special unitary Lie algebra](../../../../../special-unitary-lie-algebra.md), let $g(t)$ be a differentiable curve in the [special unitary group](../../../../../special-unitary-group.md) with $g(0)=I$ and $A=g'(0)$. Differentiating $g(t)^\dagger g(t)=I$ gives $A^\dagger+A=0$. Differentiating $\det g(t)=1$ at the identity gives $\operatorname{tr}A=0$. Conversely a traceless [skew-Hermitian matrix](../../../../../skew-hermitian-matrix.md) has $e^{tA}$ unitary and $\det e^{tA}=e^{t\operatorname{tr}A}=1$, so it really is a tangent vector. Therefore

$$
\boxed{\mathfrak{su}(n)=\{A\in M_n(\mathbb C):A^\dagger=-A,\ \operatorname{tr}A=0\},
\qquad \dim_{\mathbb R}\mathfrak{su}(n)=n^2-1.}
$$

This is a real [Lie algebra](../../../../../lie-algebra-split.md) of complex [matrices](../../../../../matrix.md): multiplication by $i$ generally leaves this real subspace. Its complexification is $\mathfrak{sl}_n(\mathbb C)$, not the compact algebra itself. For $A,B\in\mathfrak{su}(n)$,

$$
[A,B]^\dagger=B^\dagger A^\dagger-A^\dagger B^\dagger=BA-AB=-[A,B],
\qquad \operatorname{tr}[A,B]=0.
$$

Thus closure holds, and the already verified [commutator](../../../../../commutator.md) identities establish all the [Lie algebra](../../../../../lie-algebra-split.md) axioms.

The [cross-product Lie algebra](../../../../../cross-product-lie-algebra.md) on $\mathbb R^3$ is bilinear, antisymmetric and closed because the [cross product](../../../../../cross-product.md) has those properties. Its [Jacobi identity](../../../../../jacobi-identity.md) follows from the vector triple-product identity:

$$
\mathbf x\times(\mathbf y\times\mathbf z)
=\mathbf y(\mathbf x\cdot\mathbf z)-\mathbf z(\mathbf x\cdot\mathbf y).
$$

In the cyclic sum, the coefficients cancel by symmetry of the scalar product.

For the explicit relation to the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md), take the three [Pauli matrices](../../../../../pauli-matrices.md) and define

$$
F(\mathbf x)=-\frac{i}{2}\sum_{a=1}^3x_a\sigma_a.
$$

These [matrices](../../../../../matrix.md) are traceless and [Skew-Hermitian](../../../../../skew-hermitian-matrix.md), and the three images of the standard basis form a real basis of $\mathfrak{su}(2)$. Using the [Pauli matrix commutator identity](../../../../../pauli-matrix-commutator-identity.md),

$$
[F(\mathbf x),F(\mathbf y)]
=-\frac14\,2i\sum_c(\mathbf x\times\mathbf y)_c\sigma_c
=F(\mathbf x\times\mathbf y).
$$

Hence **$F$ is a real [Lie algebra isomorphism](../../../../../lie-algebra-isomorphism.md)**. The factor and sign $-i/2$ are essential for preserving the unscaled cross-product bracket. At the group level there is an [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md); the isomorphism of their tangent algebras does not identify the two global groups.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
