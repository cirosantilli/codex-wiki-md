<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $M=\sum_{i=1}^n m_i$ be the total exposure, and define the [prior distribution](../../../../../prior-probability.md) [expected value](../../../../../expected-value.md), prior [variance](../../../../../variance-split.md) and average binomial noise by

$$
\eta=\mathbb E\theta,\qquad v=\operatorname{Var}(\theta),\qquad w=\mathbb E[\theta(1-\theta)].
$$

Since the [prior distribution](../../../../../prior-probability.md) has a [probability density function](../../../../../probability-density-function.md) on $(0,1)$, $v>0$ and $w>0$. All relevant [moments](../../../../../moment.md) exist because the parameter and observations are bounded. The [binomial distribution](../../../../../binomial-distribution.md) gives

$$
\mathbb E[X_i\mid\theta]=\theta,\qquad
\operatorname{Var}(X_i\mid\theta)=\frac{\theta(1-\theta)}{m_i}.
$$

The [law of total expectation](../../../../../law-of-total-expectation.md), [law of total variance](../../../../../law-of-total-variance.md) and [law of total covariance](../../../../../law-of-total-covariance.md) consequently yield

$$
\mathbb E X_i=\eta,\quad
\operatorname{Var}(X_i)=v+\frac{w}{m_i},\quad
\operatorname{Cov}(X_i,X_j)=v\ (i\ne j),\quad
\operatorname{Cov}(\theta,X_i)=v.
$$

In particular, [conditional independence](../../../../../conditional-independence.md) of the annual observations does not imply unconditional [independence](../../../../../independent-random-variables.md): they share the uncertain parameter.

To derive the optimal [credibility estimate](../../../../../credibility-estimate.md) among [affine functions](../../../../../affine-function.md) of the observations, put $A=\sum_i a_i$ and write $X_i=\theta+\varepsilon_i$. The conditional errors have zero [conditional expectation](../../../../../conditional-expectation.md), [conditional variance](../../../../../conditional-variance.md) $\theta(1-\theta)/m_i$, and zero pairwise conditional [covariances](../../../../../covariance.md). They are also uncorrelated with every integrable function of $\theta$. Therefore the joint [mean squared error](../../../../../mean-squared-error.md) is

$$
\begin{aligned}
L(a_0,a_1,\ldots,a_n)
&=\mathbb E\left[\big((1-A)\theta-a_0-\sum_i a_i\varepsilon_i\big)^2\right]\\
&=((1-A)\eta-a_0)^2+v(1-A)^2+w\sum_i\frac{a_i^2}{m_i}.
\end{aligned}
$$

For fixed slopes, the first term is uniquely minimized by $a_0=(1-A)\eta$. For fixed sum $A$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
A^2=\left(\sum_i\frac{a_i}{\sqrt{m_i}}\sqrt{m_i}\right)^2
\le M\sum_i\frac{a_i^2}{m_i},
$$

with equality exactly when $a_i=A m_i/M$. Thus the remaining optimization is the strictly convex quadratic

$$
v(1-A)^2+\frac{w}{M}A^2.
$$

Its derivative vanishes at $A=Mv/(Mv+w)$. Consequently the [Bühlmann–Straub credibility estimate](../../../../../buhlmann-straub-credibility-estimate.md) is

$$
\boxed{\widehat\theta=Z\frac{\sum_i m_iX_i}{M}+(1-Z)\eta,\qquad
Z=\frac{Mv}{Mv+w}=\frac{M}{M+w/v}.}
$$

The individual coefficients are $a_i=Zm_i/M$ and $a_0=(1-Z)\eta$. The strict quadratic minimizations establish global optimality and uniqueness, not just necessary equations. Here $v$ is the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md), $w$ is the [expected process variance](../../../../../expected-process-variance.md), and $Z$ is the [Bühlmann–Straub credibility factor](../../../../../buhlmann-straub-credibility-factor.md). More exposure gives more weight to the observed claim fraction. Since $0<Z<1$, the estimate remains between the observed pooled fraction and the prior [expected value](../../../../../expected-value.md). If one separately permits a degenerate prior, $v=0$ leads to the constant estimate $\eta$, interpreted as $Z=0$.

For the [uniform distribution](../../../../../continuous-uniform-distribution.md) prior on $(0,1)$,

$$
\eta=\frac12,\qquad v=\frac1{12},\qquad
w=\int_0^1\theta(1-\theta)\,d\theta=\frac16.
$$

With two years, put $M=m_1+m_2$ and $s=Y_1+Y_2=m_1X_1+m_2X_2$. Then $Z=M/(M+2)$ and

$$
\boxed{\widehat\theta=\frac{s+1}{M+2}
=\frac{m_1X_1+m_2X_2+1}{m_1+m_2+2}.}
$$

To compare with the [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md), use [conditional independence](../../../../../conditional-independence.md) to multiply the two binomial [likelihood functions](../../../../../likelihood-function.md). Terms independent of $\theta$ cancel on normalization, and the uniform prior makes the [posterior density](../../../../../posterior-density.md) proportional to $\theta^s(1-\theta)^{M-s}$. Hence [Beta-binomial conjugacy](../../../../../beta-binomial-conjugacy.md) gives

$$
\theta\mid(Y_1,Y_2)\sim\operatorname{Beta}(s+1,M-s+1),\qquad
\mathbb E[\theta\mid Y_1,Y_2]=\frac{s+1}{M+2}.
$$

Finally, for an arbitrary reported value $d$, conditional [quadratic loss](../../../../../squared-error-loss.md) decomposes as

$$
\mathbb E[(\theta-d)^2\mid Y_1,Y_2]
=\operatorname{Var}(\theta\mid Y_1,Y_2)
+\big(d-\mathbb E[\theta\mid Y_1,Y_2]\big)^2.
$$

The unique minimum is the [posterior mean](../../../../../posterior-mean.md). Therefore **the affine [credibility estimate](../../../../../credibility-estimate.md) and the exact Bayesian estimate coincide** in this case. The agreement illustrates [exact beta-binomial credibility with unequal exposures](../../../../../exact-beta-binomial-credibility-with-unequal-exposures.md); for a general [prior distribution](../../../../../prior-probability.md), minimizing over [affine functions](../../../../../affine-function.md) of the observations need not recover the unrestricted [posterior mean](../../../../../posterior-mean.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
