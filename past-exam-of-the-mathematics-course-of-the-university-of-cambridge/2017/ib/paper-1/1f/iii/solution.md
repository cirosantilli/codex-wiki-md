<h1 id="1f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $S$ spans and has $n$ elements but is [linearly dependent](../../../../../../linear-dependence.md), a nontrivial [linear combination](../../../../../../linear-combination.md) equal to zero lets us remove one member without changing the [span](../../../../../../linear-span.md). This produces $n-1$ spanning vectors, whereas the [standard basis](../../../../../../standard-basis.md) contains $n$ [linearly independent](../../../../../../linear-independence.md) vectors, contradicting the [Steinitz exchange lemma](../../../../../../steinitz-exchange-lemma.md). Therefore $\boxed{S\text{ is linearly independent}}$. Together the three deductions establish that any two of the three properties imply the third. For $n=0$, the only independent or zero-element family is the empty [basis](../../../../../../basis.md), and the same conclusions hold.

Relative to the given [basis](../../../../../../basis.md) $e_1,e_2$, the proposed vectors are the columns of

$$
M=\begin{pmatrix}\lambda&1\\1&\lambda\end{pmatrix},\qquad \det M=\lambda^2-1.
$$

The [determinant](../../../../../../determinant.md) is nonzero exactly when the columns form a [basis](../../../../../../basis.md). Thus $\boxed{\lambda\ne\pm1}$. At $\lambda=1$ the vectors coincide, and at $\lambda=-1$ they are negatives of one another.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1F](../../1f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
