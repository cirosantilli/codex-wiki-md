<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $N=m+1$ and $d=p+1$. Average $V=\prod_{k=0}^p\mathbf1_{A_k}(X_k)$ over all permutations of the first $N$ coordinates, as justified in part (a). For any prescribed ordered tuple of $d$ distinct images $(\ell_0,\ldots,\ell_p)$, exactly $(N-d)!=(m-p)!$ permutations produce that tuple. Therefore

$$
\boxed{\mathbb E\!\left[\prod_{k=0}^p\mathbf1_{A_k}(X_k)\mid\mathcal S_m\right]
=\frac1{(m+1)m\cdots(m+1-p)}
\sum_{\substack{0\leq\ell_0,\ldots,\ell_p\leq m\\\ell_0,\ldots,\ell_p\text{ distinct}}}
\prod_{k=0}^p\mathbf1_{A_k}(X_{\ell_k}).}
$$

The denominator is the [falling factorial](../../../../../../falling-factorial.md) $(N)_d=N!/(N-d)!$, with exactly $p+1$ factors. The sum must be over ordered distinct tuples: its $k$th coordinate is attached to $A_k$, and these sets need not be equal. This is the finite-sample version of [symmetrization as conditional expectation](../../../../../../symmetrization-as-conditional-expectation.md).

The original PDF, as well as the TeX, prints the final factor as $m+1-p+1$. That is an off-by-one error: it must be $m+1-p$. With every $A_k=\mathbb R$, the conditional expectation is one and the numerator counts exactly $(N)_d$ ordered distinct tuples. This forces the normalization above and immediately detects the printed error. Interpreting the sum as unordered subsets would likewise give the wrong normalization and would lose the assignments to the different $A_k$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
