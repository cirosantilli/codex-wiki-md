<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $y\in\mathbb R^n$ for the observed response and $x_j$ for column $j$ of the working [design matrix](../../../../../design-matrix.md) $X$. The usual [LARS](../../../../../least-angle-regression.md) convention gives every [covariate](../../../../../covariate.md) unit [Euclidean norm](../../../../../euclidean-norm.md). If an unpenalized intercept is fitted separately, first centre $y$ and the nonconstant [covariates](../../../../../covariate.md), and restore the intercept afterward. For an intercept-free model no centring is required. The algebra below also applies to an unscaled full-rank design; only the literal equal-angle interpretation uses unit-length columns. The penalty is defined on the [regression coefficients](../../../../../regression-coefficient.md) of whichever working design is used, since rescaling [covariates](../../../../../covariate.md) changes the units of an L1 penalty.

Initialize $\widehat\beta^0=0$, $\widehat\mu^0=X\widehat\beta^0=0$ and residual $r^0=y$. At iteration $k$, let

$$
r^{k-1}=y-\widehat\mu^{k-1},\qquad c_j^k=x_j^Tr^{k-1},\qquad C^k=\max_j|c_j^k|.
$$

These $c_j^k$ are residual inner products, often called residual correlations. If $C^k=0$, all [normal equations](../../../../../normal-equation.md) are satisfied and the path has reached [ordinary least squares](../../../../../ordinary-least-squares.md). Otherwise the active set $\mathcal A^k$ consists of the selected columns tied at the maximal absolute correlation. Initially select the maximizing column, or all such columns in a tie. Ordinary [least angle regression](../../../../../least-angle-regression.md) retains previously selected columns and adds each new one when it ties the active correlations. Put $s_j^k=\operatorname{sign}(c_j^k)$ for active $j$.

To define the direction, form the signed active design $X_{\mathcal A}^s=(s_j^kx_j)_{j\in\mathcal A^k}$ and its [Gram matrix](../../../../../gram-matrix.md) $G_{\mathcal A}=(X_{\mathcal A}^s)^TX_{\mathcal A}^s$. Full column rank makes this matrix [positive-definite](../../../../../positive-definite-bilinear-form.md). Let $1_{\mathcal A}$ denote the vector of ones of length $|\mathcal A^k|$, and set

$$
\alpha^k=(1_{\mathcal A}^TG_{\mathcal A}^{-1}1_{\mathcal A})^{-1/2},\qquad w^k=\alpha^kG_{\mathcal A}^{-1}1_{\mathcal A},\qquad u^k=X_{\mathcal A}^sw^k.
$$

Then $\|u^k\|^2=1$ and $(X_{\mathcal A}^s)^Tu^k=\alpha^k1_{\mathcal A}$. This is the [equiangular direction in least angle regression](../../../../../equiangular-direction-in-least-angle-regression.md). Define $a_j^k=x_j^Tu^k$ for every [covariate](../../../../../covariate.md), and define the [regression coefficient](../../../../../regression-coefficient.md) direction by $d_j^k=s_j^kw_j^k$ on $\mathcal A^k$, zero otherwise. It satisfies $Xd^k=u^k$.

Along the line $\mu(\gamma)=\widehat\mu^{k-1}+\gamma u^k$, residual correlations are $c_j^k-\gamma a_j^k$. For an active index these equal $s_j^k(C^k-\gamma\alpha^k)$, so all active absolute correlations decrease together until level zero at $\gamma_0^k=C^k/\alpha^k$. An inactive [covariate](../../../../../covariate.md) first joins when its correlation equals either sign of the common level. Solving these two equalities gives

$$
\widehat\gamma_{\rm entry}^k=\min_{j\notin\mathcal A^k}^{+}\left\{\frac{C^k-c_j^k}{\alpha^k-a_j^k},\ \frac{C^k+c_j^k}{\alpha^k+a_j^k}\right\}.
$$

Here $\min^+$ means the smallest finite strictly positive candidate; zero denominators do not produce a future entry, and an empty candidate set has minimum $+\infty$. Candidates beyond the zero-correlation endpoint are capped by that endpoint. Take

$$
\boxed{\gamma_{\rm LAR}^k=\min\{\widehat\gamma_{\rm entry}^k,\gamma_0^k\},\quad\widehat\beta^k=\widehat\beta^{k-1}+\gamma_{\rm LAR}^kd^k,\quad\widehat\mu^k=\widehat\mu^{k-1}+\gamma_{\rm LAR}^ku^k.}
$$

At an entry add the newly tied [covariate](../../../../../covariate.md), or all simultaneous ties, and recompute the direction. Once all [covariates](../../../../../covariate.md) are active there is no inactive candidate: the final move is to correlation level zero and the full least-squares fit. These definitions specify every term in the stated step formula and the [entry knot in least angle regression](../../../../../entry-knot-in-least-angle-regression.md).

For definiteness use the following penalty normalization for the [Lasso estimator](../../../../../lasso.md):

