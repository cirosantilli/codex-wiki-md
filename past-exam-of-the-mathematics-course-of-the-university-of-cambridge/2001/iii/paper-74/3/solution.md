<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $R=\mathcal O_k$, $S=\mathcal O_K$ and $n=[K:k]$. For each [prime ideal](../../../../../prime-ideal.md) $\mathfrak P$ of $S$ above $\mathfrak p$ of $R$, set $f_{\mathfrak P}=[S/\mathfrak P:R/\mathfrak p]$. The relative [norm of a fractional ideal](../../../../../norm-of-a-fractional-ideal.md) can be specified on the unique [prime ideal factorization](../../../../../prime-ideal-factorization.md) by

$$
N_{K/k}\left(\prod_{\mathfrak P}\mathfrak P^{a_{\mathfrak P}}\right)
=\prod_{\mathfrak p}\mathfrak p^{\sum_{\mathfrak P\mid\mathfrak p}f_{\mathfrak P}a_{\mathfrak P}},\qquad a_{\mathfrak P}\in\mathbb Z.
$$

Here is why this definition is the intrinsic [relative ideal norm from norms of elements](../../../../../relative-ideal-norm-from-norms-of-elements.md), and why the residue weights occur. Localize at $\mathfrak p$. The finite torsion-free $R_{\mathfrak p}$-module $S_{\mathfrak p}$ is free of rank $n$, because $R_{\mathfrak p}$ is a [discrete valuation ring](../../../../../discrete-valuation-ring.md). Multiplication by a nonzero integral $a$ has [determinant](../../../../../determinant.md) $N_{K/k}(a)$. The [Smith normal form](../../../../../smith-normal-form.md) gives

$$
v_{\mathfrak p}(N_{K/k}(a))=\operatorname{length}_{R_{\mathfrak p}}(S_{\mathfrak p}/aS_{\mathfrak p}).
$$

Decompose the quotient at the [prime ideals](../../../../../prime-ideal.md) above $\mathfrak p$. In $S_{\mathfrak P}$ each quotient $\mathfrak P^j/\mathfrak P^{j+1}$ is one-dimensional over $S/\mathfrak P$, so has length $f_{\mathfrak P}$ over $R_{\mathfrak p}$. Therefore

$$
v_{\mathfrak p}(N_{K/k}(a))=\sum_{\mathfrak P\mid\mathfrak p}f_{\mathfrak P}v_{\mathfrak P}(a).
$$

For an integral [ideal](../../../../../ideal.md) $I$, all norms of elements of $I$ have valuations at least $\sum f_{\mathfrak P}v_{\mathfrak P}(I)$. These minima can be attained simultaneously at the finitely many [prime ideals](../../../../../prime-ideal.md) above a fixed $\mathfrak p$. In fact the [Chinese remainder theorem for ideals](../../../../../chinese-remainder-theorem-for-ideals.md), applied inside the finitely generated module $I$, chooses an $a\in I$ with nonzero image in each $I/\mathfrak PI$. Equivalently $v_{\mathfrak P}(a)=v_{\mathfrak P}(I)$ at all these primes. The generated ideal of the element norms consequently has exactly the displayed valuations. Clearing a denominator extends this description to [fractional ideals](../../../../../fractional-ideal.md).

Multiplication of [fractional ideals](../../../../../fractional-ideal.md) adds their prime valuations. The displayed formula therefore proves

$$
\boxed{N_{K/k}(IJ)=N_{K/k}(I)N_{K/k}(J).}
$$

It also gives $N_{K/k}((a))=(N_{K/k}(a))$.

Finally, reduction of the free rank-$n$ module $S_{\mathfrak p}$ modulo $\mathfrak p$ has dimension $n$ over $R/\mathfrak p$. The factorization $\mathfrak pS=\prod_i\mathfrak P_i^{e_i}$ and the [Chinese remainder theorem for ideals](../../../../../chinese-remainder-theorem-for-ideals.md) identify this reduction with the product of the quotients by $\mathfrak P_i^{e_i}$. Their filtrations have $e_i$ successive quotients of dimension $f_i$ over $R/\mathfrak p$. Adding dimensions proves the [fundamental identity for prime decomposition](../../../../../fundamental-identity-for-prime-decomposition.md):

$$
\boxed{[K:k]=\sum_i e_if_i.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
