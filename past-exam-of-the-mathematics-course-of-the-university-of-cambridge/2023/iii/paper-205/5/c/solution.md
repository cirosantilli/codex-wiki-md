<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the active set $A_k$, maintain

$$
M_k^{-1}=(X_{A_k}X_{A_k}^T+\lambda I)^{-1}.
$$

The initial $n\times n$ [matrix inverse](../../../../../../matrix-inverse.md) costs $O(n^3)$. At step $k$, compute $v_k=M_k^{-1}Y$ in $O(n^2)$ operations and all active ridge coefficients $X_{A_k}^Tv_k$ in $O(|A_k|n)$ operations; their smallest absolute value determines $j_k$.

After deleting $j_k$,

$$
M_{k+1}=M_k-X_{j_k}X_{j_k}^T.
$$

Part b ensures that the denominator in the [Sherman–Morrison formula](../../../../../../sherman-morrison-formula.md) is positive, and the rank-one downdate

$$
M_{k+1}^{-1}
=M_k^{-1}+
\frac{M_k^{-1}X_{j_k}X_{j_k}^TM_k^{-1}}
{1-X_{j_k}^TM_k^{-1}X_{j_k}}
$$

costs $O(n^2)$. Summing over the $p$ steps gives

$$
O(n^3)+O(pn^2)+O\!\left(n\sum_{k=1}^p|A_k|\right)
=O(n^3+pn^2+p^2n).
$$

Since $p\geq n$, both earlier terms are bounded by $O(p^2n)$, proving the claimed computational complexity within [computational complexity theory](../../../../../../computational-complexity-theory.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
