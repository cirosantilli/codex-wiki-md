<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Let $H=X(X^TX)^{-1}X^T$ be the orthogonal projection onto the design column space. [Linear transformations](../../../../../linear-map.md) of the Gaussian errors give

$$
\boxed{\hat\theta\sim N_p(\theta,\sigma^2(X^TX)^{-1}),\qquad
\hat\epsilon\sim N_n(0,\sigma^2(I-H)).}
$$

The residual distribution is a singular multivariate normal supported on the orthogonal complement of that column space. Their cross-[covariance](../../../../../covariance.md) is $\sigma^2(X^TX)^{-1}X^T(I-H)=0$. Joint normality even makes the two vectors independent.

Order the observations as $11,12,21,22$. The two [normal linear models](../../../../../normal-linear-model.md) have design [matrices](../../../../../matrix.md)

$$
X_I=\begin{pmatrix}1&0&0\\1&0&1\\0&1&2\\0&1&3\end{pmatrix},\qquad
X_{II}=\begin{pmatrix}1&0&0\\1&0&2\\0&1&3\\0&1&1\end{pmatrix}.
$$

Removing each row mean leaves the information for the common slope equal to the sum of within-row squared fertilizer deviations. These sums are $1$ and $4$, respectively. Therefore

$$
\boxed{\operatorname{Var}_I\hat\beta=\sigma^2,\qquad
\operatorname{Var}_{II}\hat\beta=\sigma^2/4.}
$$

The second design estimates the slope four times as precisely in [variance](../../../../../variance-split.md) terms.

The observed data in the second design are fitted exactly by $\hat\theta=(100,300,100)^T$. With $a=(2,2,0)^T$, the no-fertilizer total forecast is

$$
\boxed{\widehat T_{\rm next}=a^T\hat\theta=800.}
$$

The future four independent errors contribute [variance](../../../../../variance-split.md) $4\sigma^2$. Parameter-estimation uncertainty contributes $\sigma^2a^T(X_{II}^TX_{II})^{-1}a=13\sigma^2$, so the prediction-error [variance](../../../../../variance-split.md) is $17\sigma^2$, not merely the [variance](../../../../../variance-split.md) of the estimated mean. Normally, with $s^2=\|\hat\epsilon\|^2/(4-3)$, the [prediction interval in a normal linear model](../../../../../prediction-interval-in-a-normal-linear-model.md) is

$$
800\pm t_{1,0.975}\,s\sqrt{17},\qquad t_{1,0.975}=12.7062\ldots.
$$

Here the printed data have zero residual and hence $s=0$. **The formal plug-in interval collapses to $[800,800]$**, exhibiting [zero-residual degeneracy of regression prediction](../../../../../zero-residual-degeneracy-of-regression-prediction.md). Under the stated model with unknown positive [variance](../../../../../variance-split.md), this exact fit is a probability-zero sample and the Studentized statistic is undefined at it; the collapsed expression is not evidence that future yield is certain. No positive-width numerical 95% interval can be obtained from these exact data by the usual residual-[variance](../../../../../variance-split.md) method without extra [variance](../../../../../variance-split.md) information or an explicit observation-rounding model.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
