<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply [Young's rule](../../../../../../young-s-rule.md), stated as

$$
M^{(n-k,k)}\cong\bigoplus_{\rho\vdash n}(S^\rho)^{\oplus K_{\rho,(n-k,k)}}.
$$

Here the [Kostka number](../../../../../../kostka-number.md) counts [Semistandard Young tableaux](../../../../../../semistandard-young-tableau.md) of shape $\rho$ with $n-k$ entries equal to $1$ and $k$ entries equal to $2$. Their rows weakly increase and their columns strictly increase. A column can therefore have at most two cells, so only a [partition of an integer](../../../../../../partition-of-an-integer.md) $\rho=(n-j,j)$ can occur.

In such a [semistandard Young tableau](../../../../../../semistandard-young-tableau.md), all $j$ entries in the second row must be $2$ and all $j$ entries above them must be $1$. The whole first row is then fixed by the content: its first $n-k$ entries are $1$ and its remaining $k-j$ entries are $2$. This is possible exactly when $j\leq k$ and $j\leq n-k$. Because $k\leq n/2$, the second inequality follows from the first. There is exactly one filling for every $0\leq j\leq k$, and none for any other shape.

Consequently each displayed [Specht module](../../../../../../specht-module.md) has multiplicity one, proving the [two-row Young permutation module decomposition](../../../../../../two-row-young-permutation-module-decomposition.md)

$$
\boxed{M^{(n-k,k)}\cong\bigoplus_{j=0}^k S^{(n-j,j)}.}
$$

For $j=0$, the zero second part is omitted. As a dimension check, the [Hook-length formula](../../../../../../hook-length-formula.md) gives $\dim S^{(n-j,j)}=\binom nj-\binom n{j-1}$, with $\binom n{-1}=0$; the sum telescopes to $\binom nk$, the dimension of the original [permutation representation](../../../../../../permutation-representation.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
