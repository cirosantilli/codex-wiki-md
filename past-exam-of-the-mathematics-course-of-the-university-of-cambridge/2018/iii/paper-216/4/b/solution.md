<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one factor, write $\lambda\in\mathbb R^p$ for the loading vector and $v=\sigma^2>0$. Let $\lambda_t$ be its current value and $s=v+\|\lambda_t\|^2$. The E-step of the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) uses the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) to obtain

$$
Z_i\mid Y_i,\lambda_t\sim N(m_i,u),\qquad
m_i=\frac{\lambda_t^TY_i}{s},\qquad u=\frac vs.
$$

Thus $\mathbb E[Z_i^2\mid Y_i]=u+m_i^2$. The terms of the expected complete-data [log-likelihood](../../../../../../log-likelihood.md) that depend on a candidate $\lambda$ are

$$
Q(\lambda\mid\lambda_t)
=-\frac1{2v}\sum_{i=1}^n\left(\|Y_i\|^2-2m_i\lambda^TY_i+(u+m_i^2)\|\lambda\|^2\right)+\text{constant}.
$$

This is a strictly concave quadratic in $\lambda$, since $\sum_i(u+m_i^2)>0$. Its unique maximizer is

$$
\boxed{\lambda_{t+1}=\frac{\sum_iY_im_i}{\sum_i(u+m_i^2)}.}
$$

For an explicit expression involving only the current loading and data, put $S=n^{-1}\sum_iY_iY_i^T$. Substitution gives the [EM update for a single-factor Gaussian model](../../../../../../em-update-for-a-single-factor-gaussian-model.md)

$$
\boxed{\lambda_{t+1}=\frac{(v+\|\lambda_t\|^2)S\lambda_t}
{v(v+\|\lambda_t\|^2)+\lambda_t^TS\lambda_t}.}
$$

No empirical centering is applied because the model fixes the mean to zero. If initialized at zero, this update remains at zero; monotonicity alone does not guarantee that such a stationary point is a global maximum. This part is present in the PDF but missing from the TeX transcription.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
