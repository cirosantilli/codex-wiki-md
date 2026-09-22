<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $m(\lambda)=\mathbb E(X_i\mid\lambda)$ and $v(\lambda)=\operatorname{Var}(X_i\mid\lambda)$. The [Bühlmann model](../../../../../../buhlmann-model.md) uses the finite structural parameters

$$
m_0=\mathbb E m(\lambda),\qquad v=\mathbb E v(\lambda),\qquad a=\operatorname{Var}(m(\lambda)).
$$

Here $v$ is the [expected process variance](../../../../../../expected-process-variance.md) and $a$ is the [variance of hypothetical means](../../../../../../variance-of-hypothetical-means.md). The target is the latent conditional mean $m(\lambda)$, rather than the realized next count. The [Bühlmann credibility estimate](../../../../../../buhlmann-credibility-premium.md) is the best affine predictor of that target under [mean squared error](../../../../../../mean-squared-error.md).

The [law of total expectation](../../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../../law-of-total-variance.md) give $\mathbb EX_i=m_0$ and $\operatorname{Var}(X_i)=v+a$. Conditional independence gives $\operatorname{Cov}(X_i,X_j\mid\lambda)=0$ for $i\ne j$, and the [law of total covariance](../../../../../../law-of-total-covariance.md) therefore yields

$$
\operatorname{Cov}(X_i,X_j)=a\quad(i\ne j),\qquad
\operatorname{Cov}(m(\lambda),X_i)=a.
$$

To derive the optimal predictor, consider $d=A+\sum_{i=1}^n b_iX_i$. Minimizing with respect to the intercept gives $A=m_0(1-\sum_i b_i)$. Thus $d=m_0+\sum_i b_i(X_i-m_0)$. The [linear least-squares projection](../../../../../../linear-least-squares-projection.md) normal equations are

$$
(vI+a\mathbf1\mathbf1^T)b=a\mathbf1.
$$

For $v>0$, subtraction of any two equations forces all $b_i$ equal. Substituting a common coefficient then gives $b_i=a/(v+na)$. Equivalently, the [mean squared error](../../../../../../mean-squared-error.md) of the centered predictor is $a-2a\sum_i b_i+v\sum_i b_i^2+a(\sum_i b_i)^2$, a convex quadratic with precisely these normal equations. Hence

$$
\boxed{\widehat m_n=Z_n\overline X_n+(1-Z_n)m_0,
\qquad Z_n=\frac{na}{na+v}=\frac{n}{n+K},\quad K=\frac va.}
$$

The ratio notation assumes $a>0$; the [credibility factor](../../../../../../credibility-factor.md) formula $na/(na+v)$ also handles $a=0,v>0$. If $a=0$, the target is the constant $m_0$ almost surely. If $v=0,a>0$, one observation already equals $m(\lambda)$ almost surely, and the average gives it exactly. If both vanish, the target and observations are constant.

The result optimizes over affine functions of the observations. It need not equal the unrestricted [posterior mean](../../../../../../posterior-mean.md); exact [Bayesian inference](../../../../../../bayesian-statistics.md) generally depends on the whole prior and likelihood, whereas the [Bühlmann credibility estimate](../../../../../../buhlmann-credibility-premium.md) uses these second-moment structural parameters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