$$
\boxed{\widehat\beta_\lambda^{\rm Lasso}=\operatorname*{argmin}_{\beta\in\mathbb R^p}\left\{\frac12\|y-X\beta\|^2+\lambda\sum_{j=1}^p|\beta_j|\right\},\qquad\lambda>0.}
$$

Full column rank makes the criterion [strictly convex](../../../../../strictly-convex-function.md), so the minimizer is unique. With the alternative squared-error normalization $1/(2n)$, the penalty parameter is divided by $n$. The [Karush-Kuhn-Tucker conditions for the Lasso](../../../../../karush-kuhn-tucker-conditions-for-the-lasso.md) in the chosen normalization are

$$
x_j^T(y-X\beta)=\lambda\operatorname{sign}(\beta_j)\quad(\beta_j\ne0),\qquad |x_j^T(y-X\beta)|\leq\lambda\quad(\beta_j=0).
$$

Hence the zero vector is the solution for every $\lambda\geq\lambda_{\max}:=\max_j|x_j^Ty|$. Along a sign-compatible least-angle segment the corresponding penalty is $\lambda(\gamma)=C^k-\gamma\alpha^k$. Active correlation equalities and inactive bounds satisfy the KKT conditions exactly while each nonzero [regression coefficient](../../../../../regression-coefficient.md) retains the sign $s_j^k$. Ordinary LARS can let a [regression coefficient](../../../../../regression-coefficient.md) cross zero while its correlation sign stays unchanged; continuing past that crossing would violate the KKT conditions.

The required modification is therefore to monitor [regression coefficient](../../../../../regression-coefficient.md) zero crossings. Along $\beta(\gamma)=\widehat\beta^{k-1}+\gamma d^k$, define the [Lasso dropout knot](../../../../../lasso-dropout-knot.md)

$$
\widetilde\gamma^k=\min_{j\in\mathcal A^k:\,-\widehat\beta_j^{k-1}/d_j^k>0}\left(-\frac{\widehat\beta_j^{k-1}}{d_j^k}\right),
$$

with $d_j^k=0$ ignored and the empty minimum again $+\infty$. Stop at

$$
\boxed{\gamma_{\rm Lasso}^k=\min\{\widehat\gamma_{\rm entry}^k,\widetilde\gamma^k,\gamma_0^k\}.}
$$

If a nonzero active [regression coefficient](../../../../../regression-coefficient.md) reaches zero before the next entry, remove it from the active direction and recompute; the fitted value is continuous at this event. If entry comes first, add that [covariate](../../../../../covariate.md) as before. A removed [covariate](../../../../../covariate.md) is allowed to re-enter later, so the active set need not increase monotonically. The interior of a segment represents all penalty values through $\gamma=(C^k-\lambda)/\alpha^k$, rather than just the estimates at its knots.

For complete treatment of simultaneous events, full column rank alone does not imply that entries and dropouts occur singly. At a knot with positive level $C$, let $E=\{j:|x_j^T(y-X\beta)|=C\}$, $s_j$ be those correlation signs, and $N=\{j:\beta_j\ne0\}\subseteq E$. The [KKT-consistent resolution of tied Lasso knots](../../../../../kkt-consistent-resolution-of-tied-lasso-knots.md) chooses the next tangent $v$ by

$$
\min_v\left\{\frac12v^TX^TXv-\sum_{j\in E}s_jv_j\right\},\qquad v_{E^c}=0,\quad s_jv_j\geq0\quad(j\in E\setminus N).
$$

This [strictly convex](../../../../../strictly-convex-function.md) [quadratic program](../../../../../quadratic-program.md) has a unique minimizer. For nonzero or newly entering coordinates its stationarity gives $x_j^TXv=s_j$; for tied zero coordinates kept out, $s_jx_j^TXv\geq1$. Thus for a small decrease $h$ of the penalty, $\beta+hv$ has the correct [regression coefficient](../../../../../regression-coefficient.md) signs, active residual scores $s_j(C-h)$, and inactive scores within $[-(C-h),C-h]$. Strictly inactive coordinates remain feasible by continuity. Choose the resulting support for the next segment and normalize $u=Xv/\|Xv\|$; this reduces to the preceding equiangular formulas. It handles ties, including a newly tied zero [regression coefficient](../../../../../regression-coefficient.md) whose unconstrained direction would point against its correlation sign, without perturbing the data.

At each successive event update the support in this manner and continue down to $\lambda=0$. Between knots the [regression coefficients](../../../../../regression-coefficient.md) are linear in $\lambda$ and satisfy the sufficient KKT conditions. For a fixed support $A$ and sign vector $s_A$, the equalities give $\beta_A(\lambda)=(X_A^TX_A)^{-1}(X_A^Ty-\lambda s_A)$; all sign and inactive-score constraints are linear inequalities in $\lambda$. Each support/sign pattern therefore has an interval of validity, and there are only finitely many such patterns, so the complete path has finitely many linear segments. Together with the initial zero solution for $\lambda\geq\lambda_{\max}$, these interpolated segments give

$$
\boxed{\text{the entire unique Lasso regularization path for every }\lambda>0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
