<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gauss-Markov theorem](../../../../../../gauss-markov-theorem.md) states that with full-column-rank design, mean-zero errors and covariance $\sigma^2I$, the [ordinary least squares](../../../../../../ordinary-least-squares.md) estimator is the best linear unbiased estimator: its covariance is no larger than any other such estimator's in the [Loewner order](../../../../../../loewner-order.md). Normality is unnecessary for that theorem.

In the given [normal linear model](../../../../../../normal-linear-model.md), maximizing the [likelihood function](../../../../../../likelihood-function.md) is equivalent to minimizing $\|Y-X\beta\|^2$. The [normal equations](../../../../../../normal-equation.md) and full rank give

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad\mathbb E\widehat\beta=\beta,\qquad\operatorname{Cov}(\widehat\beta)=\sigma^2(X^TX)^{-1}.}
$$

For a direct variance comparison, write $\beta^*=AY$. Unbiasedness for every $\beta$ requires $AX=I_p$. Set $B=(X^TX)^{-1}X^T$ and $D=A-B$, so $DX=0$. The cross covariance terms vanish because $BD^T=(X^TX)^{-1}(DX)^T=0$. Therefore

$$
\operatorname{Cov}(\beta^*)=\sigma^2[(X^TX)^{-1}+DD^T],\qquad
\boxed{\operatorname{Var}(t^T\beta^*)-\operatorname{Var}(t^T\widehat\beta)=\sigma^2\|D^Tt\|^2\ge0.}
$$

This proves the requested comparison for every contrast $t$ without relying only on the theorem's name.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
