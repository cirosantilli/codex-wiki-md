<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md), let $x_i=i/n$ and $K_h(u)=h^{-1}K(u/h)$. The degree-$p$ [local polynomial estimator](../../../../../local-polynomial-regression.md) takes the fitted intercept $\widehat m_h(x;p)=\widehat\beta_0$, where

$$
(\widehat\beta_0,\ldots,\widehat\beta_p)
\in\operatorname*{argmin}_{\beta\in\mathbb R^{p+1}}
\sum_{i=1}^n K_h(x_i-x)\left[Y_i-\sum_{r=0}^p\beta_r(x_i-x)^r\right]^2.
$$

Use a nonnegative [regression kernel](../../../../../kernel-for-nonparametric-regression.md) and an invertible [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md) to obtain a unique fit. For $p=0$, solving the single [weighted least squares](../../../../../weighted-least-squares.md) [normal equation](../../../../../normal-equation.md) gives the [local constant estimator](../../../../../nadaraya-watson-estimator.md):

$$
\boxed{\widehat m_h(x;0)=\frac{\sum_i K_h(x_i-x)Y_i}{\sum_i K_h(x_i-x)}.}
$$

At the interior point $x_0$, use the standard unit-integral [regression kernel](../../../../../kernel-for-nonparametric-regression.md) convention $\mu_0(K)=1$. Otherwise the leading [variance](../../../../../variance-split.md) below is $R(K)/(nh\mu_0(K)^2)$; unlike a [kernel density estimator](../../../../../kernel-density-estimation.md), the [local constant estimator](../../../../../nadaraya-watson-estimator.md) itself is unchanged by rescaling $K$.

The [local constant estimator](../../../../../nadaraya-watson-estimator.md) is a [linear estimator in nonparametric regression](../../../../../linear-estimator-in-nonparametric-regression.md) with weights $W_i=K_h(x_i-x_0)/(ns_{0,h})$. The independent unit-variance errors imply

$$
\operatorname{Var}\{\widehat m_h(x_0;0)\}
=\sum_i W_i^2=\frac{t_{0,h}}{n s_{0,h}^2}
=\frac{R(K)}{nh}+o((nh)^{-1}).
$$

To control the [bias of an estimator](../../../../../bias-of-an-estimator.md), [differentiability](../../../../../differentiability.md) at this one point is enough. Write

$$
m(x_0+u)-m(x_0)=m'(x_0)u+r(u),\qquad
\eta(h):=\sup_{0<|u|\leq h}\frac{|r(u)|}{|u|}\longrightarrow0.
$$

Symmetry makes $\mu_1(K)=0$, and the supplied moment approximation gives $s_{1,h}=o(h)$. Therefore the linear contribution to the [bias of an estimator](../../../../../bias-of-an-estimator.md) is $m'(x_0)s_{1,h}/s_{0,h}=o(h)$. The remaining contribution has absolute value at most $\eta(h)h$, because only $|x_i-x_0|\leq h$ receive positive weight. This is the [interior first-order bias cancellation for local constant regression](../../../../../interior-first-order-bias-cancellation-for-local-constant-regression.md), and gives squared [bias of an estimator](../../../../../bias-of-an-estimator.md) $o(h^2)$. Combining with the [variance](../../../../../variance-split.md) proves

$$
\boxed{\operatorname{MSE}\{\widehat m_h(x_0;0)\}
=\frac{R(K)}{nh}+o\left(h^2+\frac1{nh}\right).}
$$

For fixed $\varepsilon>0$, take $h_\varepsilon=\varepsilon^{-1/3}n^{-1/3}$. It satisfies both asymptotic [smoothing bandwidth](../../../../../smoothing-bandwidth.md) conditions, and the displayed remainder, multiplied by $n^{2/3}$, tends to zero for this fixed $\varepsilon$. Thus

$$
0\leq\limsup_{n\to\infty}n^{2/3}\inf_{h>0}\operatorname{MSE}\{\widehat m_h(x_0;0)\}
\leq R(K)\varepsilon^{1/3}.
$$

