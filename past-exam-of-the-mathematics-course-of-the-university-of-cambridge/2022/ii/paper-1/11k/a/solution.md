<h1 id="11k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A binary [cyclic code](../../../../../../cyclic-code.md) of odd length $n$ is an ideal of $\mathbb F_2[X]/(X^n-1)$. For a primitive $n$th root $\alpha$, its defining set is the set of powers $\alpha^i$ at which every code polynomial vanishes. A [BCH code](../../../../../../bch-code.md) of design distance $\delta$ has $\delta-1$ consecutive powers

$$
\alpha^b,\alpha^{b+1},\ldots,\alpha^{b+\delta-2}
$$

in its defining set.

If a nonzero codeword had weight $w<\delta$, write it as $c(X)=\sum_{j=1}^wc_jX^{i_j}$. Evaluation at $w$ consecutive defining roots gives a homogeneous Vandermonde system in the nonzero values $c_j\alpha^{bi_j}$. Its determinant is nonzero because the support elements $\alpha^{i_j}$ are distinct. Thus every $c_j$ would vanish, a contradiction. This proves the [BCH bound](../../../../../../bch-bound.md)

$$
\boxed{d_{\min}\geq\delta}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11K](../../11k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
