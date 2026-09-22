<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Partition a regular parameter as $(\psi,\lambda)$, with interest $\psi$ and nuisance $\lambda$. [Orthogonal statistical parameters](../../../../../../orthogonal-statistical-parameters.md) have zero cross-block of expected [Fisher information](../../../../../../fisher-information-matrix.md),

$$
I_{\psi\lambda}=E(U_\psi U_\lambda^{\mathsf T})=-E\ell_{\psi\lambda}=0.
$$

This may hold at one parameter value or throughout a parametrization. It is expected-information orthogonality, and does not generally force the [observed information](../../../../../../observed-fisher-information.md) cross-block to vanish in each sample.

First, the asymptotic [covariance](../../../../../../covariance.md) of the joint [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is the inverse information. Orthogonality makes this matrix block diagonal, giving first-order asymptotic [independence](../../../../../../independent-random-variables.md) of interest and nuisance fits. The [efficient information](../../../../../../efficient-information.md) with unknown nuisance is

$$
I_{\psi\psi\cdot\lambda}=I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

For orthogonal parameters it equals $I_{\psi\psi}$. Thus estimating the nuisance creates no first-order information loss relative to knowing it, at the orthogonal point. This is a local asymptotic statement, not a general finite-sample [independence](../../../../../../independent-random-variables.md) theorem.

Second, orthogonality stabilizes constrained nuisance estimates. Differentiating $\ell_\lambda(\psi,\widetilde\lambda_\psi)=0$ gives

$$
\frac{d\widetilde\lambda_\psi}{d\psi}=-j_{\lambda\lambda}^{-1}j_{\lambda\psi}.
$$

When the expected cross-information vanishes, regular sampling fluctuations give $j_{\lambda\psi}=O_p(\sqrt n)$ and $j_{\lambda\lambda}=O_p(n)$. The [derivative](../../../../../../derivative.md) is therefore $O_p(n^{-1/2})$ locally. Changing the interest parameter by $O_p(n^{-1/2})$ changes its constrained nuisance fit by only $O_p(n^{-1})$, smaller than the ordinary nuisance estimation error. This reduces sensitivity to how the nuisance is fitted and simplifies higher-order [likelihood](../../../../../../likelihood-function.md) adjustments.

For scalar interest, [local orthogonal nuisance reparametrization](../../../../../../local-orthogonal-nuisance-reparametrization.md) can often be constructed explicitly. Keep $\psi$ and write the original nuisance as $\lambda(\psi,\eta)$. The transformed interest score is $U_\psi+\lambda_\psi^{\mathsf T}U_\lambda$. Its [covariance](../../../../../../covariance.md) with the new nuisance score vanishes when

$$
\frac{\partial\lambda}{\partial\psi}=-I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

With smooth nonsingular nuisance information, this ordinary differential equation has a local solution for suitable initial nuisance coordinates. For several interest coordinates the corresponding equations need compatibility conditions; global orthogonality is not automatic.

The normal model gives a transparent example. For independent observations with mean $\mu$ and [variance](../../../../../../variance-split.md) $\nu$, direct score expectations give

$$
I_{\mu\mu}=\frac n\nu,\qquad I_{\nu\nu}=\frac n{2\nu^2},\qquad I_{\mu\nu}=0.
$$

The cross-information is zero because the centered normal third [moment](../../../../../../moment.md) is zero. When fitting $\nu$ at fixed $\mu$,

$$
\widetilde\nu_\mu=\frac1n\sum_i(X_i-\mu)^2=\widehat\nu+(\mu-\overline X)^2,
$$

so the change is indeed quadratic in a local change of the mean.

Orthogonality is also useful for removing nuisance effects beyond first order. Take [variance](../../../../../../variance-split.md) $\nu$ as interest and mean $\mu$ as nuisance. Put $Q=\sum_i(X_i-\overline X)^2$. The [profile log-likelihood](../../../../../../profile-log-likelihood.md) is $\ell_p(\nu)=-\tfrac n2\log\nu-Q/(2\nu)$ up to a constant. The constrained mean is $\widetilde\mu_\nu=\overline X$ for all $\nu$, so its sample-coordinate [Jacobian determinant](../../../../../../jacobian-determinant.md) is one, and $j_{\mu\mu}=n/\nu$. The information adjustment gives

$$
\boxed{\ell_m(\nu)=\ell_p(\nu)-\tfrac12\log(n/\nu)=-\frac{n-1}2\log\nu-\frac Q{2\nu}+\text{constant}.}
$$

This agrees with the exact [likelihood](../../../../../../likelihood-function.md) based on $Q/\nu\sim\chi^2_{n-1}$: estimating the mean has used one degree of freedom. In this setting the [Cox-Reid adjusted profile likelihood](../../../../../../cox-reid-adjusted-profile-likelihood.md) has the same form. The exact distribution follows by projecting the centered normal vector onto the $(n-1)$-dimensional subspace orthogonal to the constant vector; an [orthonormal basis](../../../../../../orthonormal-basis.md) there supplies $n-1$ independent standard normal coordinates whose squares sum to $Q/\nu$.

The example shows both the benefit and the limits. Orthogonality organizes first-order precision and nuisance stability; it does not eliminate all higher-order nuisance effects. Nor does it identify an [ancillary statistic](../../../../../../ancillary-statistic.md) or justify dropping the sample-coordinate factor in every [modified profile likelihood](../../../../../../modified-profile-likelihood.md). In the exponential regression calculation that factor cancels the information adjustment, so an information-only correction would give a different answer.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
