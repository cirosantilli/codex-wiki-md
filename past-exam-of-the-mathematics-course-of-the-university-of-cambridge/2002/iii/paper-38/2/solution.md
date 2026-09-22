<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an interest parameter $\psi$ and [nuisance parameter](../../../../../nuisance-parameter.md) $\lambda$, the [profile likelihood](../../../../../profile-likelihood.md) is $L_p(\psi)=L(\psi,\widetilde\lambda_\psi)$, where $\widetilde\lambda_\psi$ maximizes the [likelihood](../../../../../likelihood-function.md) at fixed $\psi$. Its maximum occurs at the joint [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) of $\psi$. It preserves the optimized [likelihood ratios](../../../../../likelihood-ratio.md) for different interest values and is unchanged by one-to-one reparametrization of the nuisance at each fixed $\psi$. It generally is neither a marginal sampling [density](../../../../../density.md) nor a conditional [likelihood](../../../../../likelihood-function.md), and eliminating [nuisance parameters](../../../../../nuisance-parameter.md) by maximization can introduce appreciable small-sample distortion. Differentiating the constrained [score equation](../../../../../score-equation.md) gives the curvature formula

$$
-\ell_p''=j_{\psi\psi}-j_{\psi\lambda}j_{\lambda\lambda}^{-1}j_{\lambda\psi}
$$

at a joint stationary point. The corresponding expected-information expression is the [efficient information](../../../../../efficient-information.md) for the interest parameter. Under the regular conditions of [Wilks theorem](../../../../../wilks-theorem.md), twice the [profile log-likelihood](../../../../../profile-log-likelihood.md) drop has an asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) with the dimension of the interest parameter as its [degrees of freedom](../../../../../degree-of-freedom.md).

For scalar nuisance, the [Barndorff-Nielsen modified profile likelihood](../../../../../modified-profile-likelihood.md) may be written

$$
\ell_m(\psi)=\ell_p(\psi)-\frac12\log j_{\lambda\lambda}(\psi,\widetilde\lambda_\psi)-\log\left|\frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}\right|,
$$

where the sample-coordinate [derivative](../../../../../derivative.md) holds $\widehat\psi$ and the [ancillary statistic](../../../../../ancillary-statistic.md) fixed. For vector nuisance the last two quantities are [determinants](../../../../../determinant.md). An equivalent form is $\ell_m=\ell_p+\tfrac12\log|j_{\lambda\lambda}|-\log|\ell_{\lambda;\widehat\lambda}|$, since differentiating the constrained nuisance score gives $\ell_{\lambda;\widehat\lambda}=j_{\lambda\lambda}\partial\widetilde\lambda_\psi/\partial\widehat\lambda$. The semicolon denotes differentiation in sample coordinates, not another ordinary parameter [derivative](../../../../../derivative.md). This [Jacobian determinant](../../../../../jacobian-determinant.md) adjustment is essential to the definition.

In the present model set

$$
A(\psi)=\sum_iY_ie^{-\psi x_i},\quad B(\psi)=\sum_i x_iY_ie^{-\psi x_i},\quad C(\psi)=\sum_i x_i^2Y_ie^{-\psi x_i}.
$$

The [log-likelihood](../../../../../log-likelihood.md) is $\ell=-n\log\lambda-\psi\sum_i x_i-A(\psi)/\lambda$. Consequently

$$
\boxed{\widetilde\lambda_\psi=\frac{A(\psi)}n,\qquad\ell_p(\psi)=-n\log\frac{A(\psi)}n-\psi\sum_i x_i-n.}
$$

The profile score is $nB/A-\sum_i x_i$, and its [derivative](../../../../../derivative.md) is $-n(C/A-(B/A)^2)$. The expression in parentheses is the [variance](../../../../../variance-split.md) of the fixed design values under positive weights proportional to $Y_ie^{-\psi x_i}$. Thus the [profile log-likelihood](../../../../../profile-log-likelihood.md) is strictly concave for a nonconstant design. Its score changes from $n\max_i x_i-\sum_i x_i>0$ to $n\min_i x_i-\sum_i x_i<0$ as $\psi$ goes from $-\infty$ to $+\infty$, giving a unique finite fit. If all $x_i$ coincide, only the mean $\lambda e^{\psi x_i}$ is identifiable and inference on $\psi$ alone is not defined; that exceptional design must be excluded.

The specified ancillary coordinates give $Y_i=\widehat\lambda\exp(\widehat\psi x_i+a_i)$. At fixed $\widehat\psi,a$, therefore,

$$
\frac{\partial Y_i}{\partial\widehat\lambda}=\frac{Y_i}{\widehat\lambda},\qquad \frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}=\frac{\widetilde\lambda_\psi}{\widehat\lambda}.
$$

Meanwhile the constrained [observed information](../../../../../observed-fisher-information.md) is

$$
j_{\lambda\lambda}=\left[-\frac n{\lambda^2}+\frac{2A}{\lambda^3}\right]_{\lambda=\widetilde\lambda_\psi}=\frac n{\widetilde\lambda_\psi^2}.
$$

Substitution proves

$$
\boxed{\ell_m(\psi)=\ell_p(\psi)+\log\widehat\lambda-\frac12\log n=\ell_p(\psi)+\text{constant in }\psi.}
$$

Equivalently the sample [derivative](../../../../../derivative.md) of the nuisance score is $\ell_{\lambda;\widehat\lambda}=A/(\lambda^2\widehat\lambda)$, which equals $n/(\widetilde\lambda_\psi\widehat\lambda)$ at the constrained fit and gives the same cancellation. Thus the [modified profile likelihood for exponential regression](../../../../../modified-profile-likelihood-for-exponential-regression.md) is proportional to the ordinary [profile likelihood](../../../../../profile-likelihood.md). This conclusion uses the given ancillary; no proof of its ancillarity is required.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
