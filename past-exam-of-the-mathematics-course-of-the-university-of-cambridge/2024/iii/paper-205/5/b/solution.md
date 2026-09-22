<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [leave-one-out residual identity for a linear smoother](../../../../../../leave-one-out-residual-identity-for-a-linear-smoother.md), obtained from the [block matrix inverse](../../../../../../block-matrix-inverse.md) or the [Sherman–Morrison formula](../../../../../../sherman-morrison-formula.md), is

$$
Y_i-\widehat f_{\lambda,-i}(x_i)
=\frac{Y_i-\widehat Y_i}{1-(H_\lambda)_{ii}}.
$$

Hence

$$
\widehat T_\lambda
=\frac1n\sum_{i=1}^n
\left(\frac{Y_i-(H_\lambda Y)_i}{1-(H_\lambda)_{ii}}\right)^2.
$$

Compute once the [spectral decomposition](../../../../../../spectral-decomposition.md) $K=U\operatorname{diag}(d_1,\ldots,d_n)U^T$ in $O(n^3)$ operations and the vector $U^TY$ in $O(n^2)$. For each $\lambda_\ell$, set

$$
h_r(\lambda_\ell)=\frac{d_r}{d_r+n\lambda_\ell}.
$$

Then compute

$$
H_{\lambda_\ell}Y
=U\operatorname{diag}(h_r(\lambda_\ell))U^TY,
\qquad
(H_{\lambda_\ell})_{ii}=\sum_{r=1}^nU_{ir}^2h_r(\lambda_\ell).
$$

Both calculations take $O(n^2)$ operations per tuning parameter, after which the displayed leave-one-out formula costs $O(n)$. All $L$ scores therefore require $O(n^3+Ln^2)$ operations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
