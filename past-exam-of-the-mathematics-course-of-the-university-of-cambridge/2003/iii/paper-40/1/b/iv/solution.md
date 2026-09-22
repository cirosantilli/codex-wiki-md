<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For independent individuals under fixed [administrative censoring](../../../../../../../administrative-censoring.md), an observed failure contributes the [probability density function](../../../../../../../probability-density-function.md) $\theta e^{-\theta x_i}$, while a censored observation contributes the [survivor function](../../../../../../../survival-function.md) $e^{-\theta x_i}$. Hence the [survival likelihood](../../../../../../../survival-likelihood.md) and [log-likelihood](../../../../../../../log-likelihood.md) are

$$
L(\theta)=\prod_i[\theta e^{-\theta x_i}]^{\Delta_i}[e^{-\theta x_i}]^{1-\Delta_i}=\theta^d e^{-\theta E},\qquad \ell(\theta)=d\log\theta-\theta E.
$$

For $d>0$, the [score function](../../../../../../../informant-function.md) $\ell'(\theta)=d/\theta-E$ vanishes at $d/E$, and $\ell''(\theta)=-d/\theta^2<0$. This is the unique maximum over $\theta>0$:

$$
\boxed{\widehat\theta=d/E=\widetilde\theta.}
$$

Thus [maximum likelihood estimation](../../../../../../../maximum-likelihood-estimation.md) agrees with the observed-exposure estimating equation. If there are no failures, the [likelihood](../../../../../../../likelihood-function.md) decreases with $\theta$: its supremum is approached as $\theta\downarrow0$, or attained at zero if that boundary is admitted.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
