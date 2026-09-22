<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a finite extension of fields [complete](../../../../../../completeness.md) for a [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md), use the unique extended [field absolute value](../../../../../../absolute-value-algebra.md). The extension is [unramified](../../../../../../unramified-extension.md) when its residue extension is a [separable field extension](../../../../../../separable-extension.md) and

$$
[L:K]=[k_L:k_K].
$$

Equivalently, it has ramification index one, a [separable field extension](../../../../../../separable-extension.md) of residue fields, and no defect. For general nondiscrete valued fields, merely saying that the ramification index is one is insufficient; the displayed degree equality is part of the unramified condition.

Put $n=[L:K]=[k_L:k_K]$. Since $\bar x$ generates the residue extension, $1,\bar x,\ldots,\bar x^{n-1}$ are [linearly independent](../../../../../../linear-independence.md) over $k_K$. Their lifts $1,x,\ldots,x^{n-1}$ are [linearly independent](../../../../../../linear-independence.md) over $K$: a nonzero relation could be divided by a coefficient of largest [field absolute value](../../../../../../absolute-value-algebra.md), giving an integral relation whose reduction has at least one nonzero coefficient, contrary to residue independence. They therefore form a $K$-[basis](../../../../../../basis.md) of $L$.

For any $y=\sum_{j=0}^{n-1}a_jx^j$, choose $a_r$ of largest [field absolute value](../../../../../../absolute-value-algebra.md). All coefficients of $y/a_r$ belong to $\mathcal O_K$, and at least one is a unit. Its reduction is a nonzero linear combination of the residue [basis](../../../../../../basis.md), so $y/a_r$ is a unit of $\mathcal O_L$. This proves the [residue-basis norm formula for an unramified extension](../../../../../../residue-basis-norm-formula-for-an-unramified-extension.md)

$$
|y|=\max_j|a_j|.
$$

Hence $y\in\mathcal O_L$ exactly when every $a_j\in\mathcal O_K$. We conclude

$$
\boxed{\mathcal O_L=\bigoplus_{j=0}^{n-1}\mathcal O_Kx^j=\mathcal O_K[x].}
$$

The last equality also uses the fact that every polynomial in the integral element $x$ is integral. The proof requires neither a [uniformizer](../../../../../../uniformizer.md) nor discrete [valuation](../../../../../../valuation.md), and applies to every residue generator specified in the question.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
