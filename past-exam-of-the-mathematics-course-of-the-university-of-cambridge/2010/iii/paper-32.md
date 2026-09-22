# Paper 32

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper32.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper32.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $G=X^TX$ and $H=XG^{-1}X^T$. The [rank of a matrix](../../../vector-space.md#matrix-rank) assumption makes $G$ invertible, and $H$ is the [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) onto the column space of the [design matrix](../../../linear-regression.md#design-matrix). The [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood) has [log-likelihood](../../../statistical-modelling.md#log-likelihood)

$$
\ell(b,v)=-\frac n2\log(2\pi v)-\frac{\|Y-Xb\|^2}{2v},\qquad v>0.
$$

Minimizing the squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) gives the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) normal equations $G\widehat\beta=X^TY$. Maximizing over $v$ then gives the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator)

$$
\boxed{\widehat\beta=G^{-1}X^TY,\qquad \widehat\sigma^2=\frac{\mathrm{RSS}}n,\qquad \mathrm{RSS}=Y^T(I-H)Y.}
$$

The divisor for the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) of the [variance](../../../variance.md) is $n$, whereas the unbiased residual [variance](../../../variance.md) estimate is $s^2=\mathrm{RSS}/(n-p)$. The exceptional event $\mathrm{RSS}=0$ has probability zero under the [Gaussian linear model](../../../statistical-modelling.md#normal-linear-model) with $\sigma^2>0$; on that event the [likelihood](../../../statistical-modelling.md#likelihood-function) is unbounded as $v\downarrow0$.

For the joint [sampling distribution](../../../statistical-modelling.md#sampling-distribution), write $\widehat\beta-\beta=G^{-1}X^T\epsilon$ and $Y-X\widehat\beta=(I-H)\epsilon$. Their cross-[covariance matrix](../../../variance.md#covariance-matrix) vanishes because $X^T(I-H)=0$. These two vectors are jointly [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution), so they are [independent random variables](../../../random-variable.md#independent-random-variables). The residual [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) has rank $n-p$, hence the standard [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) result gives

$$
\boxed{\widehat\beta\sim N_p(\beta,\sigma^2G^{-1}),\qquad \frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p},\qquad \widehat\beta\ \text{and}\ \widehat\sigma^2\ \text{independent}.}
$$

Thus these two displayed marginal laws, with their [independence](../../../random-variable.md#independent-random-variables), specify the full joint distribution.

The [quadratic form](../../../linear-algebra.md#quadratic-form)

$$
\frac{(\widehat\beta-\beta)^TG(\widehat\beta-\beta)}{\sigma^2}
$$

has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $p$ degrees of freedom and is independent of $\mathrm{RSS}/\sigma^2$. Their ratio therefore supplies the exact [F-distribution](../../../continuous-probability-distribution.md#f-distribution) pivot

$$
T(\beta)=\frac{(\widehat\beta-\beta)^TG(\widehat\beta-\beta)/p}{\mathrm{RSS}/(n-p)}\sim F_{p,n-p}.
$$

If $f_{1-\alpha}$ is the $(1-\alpha)$ quantile of that [F-distribution](../../../continuous-probability-distribution.md#f-distribution), inversion gives the [normal linear-model confidence ellipsoid](../../../statistical-modelling.md#normal-linear-model-confidence-ellipsoid)

$$
\boxed{C_{1-\alpha}(Y)=\{b\in\mathbb R^p:(\widehat\beta-b)^TG(\widehat\beta-b)\le p s^2 f_{1-\alpha}\}.}
$$

For every $\beta$ and every $\sigma^2>0$, the probability that this [confidence set](../../../statistical-inference.md#confidence-region) contains $\beta$ is exactly $1-\alpha$. To test the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), reject precisely when $\beta_0$ lies outside this [confidence ellipsoid](../../../statistical-inference.md#confidence-ellipsoid), equivalently when $T(\beta_0)>f_{1-\alpha}$. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) the rejection probability is exactly $\alpha$, independent of the unknown [variance](../../../variance.md).

For the numerical calculation, the second column of the [design matrix](../../../linear-regression.md#design-matrix) sums to zero and its sum of squares is $60$. Direct calculation from the observations gives

$$
G=\begin{pmatrix}9&0\\0&60\end{pmatrix},\qquad X^TY=\begin{pmatrix}0\\30\end{pmatrix},\qquad Y^TY=22.
$$

Consequently the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimate, [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) and unbiased residual [variance](../../../variance.md) are

$$
\widehat\beta=\begin{pmatrix}0\\1/2\end{pmatrix},\qquad \mathrm{RSS}=22-(X^TY)^TG^{-1}(X^TY)=22-15=7,\qquad s^2=7/7=1.
$$

The [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) of the [variance](../../../variance.md) is instead $7/9$. At the proposed null value the [F-distribution](../../../continuous-probability-distribution.md#f-distribution) statistic is

$$
\boxed{T(0)=\frac{15/2}{7/7}=7.5>4.74.}
$$

Therefore **reject the null hypothesis at the 5% level**. The relevant critical value has $2$ numerator and $7$ residual degrees of freedom.

## 2

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

One sufficient [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) [statistical consistency](../../../statistical-inference.md#consistency-statistics) theorem is the following. Let the observations be [independent random variables](../../../random-variable.md#independent-random-variables) with a common density $f_\theta$ relative to a fixed measure, let $\Theta$ be a compact metric parameter set containing the true value $\theta_0$, and suppose that the expected [log-likelihood](../../../statistical-modelling.md#log-likelihood)

$$
m(\theta)=\mathbb E_{\theta_0}\log f_\theta(Y_1)
$$

is finite, continuous, and uniquely maximized at $\theta_0$. Assume also the [uniform law of large numbers](../../../convergence-of-random-variables.md#uniform-law-of-large-numbers)

$$
\sup_{\theta\in\Theta}\left|\frac1n\sum_{i=1}^n\log f_\theta(Y_i)-m(\theta)\right|\xrightarrow{\mathbb P}0,
$$

and assume that a measurable global [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) exists. Then **every such maximum-likelihood estimator converges in probability to the true parameter**. A useful sufficient condition for this [uniform law of large numbers](../../../convergence-of-random-variables.md#uniform-law-of-large-numbers) is almost-sure continuity of $\theta\mapsto\log f_\theta(Y_1)$ on the compact parameter set and an integrable envelope $\sup_\theta|\log f_\theta(Y_1)|\le M(Y_1)$, $\mathbb E_{\theta_0}M(Y_1)<\infty$. Under these conditions, [identifiability](../../../statistical-model.md#identifiability) supplies uniqueness through the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) identity

$$
m(\theta_0)-m(\theta)=D_{\mathrm{KL}}(f_{\theta_0}\|f_\theta)\ge0,
$$

with equality only at $\theta=\theta_0$.

To see the [statistical consistency](../../../statistical-inference.md#consistency-statistics) conclusion, fix $\varepsilon>0$. Compactness and the unique maximum give a strictly positive separation gap

$$
\delta_\varepsilon=m(\theta_0)-\sup_{d(\theta,\theta_0)\ge\varepsilon}m(\theta)>0
$$

whenever the set outside the neighbourhood is nonempty. If $\Delta_n$ denotes the supremum discrepancy in the [uniform law of large numbers](../../../convergence-of-random-variables.md#uniform-law-of-large-numbers), maximization of the empirical [log-likelihood](../../../statistical-modelling.md#log-likelihood) yields

$$
0\le m(\theta_0)-m(\widehat\theta_n)\le2\Delta_n.
$$

Hence the probability of $d(\widehat\theta_n,\theta_0)\ge\varepsilon$ is at most $\mathbb P(2\Delta_n\ge\delta_\varepsilon)$, which tends to zero. This is the [argmin consistency under uniform convergence in probability](../../../statistical-inference.md#argmin-consistency-under-uniform-convergence-in-probability) argument applied to the negative [log-likelihood](../../../statistical-modelling.md#log-likelihood). These are sufficient conditions, not necessary ones; parameter-dependent support can require a direct argument, and independent observations need not have a common distribution in other models.

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

The [likelihood function](../../../statistical-modelling.md#likelihood-function) for the shifted [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) is

$$
L_n(\theta)=\exp\left(n\theta-\sum_{i=1}^nY_i\right)\mathbf1\{\theta\le Y_{(1)}\},\qquad Y_{(1)}=\min_iY_i.
$$

It increases strictly up to the smallest observation and is zero beyond it. Thus [shifted exponential maximum likelihood](../../../statistical-modelling.md#shifted-exponential-maximum-likelihood) gives

$$
\boxed{\widehat\theta_n=Y_{(1)}.}
$$

For $t\ge0$, [independence](../../../random-variable.md#independent-random-variables) and the survival function of the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) give the exact [order statistic](../../../probability-theory.md#order-statistic) law

$$
\mathbb P_\theta(\widehat\theta_n-\theta>t)=\prod_{i=1}^n\mathbb P_\theta(Y_i-\theta>t)=e^{-nt}.
$$

In particular, $\widehat\theta_n\ge\theta$ almost surely and $\mathbb P_\theta(|\widehat\theta_n-\theta|>\varepsilon)=e^{-n\varepsilon}\to0$. This proves [statistical consistency](../../../statistical-inference.md#consistency-statistics). The [exact endpoint limit for a shifted exponential distribution](../../../statistical-modelling.md#exact-endpoint-limit-for-a-shifted-exponential-distribution) is stronger than an asymptotic approximation:

$$
\boxed{n(\widehat\theta_n-\theta)\sim\operatorname{Exp}(1)\ \text{for every }n,\qquad n(\widehat\theta_n-\theta)\xrightarrow{d}\operatorname{Exp}(1).}
$$

The limit is one-sided and nonnormal; the moving support endpoint explains why a regular square-root-$n$ [asymptotic normality of a maximum likelihood estimator](../../../statistical-modelling.md#asymptotic-normality-of-a-maximum-likelihood-estimator) theorem does not apply here.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

Set $S_n=\sum_{i=1}^nY_i$ and $a_n=\sum_{i=1}^n2^{-i}=1-2^{-n}$. For the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) observations, factors independent of $\theta$ can be removed from the [likelihood function](../../../statistical-modelling.md#likelihood-function), leaving

$$
L_n(\theta)\propto\theta^{S_n}e^{-a_n\theta},\qquad \ell_n(\theta)=S_n\log\theta-a_n\theta+\text{constant}.
$$

When $S_n>0$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) derivative is $S_n/\theta-a_n$ and its second derivative is negative. The unique positive [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is therefore

$$
\boxed{\widehat\theta_n=\frac{S_n}{1-2^{-n}}\quad(S_n>0).}
$$

There is a genuine boundary qualification: if $S_n=0$, the [likelihood](../../../statistical-modelling.md#likelihood-function) decreases strictly on $\theta>0$, so **no maximum is attained in the stated open parameter space**. On the closure $\theta\ge0$, its maximizer is $0$. Defining the usual extended [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) by the same displayed formula for every $S_n$ allows its [statistical consistency](../../../statistical-inference.md#consistency-statistics) to be examined; the all-zero event cannot be ignored because its probability does not tend to zero.

Indeed, sums of independent [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) variables give $S_n\sim\operatorname{Poi}(\theta a_n)$, so

$$
\mathbb P_\theta\bigl(|\widehat\theta_n-\theta|>\theta/2\bigr)\ge\mathbb P_\theta(S_n=0)=e^{-\theta a_n}\longrightarrow e^{-\theta}>0.
$$

Thus **the extended maximum-likelihood estimator is inconsistent**. More precisely, $S_n$ increases to $S_\infty=\sum_{i\ge1}Y_i$, and $\mathbb E S_\infty=\theta<\infty$ shows that this total count is finite almost surely. Its distribution is [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\theta$, by taking limits of the finite-sum laws. Hence

$$
\widehat\theta_n\longrightarrow S_\infty\sim\operatorname{Poi}(\theta)\quad\text{almost surely}.
$$

This [finite-exposure Poisson inconsistency](../../../statistical-modelling.md#finite-exposure-poisson-inconsistency) leaves a nondegenerate random limit even with infinitely many observations. Correspondingly, the total [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) is $a_n/\theta\to1/\theta$, rather than diverging. The common-distribution hypothesis in the introductory [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) theorem is absent here.

## 3

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In a [linear regression](../../../linear-regression.md) model, a large number of predictors or nearly dependent columns of the [design matrix](../../../linear-regression.md#design-matrix) can make some [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $G=X^TX$ small. The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimate has [covariance matrix](../../../variance.md#covariance-matrix) $\sigma^2G^{-1}$, so these directions have large [variance](../../../variance.md), even though the estimator is unbiased. [Ridge regression](../../../linear-regression.md#ridge-regression) reduces this [variance](../../../variance.md) by shrinking the estimate towards zero, at the cost of introducing [bias](../../../statistical-modelling.md#bias-of-an-estimator). This [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff) can improve the [mean squared error](../../../statistical-modelling.md#mean-squared-error) when the signal is not too large in the shrunken directions.

For the usual preprocessing with a [regression intercept](../../../linear-regression.md#regression-intercept), separate the constant column from the predictors and leave the intercept unpenalized. Subtract the [sample mean](../../../variance.md#sample-mean) from the response and from each nonconstant predictor, then divide each centered predictor column by its positive scale, for example its [Euclidean norm](../../../functional-analysis.md#euclidean-norm). Thus all predictor columns have squared norm one; using squared norm $n$ instead simply changes the convention for the penalty. Centering is performed on the slope columns, not on the constant column. A full-rank design containing an intercept retains full rank on its centered slope columns. A model without an intercept should retain its specified mean structure unless an intercept is deliberately introduced.

Let $Z$ be the resulting scaled, centered slope [design matrix](../../../linear-regression.md#design-matrix), let $Y_c$ be the centered response, and let $b$ denote the coefficients in these standardized coordinates. The [ridge regression](../../../linear-regression.md#ridge-regression) problem is

$$
\min_{b\in\mathbb R^q}\bigl\{\|Y_c-Zb\|^2+\lambda\|b\|^2\bigr\},\qquad \lambda>0.
$$

Here $q$ is the number of slopes; it is one less than the original number of columns when a constant column was present. The [gradient](../../../calculus.md#gradient) of this objective is $2(Z^TZ+\lambda I)b-2Z^TY_c$. Its [Hessian matrix](../../../calculus.md#hessian-matrix) is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), giving the unique [closed-form ridge regression estimator](../../../linear-regression.md#closed-form-ridge-regression-estimator)

$$
\boxed{\widehat b_\lambda^R=(Z^TZ+\lambda I)^{-1}Z^TY_c.}
$$

The [regression intercept](../../../linear-regression.md#regression-intercept) in the original coordinates is recovered as $\widehat a=\overline Y-\sum_j\overline X_j\widehat b_j/s_j$, and the original slopes are $\widehat\beta_j=\widehat b_j/s_j$, where $s_j$ is the scale used for column $j$. This is the [unpenalized intercept in ridge regression](../../../linear-regression.md#unpenalized-intercept-in-ridge-regression) convention. For a fixed full-rank coefficient design written simply as $X$, with response $Y$ and coefficient $\beta$, the same formula reads

$$
\boxed{\widehat\beta_\lambda^R=(X^TX+\lambda I)^{-1}X^TY.}
$$

The risk comparison below first uses the fixed coefficient coordinates in which this quadratic penalty is imposed, and then addresses reversal of the scaling.

Assume at least one penalized coefficient, zero-mean errors with [covariance matrix](../../../variance.md#covariance-matrix) $\sigma^2I$, and $\sigma^2>0$. No [normal distribution](../../../probability-theory.md#normal-distribution) assumption is needed for this [mean squared error](../../../statistical-modelling.md#mean-squared-error) calculation. Put $G=X^TX$ and $A_\lambda=(G+\lambda I)^{-1}$. The [covariance and bias of a ridge regression estimator](../../../linear-regression.md#covariance-and-bias-of-a-ridge-regression-estimator) follow directly from its linear expression:

$$
\mathbb E\widehat\beta_\lambda^R-\beta=-\lambda A_\lambda\beta,\qquad
\operatorname{Cov}(\widehat\beta_\lambda^R)=\sigma^2A_\lambda G A_\lambda.
$$

For the centered slope model, the response errors have [covariance matrix](../../../variance.md#covariance-matrix) $\sigma^2C$, where $C=I-\mathbf1\mathbf1^T/n$. Since $CZ=Z$, the same coefficient [covariance matrix](../../../variance.md#covariance-matrix) formula still holds with $X=Z$.

By the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices), write $G=Q\operatorname{diag}(d_1,\ldots,d_q)Q^T$, with $Q$ orthogonal and every $d_j>0$, and put $\gamma=Q^T\beta$. The [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error) now gives

$$
\mathcal R(\lambda)=\mathbb E\|\widehat\beta_\lambda^R-\beta\|^2
=\sum_{j=1}^q\frac{\lambda^2\gamma_j^2+\sigma^2d_j}{(d_j+\lambda)^2},\qquad
\mathcal R(0)=\sigma^2\sum_{j=1}^q\frac1{d_j}.
$$

The expression at $\lambda=0$ is the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) [mean squared error](../../../statistical-modelling.md#mean-squared-error). Its right derivative is

$$
\mathcal R'(0)=-2\sigma^2\sum_{j=1}^q\frac1{d_j^2}<0.
$$

Therefore, for every fixed coefficient vector, **all sufficiently small positive penalties strictly improve mean squared error**.

An explicit sufficient choice follows by subtracting the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) risk term by term:

$$
\mathcal R(\lambda)-\mathcal R(0)
=\sum_{j=1}^q\frac{\lambda\left(\lambda\gamma_j^2-2\sigma^2-\lambda\sigma^2/d_j\right)}{(d_j+\lambda)^2}.
$$

Since $\gamma_j^2\le\|\beta\|^2$, every summand is negative whenever

$$
\boxed{\lambda>0,\qquad\lambda\|\beta\|^2<2\sigma^2.}
$$

When $\beta=0$, every positive penalty works. This is a pointwise result: the permitted penalty may depend on the true coefficient vector. A fixed positive penalty cannot improve risk for all arbitrarily large signals, because its squared [bias](../../../statistical-modelling.md#bias-of-an-estimator) grows quadratically with the signal. The same distinction appears in [uniform directional risk improvement by ridge regression](../../../linear-regression.md#uniform-directional-risk-improvement-by-ridge-regression) and [unbounded directional risk of fixed ridge shrinkage](../../../linear-regression.md#unbounded-directional-risk-of-fixed-ridge-shrinkage). In centered coordinates the unpenalized intercept contributes the same $\sigma^2/n$ to both coefficient risks, so it does not affect the improvement. Reversing a fixed predictor scaling measures coefficient error with a fixed [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $W$ instead of the [identity matrix](../../../vector-space.md#identity-matrix). For this weighted loss the squared [bias](../../../statistical-modelling.md#bias-of-an-estimator) still has derivative zero at $\lambda=0$, while the [variance](../../../variance.md) term has derivative

$$
-2\sigma^2\operatorname{tr}(WG^{-2})<0.
$$

The inequality follows because $\operatorname{tr}(WG^{-2})=\operatorname{tr}(G^{-1}WG^{-1})>0$. Thus sufficiently small penalties also improve the original-coordinate [mean squared error](../../../statistical-modelling.md#mean-squared-error), though the explicit sufficient bound above was for the unweighted coordinates. Recovering an uncentered intercept adds a fixed nonnegative quadratic form to the slope loss, and its sample-mean error is uncorrelated with the centered slope errors, so the same weighted argument applies. A model with only an unpenalized intercept gives identical estimators. If the noise [variance](../../../variance.md) were zero, the strict improvement assertion would fail; positive noise [variance](../../../variance.md) is essential.

## 4

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $R$ be the total number of rejected [null hypotheses](../../../statistical-modelling.md#null-hypothesis), and let $V$ count rejected null hypotheses that are in fact true. The [false discovery proportion](../../../statistical-modelling.md#false-discovery-proportion) and [false discovery rate](../../../statistical-modelling.md#false-discovery-rate) are

$$
\boxed{\operatorname{FDP}=\frac{V}{R\vee1},\qquad \operatorname{FDR}=\mathbb E\left[\frac{V}{R\vee1}\right].}
$$

Thus the [false discovery proportion](../../../statistical-modelling.md#false-discovery-proportion) is zero when there are no rejections, and the [false discovery rate](../../../statistical-modelling.md#false-discovery-rate) averages the realized proportion of erroneous rejections.

For the [Benjamini-Hochberg procedure](../../../statistical-modelling.md#benjamini-hochberg-procedure), order the [p-values](../../../statistical-modelling.md#p-value) as $P_{(1)}\le\cdots\le P_{(m)}$ and define

$$
R=\max\bigl(\{k\in\{1,\ldots,m\}:P_{(k)}\le\alpha k/m\}\cup\{0\}\bigr).
$$

Reject every hypothesis whose [p-value](../../../statistical-modelling.md#p-value) satisfies $P_i\le\alpha R/m$ when $R>0$, and reject none otherwise. There are exactly $R$ such hypotheses: if a further [p-value](../../../statistical-modelling.md#p-value) also met the threshold, its larger rank would satisfy its own, still larger, threshold, contradicting maximality. Under the stated [independence](../../../random-variable.md#independent-random-variables) and uniform true-null [p-values](../../../statistical-modelling.md#p-value), this procedure has [false discovery rate](../../../statistical-modelling.md#false-discovery-rate) $\alpha m_0/m\le\alpha$.

For the first modified [Benjamini-Hochberg procedure](../../../statistical-modelling.md#benjamini-hochberg-procedure), remove $P_1$, order the remaining $m-1$ [p-values](../../../statistical-modelling.md#p-value) as $Q_{(1)},\ldots,Q_{(m-1)}$, and use the shifted critical values $\alpha(j+1)/m$. Define its rejection count by

$$
R_{-1}=\max\bigl(\{j\in\{1,\ldots,m-1\}:Q_{(j)}\le\alpha(j+1)/m\}\cup\{0\}\bigr).
$$

Equivalently, insert a zero in place of $P_1$ and run the ordinary [Benjamini-Hochberg procedure](../../../statistical-modelling.md#benjamini-hochberg-procedure) on $m$ values; its total rejection count is $R^{(1)}=R_{-1}+1$. For $r=1,\ldots,m$, the [Benjamini-Hochberg leave-one-out identity](../../../statistical-modelling.md#benjamini-hochberg-leave-one-out-identity) in event form is

$$
\boxed{\{P_1\le\alpha r/m,\ R=r\}=\{P_1\le\alpha r/m,\ R_{-1}=r-1\}.}
$$

To prove it, suppose first that the left event holds. Then $P_1$ is among the rejected values. Lowering it to zero leaves all ordered [p-values](../../../statistical-modelling.md#p-value) at ranks greater than $r$ unchanged, so no new rank can meet its threshold. Rank $r$ still meets its threshold, giving $R^{(1)}=r$. Conversely, if $R^{(1)}=r$ and $P_1\le\alpha r/m$, the $r-1$ rejected remaining values and $P_1$ all meet the original rank-$r$ threshold. Hence the original count is at least $r$. Lowering a [p-value](../../../statistical-modelling.md#p-value) cannot decrease the rejection count, so the original count is also at most $R^{(1)}=r$. This proves equality of the events, including possible ties.

For the second modified [Benjamini-Hochberg procedure](../../../statistical-modelling.md#benjamini-hochberg-procedure), remove both $P_1,P_2$, order the remaining [p-values](../../../statistical-modelling.md#p-value) as $T_{(j)}$, and use shifted critical values $\alpha(j+2)/m$. Its count is

$$
R_{-12}=\max\bigl(\{j\in\{1,\ldots,m-2\}:T_{(j)}\le\alpha(j+2)/m\}\cup\{0\}\bigr).
$$

Replacing $P_1,P_2$ by zeros in the full procedure gives a total of $R^{(12)}=R_{-12}+2$ rejections. The same argument gives the [Benjamini-Hochberg leave-two-out identity](../../../statistical-modelling.md#benjamini-hochberg-leave-two-out-identity), for $r=2,\ldots,m$:

$$
\boxed{\{P_1\le\alpha r/m,\ P_2\le\alpha r/m,\ R=r\}
=\{P_1\le\alpha r/m,\ P_2\le\alpha r/m,\ R_{-12}=r-2\}.}
$$

In the forward direction both replaced values already lie among the first $r$, so ordered ranks greater than $r$ remain unchanged. In the reverse direction reinserting the two values below the rank-$r$ threshold still leaves at least $r$ qualifying values, while monotonicity under lowering bounds the original count above by $r$. For $r=1$, the event of two [p-values](../../../statistical-modelling.md#p-value) meeting the displayed threshold while only one is rejected is empty. For $m=1$ only the first modification is needed.

To calculate the second moment, write $I_i=\mathbf1\{i\text{ rejected}\}$ for a true null. Expanding the square gives

$$
V^2=\sum_{i=1}^{m_0}I_i+\sum_{\substack{1\le i,j\le m_0\\i\ne j}}I_iI_j.
$$

For a true-null index $i$, let $R_{-i}$ denote the first modified count after removing $P_i$. It is a function only of the remaining [p-values](../../../statistical-modelling.md#p-value), and so is independent of the uniform variable $P_i$. The first event identity therefore yields

$$
\mathbb E\frac{I_i}{(R\vee1)^2}
=\sum_{r=1}^m\frac1{r^2}\mathbb P(P_i\le\alpha r/m,\ R_{-i}=r-1)
=\frac\alpha m\sum_{r=1}^m\frac{\mathbb P(R_{-i}=r-1)}r
=\frac\alpha m\mathbb E\frac1{R_{-i}+1}.
$$

For distinct true-null indices $i,j$, the two independent uniform [p-values](../../../statistical-modelling.md#p-value) are independent of the second modified count $R_{-ij}$. The second event identity gives

$$
\mathbb E\frac{I_iI_j}{(R\vee1)^2}
=\sum_{r=2}^m\frac1{r^2}\left(\frac{\alpha r}{m}\right)^2\mathbb P(R_{-ij}=r-2)
=\frac{\alpha^2}{m^2}.
$$

The last sum is one because $R_{-ij}$ always takes a value in $\{0,\ldots,m-2\}$. The ordered pairs in the expansion of $V^2$ number $m_0(m_0-1)$, with no factor of one half.

The true-null [p-values](../../../statistical-modelling.md#p-value) are identically distributed and independent, so permutations among their indices leave the law of the full collection unchanged. Thus every $R_{-i}$ with $i\le m_0$ has the same distribution as $R_{-1}$, even though the false-null [p-values](../../../statistical-modelling.md#p-value) need not be identically distributed. Combining the diagonal and off-diagonal contributions proves the [second moment of the Benjamini-Hochberg false discovery proportion](../../../statistical-modelling.md#second-moment-of-the-benjamini-hochberg-false-discovery-proportion):

$$
\boxed{\mathbb E(\operatorname{FDP}^2)=\frac{\alpha m_0}{m}\mathbb E(A)+\frac{\alpha^2m_0(m_0-1)}{m^2},\qquad A=\frac1{R_{-1}+1}.}
$$

If the first modified count is instead defined to include the inserted zero, the same answer is $A=1/R^{(1)}$. When $m_0=0$, both sides are zero; when $m_0=1$, there are no off-diagonal terms. Finally, repeating the first calculation with denominator $R\vee1$ rather than its square gives $\mathbb E[I_i/(R\vee1)]=\alpha/m$, which verifies the claimed exact [false discovery rate](../../../statistical-modelling.md#false-discovery-rate).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
