# Lasso

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lasso_(statistics))

The Lasso minimizes regression error plus an $\ell^1$ penalty.

**Table of contents**

- [Karush-Kuhn-Tucker conditions for the Lasso](#karush-kuhn-tucker-conditions-for-the-lasso)
- [Lasso regularization path](#lasso-regularization-path)
  - [KKT-consistent resolution of tied Lasso knots](#kkt-consistent-resolution-of-tied-lasso-knots)
  - [Lasso dropout knot](#lasso-dropout-knot)
- [Gaussian score event for the Lasso](#gaussian-score-event-for-the-lasso)
- [Sparse maximum eigenvalue](#sparse-maximum-eigenvalue)
  - [Lasso support bound from sparse eigenvalues](#lasso-support-bound-from-sparse-eigenvalues)
- [Lava estimator](#lava-estimator)
  - [Lasso reduction for the Lava estimator](#lasso-reduction-for-the-lava-estimator)
- [Fused Lasso](#fused-lasso)
  - [One-dimensional total variation denoising](#one-dimensional-total-variation-denoising)
- [Dantzig selector](#dantzig-selector)
- [Square-root Lasso](#square-root-lasso)
  - [Residual-score decomposition from square-root Lasso](#residual-score-decomposition-from-square-root-lasso)
  - [Tuning relation between Lasso and square-root Lasso](#tuning-relation-between-lasso-and-square-root-lasso)
- [Group Lasso](#group-lasso)
  - [Paired group Lasso for Gaussian graph estimation](#paired-group-lasso-for-gaussian-graph-estimation)
    - [Paired group Lasso optimality conditions](#paired-group-lasso-optimality-conditions)
- [Basic inequality for the Lasso](#basic-inequality-for-the-lasso)
  - [Prediction inequality from Lasso stationarity](#prediction-inequality-from-lasso-stationarity)
  - [Slow-rate prediction bound for the Lasso](#slow-rate-prediction-bound-for-the-lasso)
  - [Lasso cone condition](#lasso-cone-condition)
    - [Restricted eigenvalue condition](#restricted-eigenvalue-condition)
    - [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso)
      - [Fast-rate Lasso prediction bound under compatibility](#fast-rate-lasso-prediction-bound-under-compatibility)
        - [Prediction and coefficient error bound for compatible Lasso](#prediction-and-coefficient-error-bound-for-compatible-lasso)
        - [Lasso sign recovery under compatibility](#lasso-sign-recovery-under-compatibility)
      - [Compatibility constant](#compatibility-constant)
        - [Stability of a compatibility constant under entrywise perturbation](#stability-of-a-compatibility-constant-under-entrywise-perturbation)
      - [Lasso sign recovery from cone invertibility](#lasso-sign-recovery-from-cone-invertibility)
- [Debiased Lasso](#debiased-lasso)
  - [Debiased-Lasso remainder bound](#debiased-lasso-remainder-bound)
  - [Approximate inverse of a Gram matrix](#approximate-inverse-of-a-gram-matrix)
  - [Nodewise Lasso](#nodewise-lasso)
    - [Nodewise-Lasso residual identity](#nodewise-lasso-residual-identity)
  - [Debiased-Lasso asymptotic normality](#debiased-lasso-asymptotic-normality)
    - [Gaussian identity design for debiased Lasso](#gaussian-identity-design-for-debiased-lasso)
- [Soft thresholding](#soft-thresholding)
- [Berhu penalty](#berhu-penalty)
- [Elastic net regularization](#elastic-net-regularization)
  - [Elastic net regularization in Hilbert sequence space](#elastic-net-regularization-in-hilbert-sequence-space)
    - [Nonlinearity of elastic net reconstruction](#nonlinearity-of-elastic-net-reconstruction)
    - [Norm convergence of elastic net regularization](#norm-convergence-of-elastic-net-regularization)
  - [Grouping effect of the elastic net](#grouping-effect-of-the-elastic-net)

## Karush-Kuhn-Tucker conditions for the Lasso

↑ **Parent:** [Lasso](lasso.md)

For the [Lasso](lasso.md) criterion $\|Y-Xb\|_2^2/(2n)+\lambda\|b\|_1$, the displayed [subgradient optimality condition](real-analysis.md#subgradient-optimality-condition) is necessary and sufficient. A nonzero coefficient has residual score $\lambda\operatorname{sign}(b_k)$, and a zero coefficient has residual score in $[-\lambda,\lambda]$. The [subdifferential of the L1 norm](convex-optimization.md#subdifferential-of-the-l1-norm) supplies both cases.

## Lasso regularization path

↑ **Parent:** [Lasso](lasso.md)

The [Lasso](lasso.md) regularization path follows its coefficients as the penalty or constraint radius changes. Under the usual least-angle construction, the coefficient path is piecewise linear between knots, and variables can enter or leave the active set. Reading support at a selected [cross-validation](statistical-learning.md#cross-validation) fraction requires checking which coefficients are actually zero at that fraction, rather than retaining only visibly large traces.

### KKT-consistent resolution of tied Lasso knots

↑ **Parent:** [Lasso regularization path](#lasso-regularization-path)

At a positive penalty level, let $E$ be the residual-score equality set, $s_j$ its signs and $N$ the nonzero [regression coefficient](linear-regression.md#regression-coefficient) support. With full column rank, the displayed [strictly convex](real-analysis.md#strictly-convex-function) [quadratic program](mathematical-optimization.md#quadratic-program) selects the direction for a small decrease of the penalty. Existing nonzero [regression coefficients](linear-regression.md#regression-coefficient) have unrestricted tangent components; tied zero [regression coefficients](linear-regression.md#regression-coefficient) may move only with their residual signs. Stationarity gives $X_j^TXv=s_j$ for $j\in N$ and for entering zero coordinates, and $s_jX_j^TXv\geq1$ for tied coordinates that remain zero. These are exactly the first-order [Karush-Kuhn-Tucker conditions for the Lasso](#karush-kuhn-tucker-conditions-for-the-lasso) along the next segment. Normalize $Xv$ to obtain the corresponding least-angle direction. This resolves simultaneous entries or dropouts without adding a generic-position assumption.

// Target: mathematical-optimization.bigb

### Lasso dropout knot

↑ **Parent:** [Lasso regularization path](#lasso-regularization-path)

On a least-angle segment $\beta(\gamma)=\beta+\gamma d$, a nonzero active [regression coefficient](linear-regression.md#regression-coefficient) reaches zero at the displayed first positive root. Continue only as far as the first dropout, inactive-entry event or zero-correlation endpoint. At a dropout remove the vanishing [regression coefficient](linear-regression.md#regression-coefficient) from the active direction and recompute. This preserves agreement between nonzero [regression coefficient](linear-regression.md#regression-coefficient) signs and residual-score signs, which the [Karush-Kuhn-Tucker conditions for the Lasso](#karush-kuhn-tucker-conditions-for-the-lasso) require. A removed [regression coefficient](linear-regression.md#regression-coefficient) may re-enter later; the active set need not grow monotonically.

## Gaussian score event for the Lasso

↑ **Parent:** [Lasso](lasso.md)

Let $0<c<1$, $A>0$, $\sigma>0$ and $p\geq2$. For [design matrix](linear-regression.md#design-matrix) columns of norm $\sqrt n$ and $\varepsilon\sim N_n(0,\sigma^2I)$, the event $\|X^T\varepsilon\|_\infty/n\leq c\lambda$ has probability at least $1-p^{1-A^2c^2/2}$ when $\lambda=A\sigma\sqrt{\log(p)/n}$. Apply the [sharp two-sided Gaussian tail bound](probability-and-statistics.md#sharp-two-sided-gaussian-tail-bound) to each standardized score and then the [union bound](probability-inequality.md#boole-s-inequality); independence of the scores is not required.

## Sparse maximum eigenvalue

↑ **Parent:** [Lasso](lasso.md)

For a [design matrix](linear-regression.md#design-matrix) $X$ with $p$ columns, define $\kappa_m^2=\max_{|M|=m}\lambda_{\max}(X_M^TX_M/n)$ for $1\le m\le p$. Equivalently this bounds $\|Xv\|_2^2/(n\|v\|_2^2)$ for [vectors](vector-space.md#vector) supported on at most $m$ coordinates. These quantities are nondecreasing: extend the support of a maximizing [vector](vector-space.md#vector) by zero coordinates and use the variational characterization of the largest [eigenvalue](linear-operator-theory.md#eigenvalue). Values at $m>p$, including infinity, require a separate convention.

### Lasso support bound from sparse eigenvalues

↑ **Parent:** [Sparse maximum eigenvalue](#sparse-maximum-eigenvalue)

For $\lambda>0$ and $\phi>0$, use the [Lasso](lasso.md) objective $\|Y-X\beta\|_2^2/(2n)+\lambda\|\beta\|_1$. Suppose the noise score has maximum [norm](normed-vector-space.md#norm) at most $\lambda/2$, the true support has size $s$, and $\|X(\widehat\beta-\beta^0)\|_2^2/n\le16\lambda^2s/\phi^2$. For any nonempty $B\subseteq\widehat S$, the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) imply

$$
\lambda|B|/2\le n^{-1}\operatorname{sgn}(\widehat\beta_B)^TX_B^TX(\beta^0-\widehat\beta)\le4\lambda\kappa_{|B|}\sqrt{|B|s}/\phi.
$$

The upper bound is the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Hence $|B|\le64\kappa_{|B|}^2s/\phi^2$. A finite first index $m_*$ violating this inequality must exceed $|\widehat S|$. Its minimality also gives $|\widehat S|\le64\kappa_{m_*}^2s/\phi^2$. If no such index exists within $1,\ldots,p$, use the always defined bound $|\widehat S|\le64\kappa_p^2s/\phi^2$.

## Lava estimator

↑ **Parent:** [Lasso](lasso.md)

The Lava estimator minimizes $\|Y-X(\delta+\beta)\|_2^2/(2n)+\lambda_1\|\delta\|_1+\lambda_2\|\beta\|_2^2$. It combines a component selected by [Lasso](lasso.md) with a component shrunk by [ridge regression](linear-regression.md#ridge-regression). Profiling the latter yields a transformed [Lasso](lasso.md) problem; this is not the same coefficient penalty as [elastic net regularization](#elastic-net-regularization).

### Lasso reduction for the Lava estimator

↑ **Parent:** [Lava estimator](#lava-estimator)

For $Q=(X^TX+2n\lambda_2I)^{-1}$ and $A=(I-XQX^T)^{1/2}$, profiling the dense coefficient gives $\widehat\beta=QX^T(Y-X\widehat\delta)$. The sparse coefficient minimizes $\|AY-AX\delta\|_2^2/(2n)+\lambda_1\|\delta\|_1$. The transformation uses the [principal square root of a positive semidefinite matrix](quadratic-form.md#principal-square-root-of-a-positive-semidefinite-matrix) and remains valid for rank-deficient designs.

## Fused Lasso

↑ **Parent:** [Lasso](lasso.md)

The fused Lasso adds an [L1 norm](normed-vector-space.md#l1-norm) penalty on adjacent coefficient differences to a squared-error objective, optionally together with an [L1 norm](normed-vector-space.md#l1-norm) penalty on the coefficients themselves. The differences penalty encourages neighbouring coefficients to coincide.

### One-dimensional total variation denoising

↑ **Parent:** [Fused Lasso](#fused-lasso)

This version of the [fused Lasso](#fused-lasso) penalizes only adjacent differences. It estimates a piecewise-constant signal while preserving an unpenalized constant level. Larger penalties generally favour fewer fitted changes.

## Dantzig selector

↑ **Parent:** [Lasso](lasso.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dantzig_selector)

The Dantzig selector minimizes the coefficient $\ell^1$ norm subject to an $\ell^\infty$ bound on residual correlations.

## Square-root Lasso

↑ **Parent:** [Lasso](lasso.md)

The square-root Lasso uses the unsquared residual norm plus an $\ell^1$ penalty.

### Residual-score decomposition from square-root Lasso

↑ **Parent:** [Square-root Lasso](#square-root-lasso)

For a fixed residual direction $R=Z-X\widetilde\beta_\gamma\ne0$ obtained by [Square-root Lasso](#square-root-lasso), its optimality condition gives $\|X^TR\|_\infty\leq\sqrt n\,\gamma\|R\|_2$. In a fixed-design [normal linear model](normal-linear-model.md), the score $R^T(Y-X\widehat\beta)/\|R\|_2$ equals a $N(0,\sigma^2)$ component plus a remainder bounded by $\sqrt n\,\gamma\|\beta^0-\widehat\beta\|_1$. The direction must be fixed or independent of the response noise for that normality claim.

### Tuning relation between Lasso and square-root Lasso

↑ **Parent:** [Square-root Lasso](#square-root-lasso)

A [Lasso](lasso.md) minimizer with positive residual scale $\widehat\sigma_\lambda=\|Y-X\widehat\beta_\lambda\|_2/\sqrt n$ also minimizes the [Square-root Lasso](#square-root-lasso) objective at the displayed tuning parameter. Divide its [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) by the residual scale and use the [subgradient optimality condition](real-analysis.md#subgradient-optimality-condition).

## Group Lasso

↑ **Parent:** [Lasso](lasso.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_Lasso)

The group Lasso partitions a coefficient vector into groups $G_1,\ldots,G_q$ and replaces the coordinatewise $\ell^1$ penalty with a weighted sum of group norms,

$$
P(\beta)=\sum_{j=1}^q m_j\lVert\beta_{G_j}\rVert_2.
$$

It tends to retain or discard an entire group at once. Its dual norm is

$$
P^*(v)=\max_j m_j^{-1}\lVert v_{G_j}\rVert_2,
$$

so the corresponding [Holder inequality](functional-analysis.md#holder-inequality) is $|u^Tv|\leq P(u)P^*(v)$.

### Paired group Lasso for Gaussian graph estimation

↑ **Parent:** [Group Lasso](#group-lasso)

Joint squared-error [nodewise regression](random-variable.md#nodewise-regression) with this penalty groups the two coefficients of each unordered edge. Its norm is nonsmooth only when the whole pair is zero, encouraging edge-wise sparsity. A fitted edge is present when its pair norm is positive. The penalty does not require equal directional coefficients, two nonzero entries in every selected group, or a symmetric positive definite [precision matrix](variance.md#precision-matrix).

#### Paired group Lasso optimality conditions

↑ **Parent:** [Paired group Lasso for Gaussian graph estimation](#paired-group-lasso-for-gaussian-graph-estimation)

For each unordered pair, $g=(\Theta_{jk},\Theta_{kj})$ and $c=(X_j^{\mathsf T}r_k/n,X_k^{\mathsf T}r_j/n)$ with centred columns and [regression residuals](probability-and-statistics.md#regression-residual). The [subdifferential](convex-optimization.md#subdifferential) of the [Euclidean norm](normed-vector-space.md#euclidean-norm) is the unit ball at zero and $g/\|g\|_2$ otherwise. These [KKT conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) are necessary and sufficient for the convex paired objective and explain joint edge deletion.

## Basic inequality for the Lasso

↑ **Parent:** [Lasso](lasso.md)

Comparing the [Lasso](lasso.md) objective at an estimate $\widehat\beta$ and a target $\beta^0$, then expanding the squared loss, bounds the prediction error by a noise-score term and the decrease in the $\ell^1$ penalty.

### Prediction inequality from Lasso stationarity

↑ **Parent:** [Basic inequality for the Lasso](#basic-inequality-for-the-lasso)

For [Lasso](lasso.md) loss $\|Y-X\beta\|_2^2/(2n)+\lambda\|\beta\|_1$ and $Y=X\beta^0+\eta$, stationarity with a penalty [subgradient](real-analysis.md#subgradient) gives $\|X\delta\|_2^2/n\leq\eta^TX\delta/n+\lambda(\|\beta^0\|_1-\|\widehat\beta\|_1)$, $\delta=\widehat\beta-\beta^0$. This follows by multiplying the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) by $\delta$ and using $z^T\widehat\beta=\|\widehat\beta\|_1$ and $z^T\beta^0\leq\|\beta^0\|_1$.

### Slow-rate prediction bound for the Lasso

↑ **Parent:** [Basic inequality for the Lasso](#basic-inequality-for-the-lasso)

For $Y=X\beta^0+\eta$, the [Lasso](lasso.md) objective $\|Y-X\beta\|_2^2/(2n)+\lambda\|\beta\|_1$ has this prediction bound whenever $\|X^T\eta\|_\infty/n\leq\lambda$. Compare its value at $\widehat\beta$ and $\beta^0$, apply [Holder inequality](functional-analysis.md#holder-inequality) to the score, and use the triangle inequality. No [restricted eigenvalue condition](#restricted-eigenvalue-condition) is required.

### Lasso cone condition

↑ **Parent:** [Basic inequality for the Lasso](#basic-inequality-for-the-lasso)

On an event where the noise-score infinity norm is at most half the penalty, the Lasso error $\delta$ obeys $\lVert\delta_{S^c}\rVert_1\leq3\lVert\delta_S\rVert_1$.

#### Restricted eigenvalue condition

↑ **Parent:** [Lasso cone condition](#lasso-cone-condition)

A design matrix satisfies a restricted eigenvalue condition with constant $\gamma>0$ on a cone $C$ when $\lVert X\delta\rVert_2^2/n\geq\gamma\lVert\delta\rVert_2^2$ for every nonzero $\delta\in C$.

#### Compatibility condition for the Lasso

↑ **Parent:** [Lasso cone condition](#lasso-cone-condition)

A compatibility condition lower-bounds prediction norm by a scaled $\ell^1$ norm on a [Lasso cone condition](#lasso-cone-condition). One convention requires $|S|\lVert X\delta\rVert_2^2/n\geq\phi^2\lVert\delta_S\rVert_1^2$ throughout the cone.

##### Fast-rate Lasso prediction bound under compatibility

↑ **Parent:** [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso)

Let $\delta=\widehat\beta-\beta^0$, $s=|S|>0$ and $\phi>0$. On the score event $\|X^T\eta\|_\infty/n\leq c\lambda$ with $0<c<1$, the [prediction inequality from Lasso stationarity](#prediction-inequality-from-lasso-stationarity) gives $Q+(1-c)\lambda\|\delta_{S^c}\|_1\leq(1+c)\lambda\|\delta_S\|_1$. If the [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso) with constant $\phi$ holds on this cone, then $Q+(1-c)\lambda\|\delta_{S^c}\|_1\leq(1+c)^2\lambda^2s/\phi^2$. Here $Q=\|X\delta\|_2^2/n$ and $S$ is the true [support of a vector](numerical-analysis.md#support-of-a-vector).

###### Prediction and coefficient error bound for compatible Lasso

↑ **Parent:** [Fast-rate Lasso prediction bound under compatibility](#fast-rate-lasso-prediction-bound-under-compatibility)

With objective $\|Y-Xb\|_2^2/(2n)+\lambda\|b\|_1$, the [Gaussian score event for the Lasso](#gaussian-score-event-for-the-lasso) $\|X^T\epsilon/n\|_\infty\leq\lambda/2$ gives $Q+\lambda\|\delta_{S^c}\|_1\leq3\lambda\|\delta_S\|_1$, where $Q=\|X\delta\|_2^2/n$. The [Lasso cone condition](#lasso-cone-condition) activates the [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso). Then $Q+\lambda\|\delta\|_1\leq4\lambda\sqrt{sQ}/\phi_0\leq Q/2+8\lambda^2s/\phi_0^2$. Thus even $Q+2\lambda\|\delta\|_1\leq16\lambda^2s/\phi_0^2$. This controls prediction and coefficient error together, including a design with correlated columns.

###### Lasso sign recovery under compatibility

↑ **Parent:** [Fast-rate Lasso prediction bound under compatibility](#fast-rate-lasso-prediction-bound-under-compatibility)

The [fast-rate Lasso prediction bound under compatibility](#fast-rate-lasso-prediction-bound-under-compatibility) implies $\|\widehat\beta_S-\beta^0_S\|_1\leq(1+c)\lambda s/\phi^2$. Each true coefficient larger in absolute value than this bound has the correct estimated sign. This conclusion alone does not ensure absence of false positives.

##### Compatibility constant

↑ **Parent:** [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso)

For a positive-semidefinite matrix $\Sigma$, an active set $S$ of size $s$, and cone factor three, one compatibility constant is defined by

$$
\phi_\Sigma^2
=s\inf_{\|\delta_S\|_1=1,\,\|\delta_{S^c}\|_1\leq3}
\delta^T\Sigma\delta.
$$

It measures how strongly the quadratic form controls active-coordinate $\ell^1$ error on the [Lasso cone condition](#lasso-cone-condition).

###### Stability of a compatibility constant under entrywise perturbation

↑ **Parent:** [Compatibility constant](#compatibility-constant)

If $\|\Theta-\Sigma\|_{\max}\leq\phi_\Sigma^2/(32s)$, then $\phi_\Theta^2\geq\phi_\Sigma^2/2$. Indeed, every normalized cone vector has $\|\delta\|_1\leq4$, so its quadratic form changes by at most $16\|\Theta-\Sigma\|_{\max}\leq\phi_\Sigma^2/(2s)$.

##### Lasso sign recovery from cone invertibility

↑ **Parent:** [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso)

Suppose every $\delta$ in the [Lasso cone condition](#lasso-cone-condition) satisfies $\psi\|\delta_S\|_\infty\leq\|\widehat\Sigma\delta\|_\infty$. On the usual score event, the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) give $\|\widehat\Sigma(\widehat\beta-\beta^0)\|_\infty\leq3\lambda/2$. Hence every active-coordinate error is at most $3\lambda/(2\psi)$, and a larger minimum nonzero signal guarantees coordinatewise sign recovery.

## Debiased Lasso

↑ **Parent:** [Lasso](lasso.md)

The debiased Lasso adds an approximate inverse-Gram correction to a Lasso estimate so that each corrected coordinate has an asymptotically linear expansion.

### Debiased-Lasso remainder bound

↑ **Parent:** [Debiased Lasso](#debiased-lasso)

Let $\widehat\Sigma=X^TX/n$ and use [Nodewise Lasso](#nodewise-lasso) with $\lambda_j>0$ and nonzero design columns. Form $c_j$ with entry $j$ equal to one and other entries $-\widehat\gamma^{(j)}$, and put row $j$ of $\widehat\Theta$ equal to $c_j^T/\widehat\tau_j^2$. The [nodewise-Lasso residual identity](#nodewise-lasso-residual-identity) and the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) show that the diagonal of $\widehat\Theta\widehat\Sigma$ equals one and its row-$j$ off-diagonal entries have magnitude at most $\lambda_j/\widehat\tau_j^2$. For the [Debiased Lasso](#debiased-lasso),

$$
\sqrt n(\widehat b-\beta^0)=\widehat\Theta X^T\varepsilon/\sqrt n+\Delta,\qquad \Delta=\sqrt n(\widehat\Theta\widehat\Sigma-I)(\beta^0-\widehat\beta).
$$

The displayed bound follows row by row from [Holder inequality](functional-analysis.md#holder-inequality). If the noise is conditionally [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) with [covariance](variance.md#covariance) $\sigma^2I$, and the nodewise fits and tuning parameters depend only on $X$, the first term is conditionally normal with [covariance](variance.md#covariance) $\sigma^2\widehat\Theta\widehat\Sigma\widehat\Theta^T$.

### Approximate inverse of a Gram matrix

↑ **Parent:** [Debiased Lasso](#debiased-lasso)

A matrix $\Theta$ is an $\eta$-approximate inverse of a Gram matrix $\widehat\Sigma$ in entrywise maximum norm when

$$
\lVert\widehat\Sigma\Theta-I\rVert_{\max}\leq\eta.
$$

This turns the bias remainder of a [Debiased Lasso](#debiased-lasso) into a product of $\eta$ and the coefficient $\ell^1$ error.

### Nodewise Lasso

↑ **Parent:** [Debiased Lasso](#debiased-lasso)

The nodewise Lasso regresses each design column on the remaining columns and uses its residual to estimate a column of the inverse covariance or inverse Gram matrix.

#### Nodewise-Lasso residual identity

↑ **Parent:** [Nodewise Lasso](#nodewise-lasso)

For [Nodewise Lasso](#nodewise-lasso) with objective $\|X_j-X_{-j}\gamma\|_2^2/(2n)+\lambda_j\|\gamma\|_1$, put $r_j=X_j-X_{-j}\widehat\gamma^{(j)}$. Its [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) give $X_{-j}^Tr_j/n=\lambda_jz_j$ with $z_j\in\partial\|\widehat\gamma^{(j)}\|_1$. Hence

$$
X_j^Tr_j/n=\|r_j\|_2^2/n+\lambda_j\|\widehat\gamma^{(j)}\|_1=\widehat\tau_j^2.
$$

For $\lambda_j>0$ this is positive whenever $X_j\ne0$; if it were zero both nonnegative terms would vanish, forcing $\widehat\gamma^{(j)}=0$ and $X_j=r_j=0$. Nonzero columns are therefore an essential hypothesis for division by this quantity.

### Debiased-Lasso asymptotic normality

↑ **Parent:** [Debiased Lasso](#debiased-lasso)

Under sparsity, compatibility, and inverse-Gram estimation conditions, the standardized coordinatewise error of the [Debiased Lasso](#debiased-lasso) converges in distribution to a [standard normal distribution](probability-distribution.md#standard-normal-distribution).

#### Gaussian identity design for debiased Lasso

↑ **Parent:** [Debiased-Lasso asymptotic normality](#debiased-lasso-asymptotic-normality)

In the [normal linear model](normal-linear-model.md), assume $\varepsilon\sim N_n(0,\sigma^2I)$ is independent of $X$. Independent rows of $X$ with [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) $N_p(0,I_p)$ give a simple random design for [Debiased Lasso](#debiased-lasso). Let $p\to\infty$, $\log p=o(n)$ and $s\log p=o(\sqrt n)$, with fixed positive noise scale. Choose the [Lasso](lasso.md) penalty and all [Nodewise Lasso](#nodewise-lasso) penalties as sufficiently large constant multiples of $\sqrt{\log p/n}$, including the noise scale in the former. Uniform sample cross-correlations are bounded by this scale, so zero is the nodewise solution with [probability](probability-theory.md#probability) tending to one. Column squared [norms](normed-vector-space.md#norm) divided by $n$ converge uniformly to one. To check the [Compatibility condition for the Lasso](#compatibility-condition-for-the-lasso) directly, put $\widehat\Sigma=X^TX/n$ and $\eta=\max_{j,k}|\widehat\Sigma_{jk}-\mathbf1_{\{j=k\}}|$. On the [Lasso cone condition](#lasso-cone-condition), $\|\delta\|_1\le4\|\delta_S\|_1$, and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\delta^T\widehat\Sigma\delta\ge\|\delta\|_2^2-\eta\|\delta\|_1^2\ge(1/s-16\eta)\|\delta_S\|_1^2.
$$

For $s\ge1$, [entrywise concentration of a Gaussian Gram matrix](probability-inequality.md#entrywise-concentration-of-a-gaussian-gram-matrix) gives $\eta\le D_0\sqrt{\log p/n}$ with [probability](probability-theory.md#probability) tending to one for sufficiently large fixed $D_0$. The stated sparsity condition implies $s\eta\to0$ on this event, so one can take $\phi^2\ge1/2$ eventually. The conditional [Gaussian tail bound](probability-and-statistics.md#gaussian-tail-bound) for the noise score and the [Basic inequality for the Lasso](#basic-inequality-for-the-lasso) then give $\|\widehat\beta-\beta^0\|_1\le C s\sqrt{\log p/n}$ with [probability](probability-theory.md#probability) tending to one. Consequently the [debiased-Lasso remainder bound](#debiased-lasso-remainder-bound) is at most $A s\log p/\sqrt n$ with [probability](probability-theory.md#probability) tending to one, for a fixed constant $A$. These assumptions allow both $p$ and $s$ to grow, for example $p=n^2$, $s=\lfloor n^{1/4}\rfloor$.

## Soft thresholding

↑ **Parent:** [Lasso](lasso.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Soft_thresholding)

Soft thresholding maps $u$ to $\operatorname{sgn}(u)(|u|-\lambda)_+$ and is the proximal operator of the absolute-value penalty.

## Berhu penalty

↑ **Parent:** [Lasso](lasso.md)

The Berhu, or reverse-Huber, penalty with threshold $\delta>0$ is

$$
\rho_\delta(t)=
\begin{cases}
|t|,&|t|\leq\delta,\\
(t^2+\delta^2)/(2\delta),&|t|>\delta.
\end{cases}
$$

It behaves like the [absolute value](real-analysis.md#absolute-value) near zero and quadratically for large coefficients.

## Elastic net regularization

↑ **Parent:** [Lasso](lasso.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elastic_net_regularization)

Elastic-net regression minimizes squared error plus both an $\ell^1$ coefficient penalty and a squared $\ell^2$ penalty. It combines exact sparsity with strict convexity when the quadratic penalty is positive.

### Elastic net regularization in Hilbert sequence space

↑ **Parent:** [Elastic net regularization](#elastic-net-regularization)

Extend $J$ by infinity outside $\ell^1$. For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $K:\ell^2\to\ell^2$, the objective $\|Ku-f\|_2^2/2+\alpha J(u)$ is coercive, weakly lower semicontinuous and [strictly convex](real-analysis.md#strictly-convex-function) for $\alpha>0$, so it has a unique minimizer. The quadratic penalty ensures existence and uniqueness even if $K$ has a [null space](kernel-of-a-linear-map.md). Its limiting exact solution minimizes $J$ in the data fiber, which need not be the [minimum-norm least-squares solution](inverse-problem.md#minimum-norm-least-squares-solution).

#### Nonlinearity of elastic net reconstruction

↑ **Parent:** [Elastic net regularization in Hilbert sequence space](#elastic-net-regularization-in-hilbert-sequence-space)

For fixed $\alpha>0$ and nonzero bounded $K$, the reconstruction vanishes when $\|K^*f\|_\infty\leq\alpha$, which includes a neighborhood of zero. If it were linear it would vanish everywhere. Choose a coordinate $e_j$ with $Ke_j\ne0$ and data $f=tKe_j$ with $t\|Ke_j\|^2>\alpha$; the optimality inequality at zero fails, so its minimizer is nonzero. Thus the map is nonlinear. The qualification $K\ne0$ is essential: $K=0$ gives the zero linear map.

#### Norm convergence of elastic net regularization

↑ **Parent:** [Elastic net regularization in Hilbert sequence space](#elastic-net-regularization-in-hilbert-sequence-space)

Assume an exact solution of finite penalty exists and select the unique $J$-minimizing exact solution $u^\dagger$. Minimality gives $\|Ku_\alpha^\delta-f^\delta\|^2/2+\alpha J(u_\alpha^\delta)\leq\delta^2/2+\alpha J(u^\dagger)$. If $\alpha\to0$ and $\delta^2/\alpha\to0$, boundedness, [weak sequential compactness of bounded sequences in a reflexive Banach space](functional-analysis.md#weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space) and lower semicontinuity identify every weak limit with $u^\dagger$. The separate lower semicontinuity of $\|u\|_1$ and $\|u\|_2^2$, together with the upper bound on $J$, forces the Hilbert norms to converge. The [Radon-Riesz theorem](hilbert-space.md#radon-riesz-theorem) then gives [norm convergence](normed-vector-space.md#norm-convergence).

### Grouping effect of the elastic net

↑ **Parent:** [Elastic net regularization](#elastic-net-regularization)

The quadratic penalty encourages strongly correlated predictors to receive similar coefficients, so an elastic net tends to retain or discard correlated predictors as a group more readily than the Lasso.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (39)

- [Basic inequality for the Lasso](#basic-inequality-for-the-lasso)
- [Gaussian identity design for debiased Lasso](#gaussian-identity-design-for-debiased-lasso)
- [Graphical Lasso column regression](variance.md#graphical-lasso-column-regression)
- [Karush-Kuhn-Tucker conditions for the Lasso](#karush-kuhn-tucker-conditions-for-the-lasso)
- [LAR active correlation invariant](linear-regression.md#lar-active-correlation-invariant)
- [Lasso regularization path](#lasso-regularization-path)
- [Lasso support bound from sparse eigenvalues](#lasso-support-bound-from-sparse-eigenvalues)
- [Lava estimator](#lava-estimator)
- [Least angle regression](linear-regression.md#least-angle-regression)
- [Neighbourhood selection](random-variable.md#neighbourhood-selection)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-218.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-205.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-218.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-205.md#1/solution)
- [Penalized least-squares estimator](statistical-learning.md#penalized-least-squares-estimator)
- [Prediction inequality from Lasso stationarity](#prediction-inequality-from-lasso-stationarity)
- [Sign compatibility of LAR and Lasso](linear-regression.md#sign-compatibility-of-lar-and-lasso)
- [Slow-rate prediction bound for the Lasso](#slow-rate-prediction-bound-for-the-lasso)
- [Subdifferential of the L1 norm](convex-optimization.md#subdifferential-of-the-l1-norm)
- [Tuning relation between Lasso and square-root Lasso](#tuning-relation-between-lasso-and-square-root-lasso)
- [Variable selection](statistical-modelling.md#variable-selection)
