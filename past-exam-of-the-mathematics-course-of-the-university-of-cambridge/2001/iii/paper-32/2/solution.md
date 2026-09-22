<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Partition the [statistical parameter](../../../../../statistical-parameter.md) as $\theta=(\psi,\lambda)$, with $\psi$ of interest. For each fixed $\psi$, maximize over the [nuisance parameter](../../../../../nuisance-parameter.md) to obtain $\widehat\lambda_\psi$. The [profile likelihood](../../../../../profile-likelihood.md) and [profile log-likelihood](../../../../../profile-log-likelihood.md) are

$$
L_p(\psi)=L(\psi,\widehat\lambda_\psi),\qquad
\ell_p(\psi)=\ell(\psi,\widehat\lambda_\psi).
$$

Their maximizer is the interest component of the joint [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md). At a regular nuisance maximum, $\ell_p'(\psi)=\ell_\psi(\psi,\widehat\lambda_\psi)$ and its negative [Hessian matrix](../../../../../hessian-matrix.md) is the [Schur complement](../../../../../schur-complement.md)

$$
j_p=j_{\psi\psi}-j_{\psi\lambda}j_{\lambda\lambda}^{-1}j_{\lambda\psi}.
$$

The profile [likelihood ratio](../../../../../likelihood-ratio.md) is unchanged by a one-to-one nuisance reparametrization, and transforms naturally under a one-to-one interest reparametrization. Under the regular conditions of [Wilks theorem](../../../../../wilks-theorem.md), $2\{\ell_p(\widehat\psi)-\ell_p(\psi_0)\}$ has a limiting [chi-squared distribution](../../../../../chi-squared-distribution.md) with dimension of $\psi$ degrees of freedom. Profiling is maximization, rather than integration or conditioning; $L_p$ need not be a normalized data density, and nuisance fitting can cause appreciable higher-order distortion.

The [modified profile likelihood](../../../../../modified-profile-likelihood.md) corrects for nuisance curvature and sample-coordinate distortion. In suitable coordinates $(\widehat\psi,\widehat\lambda,a)$, with $a$ an [ancillary statistic](../../../../../ancillary-statistic.md), set

$$
J_\psi=\left|\det\frac{\partial\widehat\lambda_\psi}{\partial\widehat\lambda}\right|,
$$

holding $\widehat\psi,a$ fixed when differentiating the data coordinates. Up to an interest-independent factor, the [Barndorff-Nielsen modified profile likelihood](../../../../../modified-profile-likelihood.md) is

$$
\boxed{L_m(\psi)=L_p(\psi)
|j_{\lambda\lambda}(\psi,\widehat\lambda_\psi)|^{-1/2}J_\psi^{-1}.}
$$

Equivalently, implicit differentiation of the nuisance score equation gives $J_\psi=|j_{\lambda\lambda}|^{-1}|\ell_{\lambda;\widehat\lambda}|$, and

$$
\ell_m=\ell_p+\tfrac12\log|j_{\lambda\lambda}|
-\log|\ell_{\lambda;\widehat\lambda}|.
$$

The semicolon denotes sample-coordinate differentiation, not a second parameter derivative. In orthogonal coordinates, the [Cox-Reid adjusted profile likelihood](../../../../../cox-reid-adjusted-profile-likelihood.md) uses the information adjustment alone; it agrees with this modification when $J_\psi=1$, as happens below.

For the [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md), write $s=\sum_i y_i$, $r=\sum_i y_i^{-1}$ and $\bar y=s/n$. Terms independent of both parameters can be absorbed into $c(y)$, giving

$$
\ell(\psi,\lambda)=c(y)+\frac n2\log\psi
-\frac\psi2\left(r-\frac{2n}{\lambda}+\frac{s}{\lambda^2}\right).
$$

The nuisance [score function](../../../../../informant-function.md) is

$$
\ell_\lambda=\frac{\psi(s-n\lambda)}{\lambda^3}.
$$

It is positive below $\bar y$ and negative above it. Thus its global maximum is

$$
\widehat\lambda_\psi=\widehat\lambda=\bar y,
$$

independent of $\psi$. Put $D=r-n/\bar y$. Then

$$
\boxed{\ell_p(\psi)=\frac n2\log\psi-\frac\psi2D+\text{constant}.}
$$

The nuisance [observed information](../../../../../observed-fisher-information.md) at this fit is

$$
j_{\lambda\lambda}(\psi,\bar y)=\frac{n\psi}{\bar y^3}.
$$

Since the constrained nuisance estimator is literally the full nuisance estimator as a function of the data, $J_\psi=1$ in the specified sample coordinates. Hence the [modified profile likelihood for inverse Gaussian shape](../../../../../modified-profile-likelihood-for-inverse-gaussian-shape.md) is

$$
\boxed{\ell_m(\psi)=\frac{n-1}{2}\log\psi-\frac\psi2D+\text{constant}.}
$$

For $n\ge2$ and a nonconstant positive sample, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $D>0$. The corresponding fits are $\widehat\psi_p=n/D$ and $\widehat\psi_m=(n-1)/D$. A constant sample has $D=0$ and no finite profile maximum; under continuous independent sampling this event has probability zero when $n\ge2$. In particular, the modified coefficient accounts for the fitted mean [nuisance parameter](../../../../../nuisance-parameter.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
