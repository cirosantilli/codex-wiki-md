<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [complexification of a Lie algebra](../../../../../complexification-of-a-lie-algebra.md) $L_0$ is $L=L_0\otimes_{\mathbb R}\mathbb C$, with the [Lie bracket](../../../../../lie-bracket.md) extended complex-bilinearly. Equivalently write $L=L_0\oplus iL_0$, where

$$
[x+iy,z+iw]=[x,z]-[y,w]+i([x,w]+[y,z]).
$$

Complex conjugation is an [antilinear map](../../../../../antilinear-map.md) and a [Lie algebra automorphism](../../../../../automorphism-of-a-lie-algebra.md) whose fixed subalgebra is $L_0$.

If the [solvable radical](../../../../../radical-of-a-lie-algebra.md) of $L_0$ is nonzero, its complexification is a nonzero solvable ideal of $L$. Conversely the [solvable radical](../../../../../radical-of-a-lie-algebra.md) $R$ of $L$ is preserved by [complex conjugation](../../../../../complex-conjugation.md), because it is the unique largest solvable ideal. Consequently

$$
R=R_0\oplus iR_0,\qquad R_0=R\cap L_0:
$$

for $z\in R$, both $(z+\overline z)/2$ and $(z-\overline z)/(2i)$ belong to $R_0$. If $R\ne0$, $R_0\ne0$ is a solvable ideal of $L_0$. This proves **$L_0$ is semisimple if and only if $L_0\otimes_{\mathbb R}\mathbb C$ is semisimple**. Consistently, the complex [Killing form](../../../../../killing-form.md) is just the complex-bilinear extension of the real one; its determinant in a real [basis](../../../../../basis.md) is unchanged by extending scalars.

Take the [sl2R Lie algebra](../../../../../sl2r-lie-algebra.md) $\mathfrak{sl}_2(\mathbb R)$ and the [special unitary Lie algebra](../../../../../special-unitary-lie-algebra.md) $\mathfrak{su}(2)$. Both complexify to $\mathfrak{sl}_2(\mathbb C)$. This is immediate for the former; for the latter, the real [basis](../../../../../basis.md) $ih,e-f,i(e+f)$ consists of [traceless matrices](../../../../../traceless-matrix.md) that are [skew-Hermitian matrices](../../../../../skew-hermitian-matrix.md) and is also a complex [basis](../../../../../basis.md) of $\mathfrak{sl}_2(\mathbb C)$.

They are not isomorphic as real [Lie algebras](../../../../../lie-algebra-split.md). Their [Killing forms](../../../../../killing-form.md) are $B(X,Y)=4\operatorname{tr}(XY)$, but on $\mathfrak{su}(2)$ this is negative definite. On $\mathfrak{sl}_2(\mathbb R)$ the [basis](../../../../../basis.md) $h,e+f,e-f$ has a diagonal [Gram matrix](../../../../../gram-matrix.md) with entries $8,8,-8$, so the [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) is $(2,1)$. A [Lie algebra isomorphism](../../../../../lie-algebra-isomorphism.md) preserves the [Killing form](../../../../../killing-form.md) and therefore its [signature](../../../../../signature-of-a-quadratic-form.md).

A real [split semisimple Lie algebra](../../../../../split-semisimple-lie-algebra.md) has a [Cartan subalgebra](../../../../../cartan-subalgebra.md) whose [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) is simultaneously diagonalizable over $\mathbb R$, so its [root-space decomposition](../../../../../root-space-decomposition.md) is defined over $\mathbb R$. The example $\mathfrak{sl}_2(\mathbb R)$ is split: the diagonal [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathbb Rh$ has [eigenvalues](../../../../../eigenvalue.md) $0,2,-2$ and real [root spaces](../../../../../root-space.md) $\mathbb Re,\mathbb Rf$. The example $\mathfrak{su}(2)$ is not split. Invariance makes every $\operatorname{ad}x$ skew-adjoint for the positive definite [inner product](../../../../../inner-product.md) $-B$, so its [eigenvalues](../../../../../eigenvalue.md) are purely imaginary. If it were diagonalizable over $\mathbb R$, all these eigenvalues would be zero and $\operatorname{ad}x=0$. The center is zero, so only $x=0$ has this property; no nonzero split [Cartan subalgebra](../../../../../cartan-subalgebra.md) exists. Thus **$\mathfrak{sl}_2(\mathbb R)$ is split and $\mathfrak{su}(2)$ is not**.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
