<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Condition on the training covariates, and let $m_i=\mathbb E Y_i$. The fresh response $Y_i^N$ has the same marginal distribution as $Y_i$ and is independent of the complete training response vector, hence independent of $\widehat Y_i=\widehat f(x_i)$. Assume the relevant second moments are finite. Expanding the squared errors gives

$$
\begin{aligned}
\mathbb E[(Y_i^N-\widehat Y_i)^2]&=\mathbb E Y_i^2-2m_i\mathbb E\widehat Y_i+\mathbb E\widehat Y_i^2,\\
\mathbb E[(Y_i-\widehat Y_i)^2]&=\mathbb E Y_i^2-2\mathbb E[Y_i\widehat Y_i]+\mathbb E\widehat Y_i^2.
\end{aligned}
$$

The first expectation averages over both training and new responses; the second averages over training responses only. Subtracting cancels both second-moment terms, leaving

$$
2\{\mathbb E[Y_i\widehat Y_i]-m_i\mathbb E\widehat Y_i\}=2\operatorname{Cov}(Y_i,\widehat Y_i).
$$

Averaging over the design points proves the [covariance formula for prediction optimism](../../../../../../covariance-formula-for-prediction-optimism.md):

$$
\boxed{\operatorname{Opt}=\operatorname{Err}_{\mathrm{in}}-\mathbb E\operatorname{err}=\frac2n\sum_{i=1}^n\operatorname{Cov}(Y_i,\widehat Y_i).}
$$

No linear fitting rule or Gaussian noise assumption is needed. The difference arises because a training response and its fitted value are dependent, whereas a fresh response and the fitted value are independent. Ordinary fitting often makes those covariances positive and the [training error](../../../../../../training-error.md) too favorable, explaining the name [prediction optimism](../../../../../../prediction-optimism.md).

For example, if $\widehat Y=HY$ is a fixed [linear smoother](../../../../../../linear-smoother.md) and $\operatorname{Cov}(Y)=\sigma^2I$, then $\operatorname{Cov}(Y_i,\widehat Y_i)=\sigma^2H_{ii}$. Thus

$$
\boxed{\operatorname{Opt}=\frac{2\sigma^2}{n}\operatorname{tr}(H)=\frac{2\sigma^2}{n}\operatorname{df}_{\mathrm{eff}}.}
$$

This links the optimism correction to [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md). For a data-selected fitting operator, its realized trace alone does not generally give the covariance penalty, since selecting the model uses the responses too.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
