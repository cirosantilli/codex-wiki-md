<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One standard construction uses the [Debiased Lasso](../../../../../../debiased-lasso.md). Starting from the [Square-root Lasso](../../../../../../square-root-lasso.md) estimate $\widehat\beta$, estimate a vector $\widehat\Theta_j$ that approximately inverts the $j$th column of the empirical Gram matrix $\widehat\Sigma=X^TX/n$, for example by a [Nodewise Lasso](../../../../../../nodewise-lasso.md). Define

$$
\widetilde\beta_j
=\widehat\beta_j+\widehat\Theta_j^T\frac{X^T(Y-X\widehat\beta)}n,
\qquad
\widehat V_j=\widehat\Theta_j^T\widehat\Sigma\widehat\Theta_j,
$$

and estimate $\sigma$ by $\widehat\sigma=\lVert Y-X\widehat\beta\rVert_2/\sqrt n$. The approximate two-sided level-$\alpha$ test rejects $H_j^\beta$ when

$$
\left|\frac{\sqrt n\,\widetilde\beta_j}{\widehat\sigma\sqrt{\widehat V_j}}\right|>z_{1-\alpha/2},
$$

where $z_{1-\alpha/2}$ is a [standard normal quantile](../../../../../../standard-normal-quantile.md).

Sufficient high-dimensional conditions include a [Compatibility condition for the Lasso](../../../../../../compatibility-condition-for-the-lasso.md) bounded away from zero, $\gamma\asymp\sqrt{\log p/n}$, $\log p=o(n)$, and

$$
\frac{s\log p}{\sqrt n}\longrightarrow0,
$$

together with the corresponding sparsity and consistency conditions for the nodewise inverse-Gram estimate. Under these assumptions the [Debiased-Lasso asymptotic normality](../../../../../../debiased-lasso-asymptotic-normality.md) makes the rejection probability under $H_j^\beta$ tend to $\alpha$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
