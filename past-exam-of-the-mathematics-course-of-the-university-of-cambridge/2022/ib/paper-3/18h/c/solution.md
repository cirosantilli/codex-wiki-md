<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\widehat\beta=AY$, where

$$
A=(X^T\Sigma_0^{-1}X)^{-1}X^T\Sigma_0^{-1},
\qquad AX=I.
$$

Any other linear unbiased estimator is $CY$ with $CX=I$, so $C=A+D$ and $DX=0$. The cross covariance vanishes because

$$
A\Sigma_0D^T
=(X^T\Sigma_0^{-1}X)^{-1}X^TD^T=0.
$$

Therefore

$$
\operatorname{Cov}(CY)-\operatorname{Cov}(AY)
=\sigma^2D\Sigma_0D^T\succeq0.
$$

By the [Gauss-Markov theorem](../../../../../../gauss-markov-theorem.md),

$$
\boxed{\widehat\beta\text{ is the best linear unbiased estimator of }\beta}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
