<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Identify a subset $A\subseteq\Omega$ with its indicator [vector](../../../../../../vector.md) $a=(a_1,\ldots,a_n)\in\mathbb F_2^n$. [Symmetric difference](../../../../../../symmetric-difference.md) becomes coordinatewise addition modulo two, so the subsets form a [vector space](../../../../../../vector-space-split.md) of dimension $n$, with the singleton subsets as a [basis](../../../../../../basis.md). The proposed form becomes the dot product

$$
B(a,b)=\sum_{i=1}^na_ib_i\in\mathbb F_2.
$$

Distributivity proves bilinearity, and commutativity proves symmetry. Its [Gram matrix](../../../../../../gram-matrix.md) in the singleton [basis](../../../../../../basis.md) is $I_n$, so it is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md). A [permutation](../../../../../../permutation.md) merely permutes coordinates and preserves the dot product, proving invariance under $S_n$.

Write $u=(1,\ldots,1)$ for the full subset. Its [bilinear orthogonal complement](../../../../../../orthogonal-complement-for-a-bilinear-form.md) $E=u^\perp$ consists exactly of even-cardinality subsets. If $n\geq2$ is even, $B(u,u)=n=0$ in $\mathbb F_2$, so $\langle u\rangle\leq E$. For any $v\in E$, $B(v,v)=\sum_iv_i^2=\sum_iv_i=0$, so the restricted form is alternating.

Nondegeneracy of the full form gives $E^\perp=\langle u\rangle$; one can also see this directly by testing against all [vectors](../../../../../../vector.md) $e_i+e_j$, which forces all coordinates of an element of $E^\perp$ to be equal. Hence the [radical of a bilinear form](../../../../../../radical-of-a-bilinear-form.md) of the restricted form is

$$
\operatorname{rad}(B|_E)=E\cap E^\perp=\langle u\rangle.
$$

Define the quotient form by $\overline B(v+\langle u\rangle,w+\langle u\rangle)=B(v,w)$. Adding $u$ to either representative does not change the pairing with $E$, so it is well-defined. It is alternating, and a class pairing to zero with all classes has a representative in $\operatorname{rad}(B|_E)=\langle u\rangle$, hence is zero. Therefore

$$
\boxed{\langle\Omega\rangle^\perp/\langle\Omega\rangle\text{ is a nondegenerate alternating space of dimension }n-2.}
$$

Both spaces are $S_n$-invariant, so the coordinate action descends and preserves the quotient form. This is the [symplectic quotient of the binary subset module](../../../../../../symplectic-quotient-of-the-binary-subset-module.md). The evenness assumption is essential because otherwise $u$ does not lie in its own [bilinear orthogonal complement](../../../../../../orthogonal-complement-for-a-bilinear-form.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
