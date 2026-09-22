<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $u(Y_i;\theta)=\partial_\theta\log f(Y_i;\theta)$ and $U_n(\theta)=\sum_i u(Y_i;\theta)$ for the individual and total [score functions](../../../../../informant-function.md). Under the usual regularity assumptions, $\mathbb E_{\theta_0}u=0$ and $\operatorname{Cov}_{\theta_0}(u)=I(\theta_0)$, the nonsingular per-observation [Fisher information matrix](../../../../../fisher-information-matrix.md). The [central limit theorem](../../../../../central-limit-theorem.md) and [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) give

$$
\frac{U_n(\theta_0)}{\sqrt n}\xrightarrow{d}N_d(0,I(\theta_0)),\qquad \frac{j_n(\theta_0)}n\xrightarrow{p}I(\theta_0).
$$

Rearranging the stipulated score expansion, including its remainder, gives

$$
\sqrt n(\widehat\theta_n-\theta_0)=\left(\frac{j_n(\theta_0)}n\right)^{-1}\frac{U_n(\theta_0)}{\sqrt n}+o_p(1).
$$

[Slutsky theorem](../../../../../slutsky-theorem.md) therefore proves the [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md):

$$
\boxed{\sqrt n(\widehat\theta_n-\theta_0)\xrightarrow{d}N_d(0,I(\theta_0)^{-1}).}
$$

A consistent plug-in [Fisher information matrix](../../../../../fisher-information-matrix.md) yields the [Wald statistic](../../../../../wald-test.md) $W_n=n(\widehat\theta_n-\theta_0)^TI(\widehat\theta_n)(\widehat\theta_n-\theta_0)$. Under the [null hypothesis](../../../../../null-hypothesis.md), $W_n\xrightarrow{d}\chi_d^2$, so a test of asymptotic size $\alpha$ rejects when $W_n$ exceeds the $(1-\alpha)$ [quantile](../../../../../quantile-function.md) of that [chi-squared distribution](../../../../../chi-squared-distribution.md). A consistent [Observed Fisher information](../../../../../observed-fisher-information.md) matrix gives the same limiting test.

With an $r$-dimensional parameter of interest $\psi$ and [nuisance parameter](../../../../../nuisance-parameter.md) $\lambda$, partition $I$ accordingly. The marginal asymptotic [covariance matrix](../../../../../covariance-matrix.md) of $\widehat\psi$ is the $\psi\psi$ block of $I^{-1}$, whose inverse is the [efficient information](../../../../../efficient-information.md)

$$
I_{\rm eff}=I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

Thus the nuisance-adjusted [Wald statistic](../../../../../wald-test.md) is $W_{\psi,n}=n(\widehat\psi-\psi_0)^TI_{\rm eff}(\widehat\theta)(\widehat\psi-\psi_0)$, with limiting null distribution $\chi_r^2$. Using $I_{\psi\psi}$ alone is generally incorrect when the [nuisance parameter](../../../../../nuisance-parameter.md) is estimated; it is valid when the cross-information vanishes.

For the [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) in this problem, expand the exponent to obtain the log [likelihood](../../../../../likelihood-function.md), up to terms independent of both parameters,

$$
\ell_n(\psi,\lambda)=\frac n2\log\psi-\frac\psi2\left(\frac{\sum_iY_i}{\lambda^2}-\frac{2n}{\lambda}+\sum_iY_i^{-1}\right).
$$

Its [score functions](../../../../../informant-function.md) are

$$
U_\lambda=\frac\psi{\lambda^3}(\sum_iY_i-n\lambda),\qquad U_\psi=\frac n{2\psi}-\frac12\left(\frac{\sum_iY_i}{\lambda^2}-\frac{2n}{\lambda}+\sum_iY_i^{-1}\right).
$$

For each positive $\psi$, the first score changes sign from positive to negative at $\lambda=\bar Y$, so this is the global maximizing [mean parameter of an exponential family](../../../../../mean-parameter-of-an-exponential-family.md). Substituting it in the second score gives

$$
\boxed{\widehat\lambda=\bar Y,\qquad\widehat\psi_U=\left(\overline{Y^{-1}}-\frac1{\bar Y}\right)^{-1}.}
$$

The reciprocal function is [strictly convex](../../../../../strictly-convex-function.md), so the denominator is positive for a nonconstant sample. The profile log [likelihood](../../../../../likelihood-function.md) is [strictly concave](../../../../../strictly-concave-function.md) in $\psi$ and tends to minus infinity at both endpoints, proving this is a maximum. Under continuous model sampling, a sample of size at least two is nonconstant [almost surely](../../../../../almost-sure-convergence.md). For a constant sample, including a one-observation sample, no finite joint [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) exists: the [likelihood](../../../../../likelihood-function.md) increases without bound as $\psi\to\infty$ at $\lambda=\bar Y$.

For one observation, differentiating again and using $\mathbb EY=\lambda$ gives

$$
I_{\psi\psi}=\frac1{2\psi^2},\qquad I_{\psi\lambda}=\mathbb E\left(\frac1{\lambda^2}-\frac Y{\lambda^3}\right)=0,\qquad I_{\lambda\lambda}=\psi\mathbb E\left(\frac{3Y}{\lambda^4}-\frac2{\lambda^3}\right)=\frac\psi{\lambda^3}.
$$

This [parameter orthogonality](../../../../../orthogonal-statistical-parameters.md) proves that estimating $\lambda$ does not reduce the [efficient information](../../../../../efficient-information.md) for $\psi$. The [Wald statistic](../../../../../wald-test.md) has the same algebraic form in the two cases:

$$
\boxed{W_\psi=\frac{n(\widehat\psi-\psi_0)^2}{2\widehat\psi^2}\xrightarrow[H_0]{d}\chi_1^2.}
$$

Using information evaluated at $\psi_0$ instead is another first-order equivalent convention.

**The printed claim of coincidence needs a first-order interpretation.** Known and unknown $\lambda$ need not give numerically identical [Wald statistics](../../../../../wald-test.md), because their [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) differ. With $\lambda$ known, direct maximization gives

$$
\widehat\psi_K=\left(\overline{Y^{-1}}-\frac2\lambda+\frac{\bar Y}{\lambda^2}\right)^{-1},\qquad \widehat\psi_K^{-1}-\widehat\psi_U^{-1}=\frac{(\bar Y-\lambda)^2}{\lambda^2\bar Y}.
$$

For example, observations $1,2$ and known $\lambda=1$ give $\widehat\psi_K=4$ and $\widehat\psi_U=12$. At $\psi_0=1$, the displayed Wald convention gives $9/16$ and $121/144$, respectively. Thus exact equality is false. Under the [null hypothesis](../../../../../null-hypothesis.md), however, $\bar Y-\lambda=O_p(n^{-1/2})$, hence $\widehat\psi_K-\widehat\psi_U=O_p(n^{-1})$. Their centered, standardized estimates differ by $o_p(1)$, so their [Wald statistics](../../../../../wald-test.md) differ by $o_p(1)$. This is the valid asymptotic coincidence supplied by [inverse Gaussian shape estimation and nuisance orthogonality](../../../../../inverse-gaussian-shape-estimation-and-nuisance-orthogonality.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
