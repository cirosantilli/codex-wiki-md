# Matrix similarity invariants

↑ **Parent:** [Matrix similarity](matrix-similarity.md)

[Matrix similarity invariants](matrix-similarity-invariants.md) are quantities unchanged by replacing $A$ with $S^{-1}AS$. Important examples are the [characteristic polynomial](characteristic-polynomial.md), [trace](matrix-trace.md), [determinant](determinant.md), [matrix rank](matrix-rank.md), and [eigenvalues](eigenvalue.md) with their [algebraic multiplicities](algebraic-multiplicity.md). The [characteristic polynomial](characteristic-polynomial.md) convention here is $\chi_A(t)=\det(tI-A)$, where $I$ is the [identity matrix](identity-matrix.md).[§9C, Definition 9.63, printed p. 363; Theorem 9.65, printed p. 364: characteristic polynomial, trace, and determinant](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

The short [determinant](determinant.md) proof works over any [field](field.md): because $tI-B=S^{-1}(tI-A)S$, [multiplicativity of the determinant](multiplicativity-of-the-determinant.md) gives

$$
\chi_B(t)=\det(S^{-1})\det(tI-A)\det(S)=\chi_A(t).
$$

Thus its roots, the [eigenvalues](eigenvalue.md), retain their [algebraic multiplicities](algebraic-multiplicity.md) in any [field extension](field-extension.md) where the [polynomial](polynomial-split.md) splits. Also $\det B=\det A$. The [cyclic property of the trace](cyclic-property-of-the-trace.md) gives $\operatorname{tr}(S^{-1}AS)=\operatorname{tr}(ASS^{-1})=\operatorname{tr}A$; equivalently, the [trace](matrix-trace.md) is determined by the [coefficient](coefficient.md) of $t^{n-1}$ in the [characteristic polynomial](characteristic-polynomial.md) for an $n$-by-$n$ [matrix](matrix.md).[§8D, Theorems 8.49–8.50, printed pp. 326–327: cyclic trace identity and basis independence](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

For the two [matrices](matrix.md) in the opening example,

$$
\chi_A(t)=\chi_B(t)=(t-2)(t-5)=t^2-7t+10,\qquad
\operatorname{tr}A=\operatorname{tr}B=7,\qquad \det A=\det B=10.
$$

Their entries differ, yet these quantities agree. Agreement is a useful necessary test for [matrix similarity](matrix-similarity.md); it is not sufficient in general, as [same eigenvalues do not imply similarity](same-eigenvalues-do-not-imply-similarity.md) illustrates.

The relation also preserves repeated application. Adjacent factors $SS^{-1}$ cancel to give

$$
B^k=S^{-1}A^kS\quad(k\geq0).
$$

For the opening example, [matrix powers](matrix-power.md) therefore have the explicit form

$$
B^k=\begin{pmatrix}2^k&2^k-5^k\\0&5^k\end{pmatrix}.
$$

At $k=2$, this is $\begin{pmatrix}4&-21\\0&25\end{pmatrix}$. Acting on $y=(1,1)^T$ gives $(-17,25)^T$, which reconstructs as $S(-17,25)^T=(8,25)^T=A^2x$. More generally $q(B)=S^{-1}q(A)S$ for every [polynomial](polynomial-split.md) $q$, so the [minimal polynomial](minimal-polynomial.md) is also unchanged. Multiplication by [invertible matrices](invertible-matrix.md) preserves [matrix rank](matrix-rank.md), giving another invariant without finding [eigenvalues](eigenvalue.md).

## ↑ Ancestors (6)

1. [Matrix similarity](matrix-similarity.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Matrix similarity](matrix-similarity.md)
- [Matrix similarity invariants](matrix-similarity-invariants.md)
- [Similarity transformation](similarity-transformation.md)
