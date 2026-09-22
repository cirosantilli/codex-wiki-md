<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the PDF's covector-first convention: its space $\mathcal T_l^k$ consists of [tensor fields](../../../../../../tensor-field.md) in

$$
(T^*M)^{\otimes k}\otimes(TM)^{\otimes l}.
$$

This reverses the order in which some texts list [tensor type](../../../../../../tensor-type.md). For a finite-dimensional real [vector space](../../../../../../vector-space-split.md) $V$, define the [tensor contraction](../../../../../../tensor-contraction.md) first on decomposable tensors:

$$
C_j^i(\alpha_1\otimes\cdots\otimes\alpha_k\otimes v_1\otimes\cdots\otimes v_l)
=\alpha_i(v_j)\,\alpha_1\otimes\cdots\widehat{\alpha_i}\cdots\otimes\alpha_k
\otimes v_1\otimes\cdots\widehat{v_j}\cdots\otimes v_l.
$$

The hats mean omission, with the other factors left in their original order. The formula is a [multilinear map](../../../../../../multilinear-map.md) of its individual factors, so the [universal property of a tensor product](../../../../../../universal-property-of-a-tensor-product.md) gives a unique [linear map](../../../../../../linear-map.md) with this formula.

Apply it with $V=T_pM$ at every $p$. Evaluation of a [covector](../../../../../../covector.md) on a vector is basis independent: under a change of frame, one factor transforms by a [matrix](../../../../../../matrix.md) and the other by its inverse transpose, and the [matrices](../../../../../../matrix.md) cancel in the pairing. Thus the fiber maps agree on overlapping [vector bundle trivializations](../../../../../../vector-bundle-trivialization.md). In a local [dual basis](../../../../../../dual-basis.md), the coefficients of the contracted tensor are finite sums of coefficients with the selected covariant and contravariant indices set equal. They remain smooth. Hence

$$
\boxed{C_j^i:\mathcal T_l^k\longrightarrow\mathcal T_{l-1}^{k-1}}
$$

is a globally defined smooth contraction for $k,l\geq1$. It is also linear over $C^\infty(M)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
