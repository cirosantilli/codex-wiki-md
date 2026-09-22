<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [P-star approximation](../../../../../p-star-approximation.md) describes the sampling [density](../../../../../density.md) of a regular [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) in sample coordinates consisting of the fitted parameter $\widehat\theta$ and a suitable [ancillary statistic](../../../../../ancillary-statistic.md) $a$. For a $d$-dimensional parameter, write $\ell(\theta;\widehat\theta,a)$ for the [log-likelihood](../../../../../log-likelihood.md) expressed in these coordinates, and $j(\widehat\theta;\widehat\theta,a)$ for the fitted [observed information](../../../../../observed-fisher-information.md). The approximation is

$$
p^*(\widehat\theta\mid a;\theta)=c(\theta,a)|j(\widehat\theta;\widehat\theta,a)|^{1/2}\exp\{\ell(\theta;\widehat\theta,a)-\ell(\widehat\theta;\widehat\theta,a)\}.
$$

The [determinant](../../../../../determinant.md) factor supplies the local volume scale, while the exponential retains the full [likelihood ratio](../../../../../likelihood-ratio.md), rather than replacing it by a quadratic. The [normalizing constant](../../../../../normalizing-constant.md) is chosen by integrating over the fitted-parameter coordinates; its leading regular large-sample value is $(2\pi)^{-d/2}$. These ingredients arise from a [statistical saddlepoint approximation](../../../../../saddlepoint-density-approximation.md). Their use requires an interior, locally unique fit, nonsingular information and suitable smoothness; an [ancillary statistic](../../../../../ancillary-statistic.md) specifies the conditioning surface when the fit alone does not exhaust the relevant sample coordinates. In a regular model the unnormalized leading expression has relative error of order $n^{-1}$ locally; normalization and conditioning matter for refined inference. It is not a universal exact [density](../../../../../density.md). Under a smooth one-to-one parameter transformation, the [Hessian](../../../../../hessian-matrix.md) at the fit transforms without a score term, so its [determinant](../../../../../determinant.md) supplies precisely the [density](../../../../../density.md) [Jacobian determinant](../../../../../jacobian-determinant.md). This proves the invariance of the construction under one-to-one changes of [statistical parameters](../../../../../statistical-parameter.md).

Here put $S=\sum_iX_i$ and $T=\sum_iY_i$. The [log-likelihood](../../../../../log-likelihood.md), apart from a data-only constant, is

$$
\ell(\psi,\lambda)=n\log\psi+2n\log\lambda-\lambda S-\psi\lambda T.
$$

The two [score equations](../../../../../score-equation.md) give

$$
\boxed{\widehat\lambda=\frac nS,\qquad\widehat\psi=\frac ST.}
$$

The sample sums form a [sufficient statistic](../../../../../sufficient-statistic.md), and there is no need to retain an additional ancillary in calculating their joint [density](../../../../../density.md). Inverting the fitted coordinates gives $S=n/\widehat\lambda$ and $T=n/(\widehat\psi\widehat\lambda)$. With parameter order $(\psi,\lambda)$, the fitted [observed information](../../../../../observed-fisher-information.md) is

$$
j(\widehat\psi,\widehat\lambda)=\begin{pmatrix}n/\widehat\psi^2&n/(\widehat\psi\widehat\lambda)\\n/(\widehat\psi\widehat\lambda)&2n/\widehat\lambda^2\end{pmatrix},\qquad |j|^{1/2}=\frac n{\widehat\psi\widehat\lambda}.
$$

Also,

$$
\ell(\psi,\lambda)-\ell(\widehat\psi,\widehat\lambda)=n\log\frac\psi{\widehat\psi}+2n\log\frac\lambda{\widehat\lambda}-\frac{n\lambda}{\widehat\lambda}\left(1+\frac\psi{\widehat\psi}\right)+2n.
$$

Thus the required joint [P-star approximation](../../../../../p-star-approximation.md) is

$$
\boxed{p^*(\widehat\psi,\widehat\lambda)=\frac{c_n n e^{2n}\psi^n\lambda^{2n}}{\widehat\psi^{n+1}\widehat\lambda^{2n+1}}\exp\left\{-\frac{n\lambda}{\widehat\lambda}\left(1+\frac\psi{\widehat\psi}\right)\right\},\quad \widehat\psi,\widehat\lambda>0.}
$$

To integrate out $\widehat\lambda$, substitute $u=b/\widehat\lambda$ in

$$
\int_0^\infty v^{-2n-1}e^{-b/v}\,dv=\frac{\Gamma(2n)}{b^{2n}}.
$$

Taking $b=n\lambda(1+\psi/\widehat\psi)$ and rearranging the powers yields

$$
p^*(\widehat\psi)=\frac{c_ne^{2n}n^{1-2n}\Gamma(2n)}\psi\left(\frac{\widehat\psi}\psi\right)^{n-1}\left(1+\frac{\widehat\psi}\psi\right)^{-2n}.
$$

The [beta function](../../../../../beta-function.md) identity $\int_0^\infty z^{n-1}(1+z)^{-2n}\,dz=\Gamma(n)^2/\Gamma(2n)$ therefore gives

$$
\boxed{c_n=\frac{n^{2n-1}e^{-2n}}{\Gamma(n)^2},\qquad p^*(\widehat\psi)=\frac{\Gamma(2n)}{\Gamma(n)^2\psi}\left(\frac{\widehat\psi}\psi\right)^{n-1}\left(1+\frac{\widehat\psi}\psi\right)^{-2n}.}
$$

Both normalized approximations are actually exact. To check the joint assertion independently, $S$ and $T$ have independent [gamma distributions](../../../../../gamma-distribution.md) with shape $n$ and rates $\lambda$ and $\psi\lambda$. Their joint [density](../../../../../density.md) is $\psi^n\lambda^{2n}S^{n-1}T^{n-1}e^{-\lambda S-\psi\lambda T}/\Gamma(n)^2$. The inverse-coordinate [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\left|\frac{\partial(S,T)}{\partial(\widehat\psi,\widehat\lambda)}\right|=\frac{n^2}{\widehat\psi^2\widehat\lambda^3},
$$

which reproduces the normalized joint expression. This is the [P-star density for two exponential rates](../../../../../p-star-density-for-two-exponential-rates.md); its marginal gives the stated [F-distribution](../../../../../f-distribution.md). [Stirling's approximation](../../../../../stirling-formula.md) gives $c_n=(2\pi)^{-1}(1-1/(6n)+O(n^{-2}))$, so using only the leading normalizer retains the exact shape but not its exact total mass.

The original PDF's displayed [density](../../../../../density.md) constant is missing a square on $\Gamma(n)$. Its printed expression integrates to $\Gamma(n)$, rather than one in general. The normalized [density](../../../../../density.md) above is the one consistent with the stated [F-distribution](../../../../../f-distribution.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