Letting $\varepsilon\downarrow0$ proves **the optimized scaled pointwise error tends to zero**. The order of these limits matters: no remainder uniform in $\varepsilon$ has been assumed.

For the lower bound over the whole function class, the absence of a uniform bound on derivatives permits a particularly direct argument. It also avoids assuming a [normal distribution](../../../../../normal-distribution.md) for errors when the model only supplies their first two moments. Fix $n$ and $x_0$. Choose a [smooth bump function](../../../../../smooth-bump-function.md) $b$ on the interval, with $b(x_0)=1$, whose support contains no design point except possibly $x_0$. Such a bump exists because the design is finite; at an endpoint use the restriction of a smooth bump on the real line. Every $m_a=ab$, $a\in\mathbb R$, belongs to the [differentiability](../../../../../differentiability.md) class.

If $x_0$ is not a design point, all observation means are zero for every $a$. The [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) applied to $a=\pm A$ has [total variation distance](../../../../../total-variation-distance.md) zero and gives a lower bound tending to infinity with $A$. In fact, the [supremum](../../../../../supremum.md) of the [mean squared error](../../../../../mean-squared-error.md) is infinite at every such $x_0$.

If $x_0$ is a design point, only its response depends on $a$. The resulting [location family](../../../../../location-family.md) is the single observation $Y=a+\epsilon$; all remaining observations are independent of $a$ and give no extra information. The [single-observation location minimax bound](../../../../../single-observation-location-minimax-bound.md) is

$$
\inf_T\sup_{a\in\mathbb R}\mathbb E\{T(a+\epsilon)-a\}^2=\operatorname{Var}(\epsilon)=1.
$$

Here is a proof covering discrete as well as continuous errors. Give $a$ the [prior distribution](../../../../../prior-probability.md) $U[-A,A]$, independently of the noise. Put $p_M=\mathbb P(|\epsilon|\leq M)$ and $v_M=\operatorname{Var}(\epsilon\mid |\epsilon|\leq M)$. Consider an easier experiment in which an oracle also reveals whether $|\epsilon|\leq M$, and reveals $a$ itself on the complementary event. On the event $|\epsilon|\leq M$ and $|Y|\leq A-M$, every possible truncated noise value places $a=Y-\epsilon$ within $[-A,A]$. The flat [prior distribution](../../../../../prior-probability.md) then makes the [Bayesian posterior](../../../../../bayesian-posterior.md) noise law exactly its truncated original law. The smallest conditional [squared-error loss](../../../../../squared-error-loss.md) is its [conditional variance](../../../../../conditional-variance.md) $v_M$, attained by the [posterior mean](../../../../../posterior-mean.md).

The probability of that event is at least $p_M(1-2M/A)$ for $A>2M$, by restricting further to $|a|\leq A-2M$. Thus every rule's [supremum](../../../../../supremum.md) [risk function](../../../../../risk-function.md) is at least the original [Bayes risk](../../../../../bayes-risk.md), which is at least the easier experiment's [Bayes risk](../../../../../bayes-risk.md), and therefore at least $p_M(1-2M/A)v_M$. Let $A\to\infty$ and then $M\to\infty$. Finite second moment and zero mean give $p_Mv_M\to1$. The rule $T(Y)=Y$ has constant [mean squared error](../../../../../mean-squared-error.md) one, proving the equality.

Consequently, at every $x_0\in[0,1]$, the unrestricted [differentiability](../../../../../differentiability.md) class satisfies the stronger conclusion

$$
\boxed{\sup_{m\in\mathcal F}\mathbb E\{\widetilde m(x_0)-m(x_0)\}^2\geq1\geq n^{-2/3}.}
$$

Thus $c=1$ works for every $n\geq1$. There is no conflict with the preceding fixed-function limit: the worst functions, including arbitrarily narrow bumps, can vary with $n$. This is the [pointwise versus uniform risk distinction](../../../../../pointwise-versus-uniform-risk-distinction.md). A smoothness ball with a common derivative bound would pose a different [minimax risk](../../../../../minimax-risk.md) problem.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
