<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

Put $C=A+yI$. For every $y$ except the finitely many roots of $\det(A+yI)$, $C$ is invertible and $CB$ is similar to $BC$, since $C^{-1}(CB)C=BC$. Hence

$$
\det(tI-(A+yI)B)=\det(tI-B(A+yI)).
$$

Both sides are polynomials in $y$. Agreement for infinitely many $y$ makes them identical, so evaluating at $y=0$ proves [Characteristic polynomials of AB and BA](../../../../../characteristic-polynomials-of-ab-and-ba.md):

$$
\boxed{\chi_{AB}(t)=\chi_{BA}(t).}
$$

Their [minimal polynomials](../../../../../minimal-polynomial.md) need not agree. For

$$
A=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&1\\0&0\end{pmatrix},
$$

we have $AB=B\ne0$, $B^2=0$, and $BA=0$. The two [minimal polynomials](../../../../../minimal-polynomial.md) are respectively **$t^2$ and $t$**, although both characteristic polynomials are $t^2$.

For any $p(t)=\sum_jp_jt^j$, the identity $(BA)^{j+1}=B(AB)^jA$ gives

$$
(BA)p(BA)=B p(AB)A.
$$

Taking $p=m_{AB}$ makes the right-hand side zero. Every annihilating polynomial is divisible by the [minimal polynomial](../../../../../minimal-polynomial.md), so

$$
\boxed{m_{BA}(t)\mid t\,p(t).}
$$

If $AB$ is [diagonalizable](../../../../../diagonalizable-matrix.md), $p$ has only simple roots. Therefore each nonzero [eigenvalue](../../../../../eigenvalue.md) of $BA$ has only size-one [Jordan blocks](../../../../../jordan-block.md), and the zero-eigenvalue blocks have size at most two. Squaring kills the latter nilpotent blocks, so $(BA)^2$ is [diagonalizable](../../../../../diagonalizable-matrix.md), as is $(AB)^2$.

By their common [characteristic polynomial](../../../../../characteristic-polynomial.md), $AB$ and $BA$ have the same [eigenvalues](../../../../../eigenvalue.md) counted with algebraic multiplicity. Squaring produces the same multiset of squared [eigenvalues](../../../../../eigenvalue.md), including combined multiplicities if two [eigenvalues](../../../../../eigenvalue.md) have the same square. The two [diagonalizable](../../../../../diagonalizable-matrix.md) squares therefore have the same diagonal normal form up to permutation. This proves [similarity of squared matrix products with one diagonalizable product](../../../../../similarity-of-squared-matrix-products-with-one-diagonalizable-product.md):

$$
\boxed{(AB)^2\text{ and }(BA)^2\text{ are conjugate}.}
$$

It does not imply that $AB$ and $BA$ themselves are conjugate: the possible size-two nilpotent blocks at zero are exactly what squaring removes.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
