<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Two square matrices are [similar](../../../../../matrix-similarity.md) when $B=P^{-1}AP$ for some invertible matrix $P$. A [Jordan normal form](../../../../../jordan-normal-form.md) is a block-diagonal matrix whose blocks have one eigenvalue on the diagonal, ones on the superdiagonal, and zeros elsewhere; over an algebraically closed field every matrix is similar to such a form, unique up to reordering its [Jordan blocks](../../../../../jordan-block.md).

Both displayed matrices have [characteristic polynomial](../../../../../characteristic-polynomial.md)

$$
\chi_A(t)=\chi_B(t)=(t-1)^3.
$$

However,

$$
\operatorname{rank}(A-I)=1,\qquad
\operatorname{rank}(B-I)=2,
$$

so their eigenspace dimensions are respectively two and one. Thus $A$ has Jordan form $J_2(1)\oplus J_1(1)$, whereas $B$ has Jordan form $J_3(1)$. By uniqueness of Jordan normal form,

$$
\boxed{A\text{ and }B\text{ are not similar}}.
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
