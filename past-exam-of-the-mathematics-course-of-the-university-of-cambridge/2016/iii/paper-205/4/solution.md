<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\Omega=\Sigma^{-1}$ for a [positive-definite matrix](../../../../../positive-definite-matrix.md). Up to a constant independent of the parameters, the [log-likelihood](../../../../../log-likelihood.md) of the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) is

$$
\ell(\mu,\Omega)=\frac n2\log\det\Omega-\frac12\sum_{i=1}^n(x_i-\mu)^T\Omega(x_i-\mu).
$$

The identity

$$
\sum_i(x_i-\mu)^T\Omega(x_i-\mu)=\sum_i(x_i-\bar X)^T\Omega(x_i-\bar X)+n(\mu-\bar X)^T\Omega(\mu-\bar X)
$$

shows that, for each $\Omega\succ0$, the unique optimizing mean is $\widehat\mu=\bar X$. Using the [matrix trace](../../../../../matrix-trace.md) to rewrite the first quadratic sum, the [profile likelihood](../../../../../profile-likelihood.md) is

$$
\ell_{\mathrm{prof}}(\Omega)=\mathrm{constant}+\frac n2\{\log\det\Omega-\operatorname{tr}(S\Omega)\}.
$$

Therefore [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) of the [precision matrix](../../../../../precision-matrix.md), whenever the maximum exists, is exactly

$$
\boxed{\widehat\Omega\in\mathop{\arg\min}_{\Omega=\Omega^T\succ0}\{-\log\det\Omega+\operatorname{tr}(S\Omega)\}.}
$$

This is the [profile likelihood for a Gaussian precision matrix](../../../../../profile-likelihood-for-a-gaussian-precision-matrix.md). The [sample covariance matrix](../../../../../sample-covariance-matrix.md) here uses divisor $n$, as appropriate for [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md).

There is an important rank qualification in the printed assumptions. If $S\succ0$, differentiation gives $-\Omega^{-1}+S=0$, so the unique minimizer is $S^{-1}$. Uniqueness follows because the negative [log-determinant](../../../../../log-determinant.md) is a [strictly convex function](../../../../../strictly-convex-function.md) on the [positive-definite matrices](../../../../../positive-definite-matrix.md). But [full column rank](../../../../../full-column-rank.md) of the uncentered $X$ alone does not imply $S\succ0$: the [rank of a centered sample covariance matrix](../../../../../rank-of-a-centered-sample-covariance-matrix.md) depends on the centered design. For example, with $n=p=2$ and raw data matrix $X=I_2$,

$$
S=\frac14\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\qquad Sv=0\quad\text{for }v=(1,1)^T.
$$

Although $X$ has [full column rank](../../../../../full-column-rank.md), setting $\Omega_t=I_2+t vv^T$ gives objective $-\log(1+2t)+\operatorname{tr}(S)\to-\infty$. Thus an unpenalized maximizer need not exist under the literal raw-rank assumption. The likelihood reduction remains valid; existence requires [full column rank](../../../../../full-column-rank.md) of the centered data, equivalently $S\succ0$. For the nonsingular Gaussian model this holds almost surely when $n>p$.

Use the entrywise-penalty convention for the [Graphical Lasso](../../../../../graphical-lasso.md):

$$
\boxed{\widehat\Omega_\lambda=\mathop{\arg\min}_{\Omega=\Omega^T\succ0}\left\{-\log\det\Omega+\operatorname{tr}(S\Omega)+\lambda\sum_{r,s=1}^p|\Omega_{rs}|\right\}.}
$$

The sum is the [entrywise matrix L1 norm](../../../../../entrywise-matrix-l1-norm.md). Its [Graphical-Lasso Karush-Kuhn-Tucker conditions](../../../../../graphical-lasso-karush-kuhn-tucker-conditions.md) are

$$
\boxed{S-\widehat\Sigma+\lambda Z=0,\qquad Z_{rs}\in\partial|\widehat\Omega_{\lambda,rs}|,\qquad\widehat\Sigma=\widehat\Omega_\lambda^{-1}.}
$$

Here $Z$ is symmetric; its nonzero-entry values are $\operatorname{sgn}(\widehat\Omega_{\lambda,rs})$, and its zero-entry values are any numbers in $[-1,1]$. These are the [subgradient optimality condition](../../../../../subgradient-optimality-condition.md) for this [convex optimization](../../../../../convex-optimization-split.md) problem. Since a [positive-definite matrix](../../../../../positive-definite-matrix.md) has positive diagonal, $Z_{rr}=1$ and $\widehat\Sigma_{rr}=S_{rr}+\lambda$. Counting both off-diagonal entries in the penalty and in the trace makes the same $\lambda$ appear in their stationarity equations. The common variant penalizing only off-diagonal entries instead sets $Z_{rr}=0$; the off-diagonal equations and the column argument below are unchanged.

For the given column problem, abbreviate

$$
A=\widehat\Sigma_{-j,-j}=W^2,\qquad s_j=S_{-j,j},\qquad v=\widehat\Sigma_{-j,j}.
$$

Its smooth part expands to $\tfrac12 b^TAb-s_j^Tb$ plus a constant, because $W$ is symmetric and $W W^{-1}=I$. The matrix $A$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md), so this quadratic is a [strictly convex function](../../../../../strictly-convex-function.md). Adding the convex [L1 norm](../../../../../l1-norm.md) penalty preserves strict convexity, and the objective tends to infinity as $\|b\|_2\to\infty$. **The minimizer $b^*$ exists and is unique.** Its [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
Ab^*-s_j+\lambda u=0,\qquad u_r\in\partial|b_r^*|.
$$

We identify that minimizer directly from the [precision matrix](../../../../../precision-matrix.md). Write $\widehat\Omega=\widehat\Omega_\lambda$ and define

$$
\widetilde b=-\frac{\widehat\Omega_{-j,j}}{\widehat\Omega_{jj}}.
$$

The denominator is positive. The off-diagonal part of column $j$ of $\widehat\Sigma\widehat\Omega=I$ gives

$$
A\widehat\Omega_{-j,j}+v\widehat\Omega_{jj}=0,\qquad\text{hence }A\widetilde b=v.
$$

On the other hand, the off-diagonal [Graphical-Lasso Karush-Kuhn-Tucker conditions](../../../../../graphical-lasso-karush-kuhn-tucker-conditions.md) read

$$
s_j-v+\lambda Z_{-j,j}=0.
$$

Because $\widehat\Omega_{jj}>0$, the coordinates of $\widetilde b$ have the opposite signs from those of $\widehat\Omega_{-j,j}$ and vanish at exactly the same positions. The [subgradient of the absolute value](../../../../../subgradient-of-the-absolute-value.md) therefore satisfies

$$
-Z_{-j,j}\in\partial\|\widetilde b\|_1.
$$

It follows that

$$
A\widetilde b-s_j+\lambda(-Z_{-j,j})=v-s_j-\lambda Z_{-j,j}=0.
$$

These are exactly the [Lasso](../../../../../lasso.md) column problem's [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md). Its unique minimizer must be $b^*=\widetilde b$, yielding

$$
\boxed{\widehat\Sigma_{-j,j}=\widehat\Sigma_{-j,-j}b^*,\qquad b^*=-\frac{\widehat\Omega_{-j,j}}{\widehat\Omega_{jj}}.}
$$

This is the [Graphical Lasso column regression](../../../../../graphical-lasso-column-regression.md) identity. The minus sign is essential: it converts the precision-entry subgradient into the regression-coefficient subgradient. The argument uses the inverse identity directly, so it does not require proving the supplied block inverse formula.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
