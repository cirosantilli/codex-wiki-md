<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A generic linear projection over an infinite [field](../../../../../../field.md) is not enough for the stated arbitrary [field](../../../../../../field.md) $k$. Instead use [Noether normalization by weighted substitutions](../../../../../../noether-normalization-by-weighted-substitutions.md) to make the defining polynomial monic in one coordinate.

For $n>1$, choose an integer $M$ at least every exponent occurring in a nonzero [monomial](../../../../../../monomial.md) of $f$, put $B=M+1$, and use the triangular polynomial change of variables

$$
x_i=y_i+y_n^{B^i}\quad(1\leq i<n),\qquad x_n=y_n.
$$

Here $M\geq1$ because the irreducible polynomial is nonconstant. This is an automorphism, with inverse $y_i=x_i-x_n^{B^i}$, $y_n=x_n$. A [monomial](../../../../../../monomial.md) $x_1^{\alpha_1}\cdots x_n^{\alpha_n}$ contributes a highest $y_n$ power

$$
w(\alpha)=\alpha_n+\sum_{i=1}^{n-1}\alpha_iB^i.
$$

These weights are all distinct: the exponents are base-$B$ digits bounded by $M$. All other terms in the expansion have smaller $y_n$ degree than that [monomial](../../../../../../monomial.md)'s weight. Therefore the highest-degree $y_n$ term in the transformed $f$ comes from exactly one original [monomial](../../../../../../monomial.md) and has a nonzero coefficient in $k$, independent of the other $y_i$. No assumption about the cardinality or characteristic of $k$ enters this argument.

Multiply by the inverse of that coefficient to obtain a [monic polynomial](../../../../../../monic-polynomial.md) $F\in A[y_n]$ of some degree $D>0$, where $A=k[y_1,\ldots,y_{n-1}]$. The same construction for $n=1$ simply rescales $f$ to be monic over $A=k$.

The [monic polynomial quotient is finite free](../../../../../../monic-polynomial-quotient-is-finite-free.md) because division by $F$ gives a unique representative of degree less than $D$. Thus

$$
\boxed{k[x_1,\ldots,x_n]/(f)\cong A[y_n]/(F)
\cong A\oplus Ay_n\oplus\cdots\oplus Ay_n^{D-1}}
$$

as $A$-modules. Uniqueness follows because any nonzero multiple of a monic $F$ has $y_n$ degree at least $D$. In particular the map $A\to A[y_n]/(F)$ is injective.

The induced morphism

$$
\boxed{X\longrightarrow\operatorname{Spec}A=\mathbb A_k^{n-1}}
$$

is finite, since its coordinate algebra is a finite module, and flat, since tensoring with a [finite free module](../../../../../../finite-free-module.md) is a finite [direct sum](../../../../../../direct-sum.md) of copies of the original module and preserves exactness. This is a [finite flat Noether normalization of an affine hypersurface](../../../../../../finite-flat-noether-normalization-of-an-affine-hypersurface.md), with the explicit projection coordinates $y_i=x_i-x_n^{B^i}$. The construction actually applies to any nonconstant polynomial, not only an irreducible one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
