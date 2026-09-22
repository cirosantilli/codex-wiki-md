<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The PDF gives an [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) with shape $k$ and scale $\theta$, and a [gamma distribution](../../../../../gamma-distribution.md) prior with shape $\alpha$ and rate $\lambda$. Write $\mu(\theta)=\theta/(k-1)$. The supplied conditional [moments](../../../../../moment.md), together with $\mathbb E\theta=\alpha/\lambda$ and $\mathbb E\theta^2=\alpha(\alpha+1)/\lambda^2$, give the three structural quantities of the [Bühlmann model](../../../../../buhlmann-model.md):

$$
\begin{aligned}
m&=\mathbb E\mu(\theta)=\frac\alpha{\lambda(k-1)},\\
v&=\operatorname{Var}(\mu(\theta))=\frac\alpha{\lambda^2(k-1)^2},\\
s^2&=\mathbb E[\operatorname{Var}(X_i\mid\theta)]
=\frac{\alpha(\alpha+1)}{\lambda^2(k-1)^2(k-2)}.
\end{aligned}
$$

Here $v$ is the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md) and $s^2$ the [expected process variance](../../../../../expected-process-variance.md). The [law of total covariance](../../../../../law-of-total-covariance.md) and [conditional independence](../../../../../conditional-independence.md) of different years imply

$$
\mathbb E X_i=m,\qquad
\operatorname{Cov}(\mu(\theta),X_i)=v,\qquad
\operatorname{Cov}(X_i,X_j)=v+s^2\mathbf1_{\{i=j\}}.
$$

All these quantities are finite because $k>2$.

For any coefficients $c_i$, minimizing the [mean squared error](../../../../../mean-squared-error.md) over the intercept first gives $c_0=m(1-\sum_i c_i)$. Let $Y=\mu(\theta)-m$ and $W_i=X_i-m$. Expanding the remaining [mean squared error](../../../../../mean-squared-error.md) gives

$$
\mathbb E\left[(Y-\sum_i c_iW_i)^2\right]
=v-2v\sum_i c_i+s^2\sum_i c_i^2+v\left(\sum_i c_i\right)^2.
$$

Its [normal equations](../../../../../normal-equation.md) are $s^2c_i+v\sum_jc_j=v$ for every $i$. Since $s^2>0$, subtracting any two equations shows that all $c_i$ agree. The quadratic part is strictly positive for every nonzero coefficient change, so the solution is the unique global minimizer. Solving gives

$$
\boxed{c_i=\frac v{s^2+nv}=\frac{k-2}{n(k-2)+\alpha+1}\quad(1\le i\le n),\qquad
c_0=\frac{\alpha(\alpha+1)}{\lambda(k-1)[n(k-2)+\alpha+1]}.}
$$

A [credibility estimate](../../../../../credibility-estimate.md) combines individual experience with the collective [expected value](../../../../../expected-value.md), using an experience weight $Z\in[0,1]$. In this equal-exposure setting, the [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md) is

$$
\boxed{\widehat\mu_{\rm lin}=(1-Z)m+Z\overline X,\qquad
Z=\frac{nv}{s^2+nv}=\frac{n(k-2)}{n(k-2)+\alpha+1}.}
$$

Thus the computed coefficients give exactly a [credibility estimate](../../../../../credibility-estimate.md), with a fixed [credibility factor](../../../../../credibility-factor.md) determined by known parameters and the number of observed years. This is [Bühlmann credibility for inverse-gamma observations](../../../../../buhlmann-credibility-for-inverse-gamma-observations.md).

For the final Bayesian calculation, the [likelihood function](../../../../../likelihood-function.md) in $\theta$ is proportional to $\theta^{nk}\exp(-\theta\sum_i x_i^{-1})$. Multiplication by the [gamma distribution](../../../../../gamma-distribution.md) prior gives the [Gamma prior for an inverse-gamma scale](../../../../../gamma-prior-for-an-inverse-gamma-scale.md) update

$$
\theta\mid x_1,\ldots,x_n\sim\operatorname{Gamma}\left(\alpha+nk,\text{ rate }\lambda+\sum_i x_i^{-1}\right).
$$

Under [quadratic loss](../../../../../squared-error-loss.md), the conditional risk of an estimate $d$ is $\operatorname{Var}(\mu(\theta)\mid x)+(d-\mathbb E[\mu(\theta)\mid x])^2$. Its minimizer is therefore the [posterior mean](../../../../../posterior-mean.md):

$$
\boxed{\widehat\mu_{\rm Bayes}=\frac{\alpha+nk}{(k-1)(\lambda+\sum_i x_i^{-1})}.}
$$

**This is not a fixed-weight arithmetic-mean [credibility estimate](../../../../../credibility-estimate.md).** For $n=2$, the observations $(1,3)$ and $(2,2)$ have the same [sample mean](../../../../../sample-mean.md), but reciprocal sums $4/3$ and $1$, hence different [posterior means](../../../../../posterior-mean.md). For any $n>2$, append the same positive observations to these two samples. For $n=1$, the estimate is $Cx/(1+\lambda x)$, with $C=(\alpha+k)/(k-1)$; its second [derivative](../../../../../derivative.md) is $-2C\lambda/(1+\lambda x)^3\ne0$, so it is not affine either. Symmetry in the observations would force equal slopes in any affine representation, so these examples also exclude a general fixed-coefficient linear representation.

One can express the [posterior mean](../../../../../posterior-mean.md) as a broader data-dependent blend. With $A=\sum_i x_i^{-1}$ and [harmonic mean](../../../../../harmonic-mean.md) $H=n/A$, it is

$$
\widehat\mu_{\rm Bayes}=(1-Z_B)m+Z_B\frac{kH}{k-1},\qquad Z_B=\frac A{\lambda+A}.
$$

This weights a harmonic-mean-based experience estimate, and the weight itself depends on the observations. It is not the [credibility estimate](../../../../../credibility-estimate.md) based on $\overline X$ and the fixed [Bühlmann credibility factor](../../../../../credibility-factor.md) derived above.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
