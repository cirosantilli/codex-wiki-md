<h1 id="18f/solution">Solution</h1>

↑ **Parent:** [18F](../18f.md)

The squared Vandermonde product defining the [polynomial discriminant](../../../../../polynomial-discriminant.md) is symmetric in all roots. By the fundamental theorem of [symmetric polynomials](../../../../../symmetric-polynomial.md), it is a [polynomial](../../../../../polynomial-split.md) in the elementary symmetric functions, which are the signed coefficients of the monic [polynomial](../../../../../polynomial-split.md). Hence it is a [polynomial](../../../../../polynomial-split.md) function of those coefficients over the base field.

For $f=X^3+pX+q$, $\Delta(f)=-\operatorname{Res}(f,f')$. Eliminating the two leading rows in the Sylvester determinant reduces the resultant to

$$
\operatorname{Res}(f,f')=\det\begin{pmatrix}-2p&-3q&0\\0&-2p&-3q\\3&0&p\end{pmatrix}
=4p^3+27q^2.
$$

Thus

$$
\boxed{\Delta(X^3+pX+q)=-4p^3-27q^2.}
$$

For $X^3-3X+1$, the only possible rational roots are $\pm1$, and neither is a root. The cubic is therefore irreducible, so its [Galois group](../../../../../galois-group.md) is a transitive subgroup of $S_3$. Its discriminant is $81=9^2$. The Vandermonde product changes sign under odd permutations, and its square being a rational square implies that the product itself is rational; hence all Galois permutations are even. The only transitive subgroup of $A_3$ is $A_3$ itself. Consequently, writing $L$ for its splitting field,

$$
\boxed{\operatorname{Gal}(L/\mathbb Q)\cong C_3.}
$$

## ↑ Ancestors (10)

1. [18F](../18f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
