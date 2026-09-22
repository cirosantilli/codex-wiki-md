<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

Let $\ell(\theta;x)=\log p(x\mid\theta)$. The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) maximizes this function; the [score function](../../../../../informant-function.md) is $U=\partial_\theta\ell$, the [Observed Fisher information](../../../../../observed-fisher-information.md) is $\widehat j=-\partial_\theta^2\ell(\widehat\theta;x)$, and the [Fisher information](../../../../../fisher-information-matrix.md) is $I_n(\theta)=\mathbb E_\theta U^2=-\mathbb E_\theta\ell''$ under the stated differentiation regularity. Differentiating normalization gives $\mathbb EU=0$. For iid observations the score is a sum of iid centered terms with [variance](../../../../../variance-split.md) $I_1$, so the [central limit theorem](../../../../../central-limit-theorem.md) gives $U/\sqrt{nI_1}\Rightarrow N(0,1)$ when $0<I_1<\infty$. Under the additional usual consistency, identifiability and interior-MLE regularity, $\sqrt{I_n}(\widehat\theta-\theta)\Rightarrow N(0,1)$. Differentiation under the [integral](../../../../../integral.md) alone does not imply all these MLE conditions.

For the specified autoregression, index the innovations so $X_i=\theta X_{i-1}+E_i$, with $x_0=1$. Conditional normal densities give

$$
L(\theta;x)=(2\pi)^{-n/2}\exp\left[-\frac12\sum_{i=1}^n(x_i-\theta x_{i-1})^2\right].
$$

Set $A=\sum x_{i-1}^2\geq1$, $B=\sum x_{i-1}x_i$ and $C=\sum x_i^2$. Completing the square gives

$$
\boxed{\widehat\theta=B/A,\qquad\widehat j=A.}
$$

The likelihood ratio between two data vectors is independent of $\theta$ precisely when their coefficients $A,B$ agree, because its log is a constant plus $\theta\Delta B-\theta^2\Delta A/2$. The positive-density likelihood-ratio criterion therefore makes $(A,B)$ minimal sufficient. Since $(A,B)\leftrightarrow(\widehat j,\widehat\theta)$ is bijective, the requested pair is also minimal sufficient.

With the flat improper prior, the posterior kernel is $\exp[-A(\theta-\widehat\theta)^2/2]$, which is integrable because $A\geq1$. Thus

$$
\boxed{\theta\mid x\sim N(\widehat\theta,A^{-1}),\qquad S=\sqrt A=\sqrt{\widehat j}.}
$$

Conditionally on the observations, $S(\theta-\widehat\theta)$ is exactly standard normal, as is $E_1$. This is a posterior statement, not a claim that the estimator standardized by the random information is an exact normal sampling pivot.

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
