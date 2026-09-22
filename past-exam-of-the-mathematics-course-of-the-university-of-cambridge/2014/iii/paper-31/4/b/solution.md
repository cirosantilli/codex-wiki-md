<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditional on $\Theta=\theta$, summing the individual independent Poisson counts gives $Y_j\sim\operatorname{Poisson}(m_j\theta)$. The between-year [conditional independence](../../../../../../conditional-independence.md) makes the [likelihood function](../../../../../../likelihood-function.md)

$$
L(\theta)=\prod_{j=1}^n\frac{e^{-m_j\theta}(m_j\theta)^{y_j}}{y_j!}
\ \propto\ \theta^y e^{-W\theta},\qquad
 y=\sum_jy_j,\quad W=\sum_jm_j.
$$

Multiplying by the [gamma distribution](../../../../../../gamma-distribution.md) prior density, proportional to $\theta^{\alpha-1}e^{-\beta\theta}$, gives the [Poisson-gamma conjugacy with unequal exposures](../../../../../../poisson-gamma-conjugacy-with-unequal-exposures.md):

$$
\boxed{\Theta\mid y_1,\ldots,y_n
\sim\operatorname{Gamma}(\alpha+y,\beta+W).}
$$

For an action $t$, the posterior [squared-error loss](../../../../../../squared-error-loss.md) decomposes as

$$
\mathbb E[(\Theta-t)^2\mid\mathbf y]
=\operatorname{Var}(\Theta\mid\mathbf y)
+\bigl(t-\mathbb E[\Theta\mid\mathbf y]\bigr)^2.
$$

Hence the [Bayes estimator under squared error loss](../../../../../../bayes-estimator-under-squared-error-loss.md) is the [posterior mean](../../../../../../posterior-mean.md), giving

$$
\boxed{\widehat\theta_{\rm Bayes}=\frac{\alpha+y}{\beta+W}.}
$$

Future counts are independent of the observed years conditional on $\Theta$, so the [law of total expectation](../../../../../../law-of-total-expectation.md) then gives the posterior predictive expected count

$$
\boxed{\mathbb E[Y_{n+1}\mid\mathbf y]
=m_{n+1}\mathbb E[\Theta\mid\mathbf y]
=m_{n+1}\frac{\alpha+\sum_jy_j}{\beta+\sum_jm_j}.}
$$

**The Bayesian and credibility estimates coincide exactly.** This [exact Bühlmann–Straub credibility for Poisson-gamma counts](../../../../../../exact-buhlmann-straub-credibility-for-poisson-gamma-counts.md) occurs because the posterior mean is already affine in the exposure-weighted experience, and therefore belongs to the class over which the credibility estimate minimizes [mean squared error](../../../../../../mean-squared-error.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
