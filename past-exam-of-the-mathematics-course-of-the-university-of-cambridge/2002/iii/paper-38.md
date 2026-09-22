# Paper 38

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper38.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper38.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)

## 1

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [P-star approximation](../../../probability-theory.md#p-star-approximation) describes the sampling [density](../../../fluid-mechanics.md#density) of a regular [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) in sample coordinates consisting of the fitted parameter $\widehat\theta$ and a suitable [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) $a$. For a $d$-dimensional parameter, write $\ell(\theta;\widehat\theta,a)$ for the [log-likelihood](../../../statistical-modelling.md#log-likelihood) expressed in these coordinates, and $j(\widehat\theta;\widehat\theta,a)$ for the fitted [observed information](../../../statistical-modelling.md#observed-fisher-information). The approximation is

$$
p^*(\widehat\theta\mid a;\theta)=c(\theta,a)|j(\widehat\theta;\widehat\theta,a)|^{1/2}\exp\{\ell(\theta;\widehat\theta,a)-\ell(\widehat\theta;\widehat\theta,a)\}.
$$

The [determinant](../../../linear-algebra.md#determinant) factor supplies the local volume scale, while the exponential retains the full [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio), rather than replacing it by a quadratic. The [normalizing constant](../../../continuous-probability-distribution.md#normalizing-constant) is chosen by integrating over the fitted-parameter coordinates; its leading regular large-sample value is $(2\pi)^{-d/2}$. These ingredients arise from a [statistical saddlepoint approximation](../../../probability-theory.md#saddlepoint-density-approximation). Their use requires an interior, locally unique fit, nonsingular information and suitable smoothness; an [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) specifies the conditioning surface when the fit alone does not exhaust the relevant sample coordinates. In a regular model the unnormalized leading expression has relative error of order $n^{-1}$ locally; normalization and conditioning matter for refined inference. It is not a universal exact [density](../../../fluid-mechanics.md#density). Under a smooth one-to-one parameter transformation, the [Hessian](../../../calculus.md#hessian-matrix) at the fit transforms without a score term, so its [determinant](../../../linear-algebra.md#determinant) supplies precisely the [density](../../../fluid-mechanics.md#density) [Jacobian determinant](../../../calculus.md#jacobian-determinant). This proves the invariance of the construction under one-to-one changes of [statistical parameters](../../../statistical-model.md#statistical-parameter).

Here put $S=\sum_iX_i$ and $T=\sum_iY_i$. The [log-likelihood](../../../statistical-modelling.md#log-likelihood), apart from a data-only constant, is

$$
\ell(\psi,\lambda)=n\log\psi+2n\log\lambda-\lambda S-\psi\lambda T.
$$

The two [score equations](../../../statistical-modelling.md#score-equation) give

$$
\boxed{\widehat\lambda=\frac nS,\qquad\widehat\psi=\frac ST.}
$$

The sample sums form a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic), and there is no need to retain an additional ancillary in calculating their joint [density](../../../fluid-mechanics.md#density). Inverting the fitted coordinates gives $S=n/\widehat\lambda$ and $T=n/(\widehat\psi\widehat\lambda)$. With parameter order $(\psi,\lambda)$, the fitted [observed information](../../../statistical-modelling.md#observed-fisher-information) is

$$
j(\widehat\psi,\widehat\lambda)=\begin{pmatrix}n/\widehat\psi^2&n/(\widehat\psi\widehat\lambda)\\n/(\widehat\psi\widehat\lambda)&2n/\widehat\lambda^2\end{pmatrix},\qquad |j|^{1/2}=\frac n{\widehat\psi\widehat\lambda}.
$$

Also,

$$
\ell(\psi,\lambda)-\ell(\widehat\psi,\widehat\lambda)=n\log\frac\psi{\widehat\psi}+2n\log\frac\lambda{\widehat\lambda}-\frac{n\lambda}{\widehat\lambda}\left(1+\frac\psi{\widehat\psi}\right)+2n.
$$

Thus the required joint [P-star approximation](../../../probability-theory.md#p-star-approximation) is

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

The [beta function](../../../complex-analysis.md#beta-function) identity $\int_0^\infty z^{n-1}(1+z)^{-2n}\,dz=\Gamma(n)^2/\Gamma(2n)$ therefore gives

$$
\boxed{c_n=\frac{n^{2n-1}e^{-2n}}{\Gamma(n)^2},\qquad p^*(\widehat\psi)=\frac{\Gamma(2n)}{\Gamma(n)^2\psi}\left(\frac{\widehat\psi}\psi\right)^{n-1}\left(1+\frac{\widehat\psi}\psi\right)^{-2n}.}
$$

Both normalized approximations are actually exact. To check the joint assertion independently, $S$ and $T$ have independent [gamma distributions](../../../continuous-probability-distribution.md#gamma-distribution) with shape $n$ and rates $\lambda$ and $\psi\lambda$. Their joint [density](../../../fluid-mechanics.md#density) is $\psi^n\lambda^{2n}S^{n-1}T^{n-1}e^{-\lambda S-\psi\lambda T}/\Gamma(n)^2$. The inverse-coordinate [Jacobian determinant](../../../calculus.md#jacobian-determinant) is

$$
\left|\frac{\partial(S,T)}{\partial(\widehat\psi,\widehat\lambda)}\right|=\frac{n^2}{\widehat\psi^2\widehat\lambda^3},
$$

which reproduces the normalized joint expression. This is the [P-star density for two exponential rates](../../../probability-theory.md#p-star-density-for-two-exponential-rates); its marginal gives the stated [F-distribution](../../../continuous-probability-distribution.md#f-distribution). [Stirling's approximation](../../../real-analysis.md#stirling-formula) gives $c_n=(2\pi)^{-1}(1-1/(6n)+O(n^{-2}))$, so using only the leading normalizer retains the exact shape but not its exact total mass.

The original PDF's displayed [density](../../../fluid-mechanics.md#density) constant is missing a square on $\Gamma(n)$. Its printed expression integrates to $\Gamma(n)$, rather than one in general. The normalized [density](../../../fluid-mechanics.md#density) above is the one consistent with the stated [F-distribution](../../../continuous-probability-distribution.md#f-distribution).

## 2

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For an interest parameter $\psi$ and [nuisance parameter](../../../statistical-model.md#nuisance-parameter) $\lambda$, the [profile likelihood](../../../statistical-modelling.md#profile-likelihood) is $L_p(\psi)=L(\psi,\widetilde\lambda_\psi)$, where $\widetilde\lambda_\psi$ maximizes the [likelihood](../../../statistical-modelling.md#likelihood-function) at fixed $\psi$. Its maximum occurs at the joint [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) of $\psi$. It preserves the optimized [likelihood ratios](../../../statistical-modelling.md#likelihood-ratio) for different interest values and is unchanged by one-to-one reparametrization of the nuisance at each fixed $\psi$. It generally is neither a marginal sampling [density](../../../fluid-mechanics.md#density) nor a conditional [likelihood](../../../statistical-modelling.md#likelihood-function), and eliminating [nuisance parameters](../../../statistical-model.md#nuisance-parameter) by maximization can introduce appreciable small-sample distortion. Differentiating the constrained [score equation](../../../statistical-modelling.md#score-equation) gives the curvature formula

$$
-\ell_p''=j_{\psi\psi}-j_{\psi\lambda}j_{\lambda\lambda}^{-1}j_{\lambda\psi}
$$

at a joint stationary point. The corresponding expected-information expression is the [efficient information](../../../statistical-inference.md#efficient-information) for the interest parameter. Under the regular conditions of [Wilks theorem](../../../statistical-inference.md#wilks-theorem), twice the [profile log-likelihood](../../../statistical-modelling.md#profile-log-likelihood) drop has an asymptotic [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with the dimension of the interest parameter as its [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom).

For scalar nuisance, the [Barndorff-Nielsen modified profile likelihood](../../../statistical-modelling.md#modified-profile-likelihood) may be written

$$
\ell_m(\psi)=\ell_p(\psi)-\frac12\log j_{\lambda\lambda}(\psi,\widetilde\lambda_\psi)-\log\left|\frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}\right|,
$$

where the sample-coordinate [derivative](../../../calculus.md#derivative) holds $\widehat\psi$ and the [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) fixed. For vector nuisance the last two quantities are [determinants](../../../linear-algebra.md#determinant). An equivalent form is $\ell_m=\ell_p+\tfrac12\log|j_{\lambda\lambda}|-\log|\ell_{\lambda;\widehat\lambda}|$, since differentiating the constrained nuisance score gives $\ell_{\lambda;\widehat\lambda}=j_{\lambda\lambda}\partial\widetilde\lambda_\psi/\partial\widehat\lambda$. The semicolon denotes differentiation in sample coordinates, not another ordinary parameter [derivative](../../../calculus.md#derivative). This [Jacobian determinant](../../../calculus.md#jacobian-determinant) adjustment is essential to the definition.

In the present model set

$$
A(\psi)=\sum_iY_ie^{-\psi x_i},\quad B(\psi)=\sum_i x_iY_ie^{-\psi x_i},\quad C(\psi)=\sum_i x_i^2Y_ie^{-\psi x_i}.
$$

The [log-likelihood](../../../statistical-modelling.md#log-likelihood) is $\ell=-n\log\lambda-\psi\sum_i x_i-A(\psi)/\lambda$. Consequently

$$
\boxed{\widetilde\lambda_\psi=\frac{A(\psi)}n,\qquad\ell_p(\psi)=-n\log\frac{A(\psi)}n-\psi\sum_i x_i-n.}
$$

The profile score is $nB/A-\sum_i x_i$, and its [derivative](../../../calculus.md#derivative) is $-n(C/A-(B/A)^2)$. The expression in parentheses is the [variance](../../../variance.md) of the fixed design values under positive weights proportional to $Y_ie^{-\psi x_i}$. Thus the [profile log-likelihood](../../../statistical-modelling.md#profile-log-likelihood) is strictly concave for a nonconstant design. Its score changes from $n\max_i x_i-\sum_i x_i>0$ to $n\min_i x_i-\sum_i x_i<0$ as $\psi$ goes from $-\infty$ to $+\infty$, giving a unique finite fit. If all $x_i$ coincide, only the mean $\lambda e^{\psi x_i}$ is identifiable and inference on $\psi$ alone is not defined; that exceptional design must be excluded.

The specified ancillary coordinates give $Y_i=\widehat\lambda\exp(\widehat\psi x_i+a_i)$. At fixed $\widehat\psi,a$, therefore,

$$
\frac{\partial Y_i}{\partial\widehat\lambda}=\frac{Y_i}{\widehat\lambda},\qquad \frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}=\frac{\widetilde\lambda_\psi}{\widehat\lambda}.
$$

Meanwhile the constrained [observed information](../../../statistical-modelling.md#observed-fisher-information) is

$$
j_{\lambda\lambda}=\left[-\frac n{\lambda^2}+\frac{2A}{\lambda^3}\right]_{\lambda=\widetilde\lambda_\psi}=\frac n{\widetilde\lambda_\psi^2}.
$$

Substitution proves

$$
\boxed{\ell_m(\psi)=\ell_p(\psi)+\log\widehat\lambda-\frac12\log n=\ell_p(\psi)+\text{constant in }\psi.}
$$

Equivalently the sample [derivative](../../../calculus.md#derivative) of the nuisance score is $\ell_{\lambda;\widehat\lambda}=A/(\lambda^2\widehat\lambda)$, which equals $n/(\widetilde\lambda_\psi\widehat\lambda)$ at the constrained fit and gives the same cancellation. Thus the [modified profile likelihood for exponential regression](../../../statistical-modelling.md#modified-profile-likelihood-for-exponential-regression) is proportional to the ordinary [profile likelihood](../../../statistical-modelling.md#profile-likelihood). This conclusion uses the given ancillary; no proof of its ancillarity is required.

## 3

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [transformation model](../../../statistical-model.md#transformation-model) consists of a [group](../../../group.md) $G$ acting on the [sample space](../../../probability-theory.md#sample-space) and on the set of [statistical parameters](../../../statistical-model.md#statistical-parameter), with the compatibility property

$$
P_{g\theta}=g_*P_\theta,\qquad g\in G.
$$

In words, transforming a sample from $P_\theta$ produces a sample from $P_{g\theta}$. A transitive [transformation model](../../../statistical-model.md#transformation-model) is generated from one reference distribution by the [group action](../../../group-theory.md#group-action). For densities, the compatibility property includes the [Jacobian determinant](../../../calculus.md#jacobian-determinant) of the sample transformation; it is not merely equality of [density](../../../fluid-mechanics.md#density) values at transformed points.

A [maximal invariant](../../../statistical-model.md#maximal-invariant) $A$ is constant on [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action) and separates them: $A(gx)=A(x)$, and $A(x)=A(y)$ implies $y=gx$ for some $g$. An [equivariant estimator](../../../statistical-model.md#equivariant-estimator) $T$ of the parameter satisfies $T(gx)=gT(x)$. Equivariance means the estimate follows the transformed parameter, whereas invariance means the reported value stays unchanged.

First suppose the set of [statistical parameters](../../../statistical-model.md#statistical-parameter) can be identified with the [group](../../../group.md), as happens for a simply transitive action. An [equivariant estimator](../../../statistical-model.md#equivariant-estimator) then provides a group-valued fit $\widehat g(x)$ with $\widehat g(gx)=g\widehat g(x)$. Normalize the sample by this fit:

$$
\boxed{A(x)=\widehat g(x)^{-1}x.}
$$

Indeed $A(gx)=\widehat g(x)^{-1}g^{-1}gx=A(x)$. Conversely, if $A(x)=A(y)$, then $y=\widehat g(y)\widehat g(x)^{-1}x$, placing $x,y$ in the same [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action). This establishes maximality, rather than only invariance.

For a transitive action with a nontrivial [stabilizer](../../../group-theory.md#stabilizer-subgroup) $H$ of a reference parameter $\theta_0$, a parameter-valued [equivariant estimator](../../../statistical-model.md#equivariant-estimator) does not specify a unique normalizing transformation. Choose a section $h_\theta$ with $h_\theta\theta_0=\theta$ and form $b(x)=h_{T(x)}^{-1}x$. Under $g$,

$$
b(gx)=h_{gT(x)}^{-1}g h_{T(x)}b(x),\qquad h_{gT(x)}^{-1}g h_{T(x)}\in H.
$$

Thus the $H$-orbit of $b(x)$ is invariant. It is maximal: if $b(y)=h b(x)$ with $h\in H$, then $y=h_{T(y)}h h_{T(x)}^{-1}x$. Appropriate [measurable](../../../measure-theory.md#measurability) sections and [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action) coordinates are assumed when treating this as a [statistic](../../../statistical-inference.md#statistic). This qualification explains why an arbitrary equivariant [statistic](../../../statistical-inference.md#statistic) alone is not automatically a complete set of invariant coordinates.

For the [location-scale family](../../../statistical-model.md#location-scale-family), write $X_i=\mu+\sigma Z_i$ with $\sigma>0$ and a fixed joint distribution of $Z$. The [group](../../../group.md) consists of maps $x_i\mapsto a+bx_i$ with $b>0$, acting on parameters by $(\mu,\sigma)\mapsto(a+b\mu,b\sigma)$. For a nonconstant sample of size $n\ge2$, take the [equivariant estimator](../../../statistical-model.md#equivariant-estimator)

$$
\widehat\mu=\overline X,\qquad \widehat\sigma=s=\left\{\frac1n\sum_i(X_i-\overline X)^2\right\}^{1/2}.
$$

It gives the [maximal invariant](../../../statistical-model.md#maximal-invariant)

$$
\boxed{A(X)=\left(\frac{X_1-\overline X}s,\ldots,\frac{X_n-\overline X}s\right).}
$$

Its coordinates satisfy $\sum_iA_i=0$ and $\sum_iA_i^2=n$. They stay unchanged under location and positive-scale transformations. If two samples have the same standardized [vector](../../../vector-space.md#vector), then

$$
y_i=\overline y+\frac{s_y}{s_x}(x_i-\overline x),
$$

so a single [group](../../../group.md) transformation maps the first sample onto the second. The [vector](../../../vector-space.md#vector) retains the observation labels: sorting it would discard information not removed by this location-scale [group](../../../group.md). The construction is algebraic and does not require the underlying distribution to have finite [moments](../../../probability-theory.md#moment). Constant samples can be assigned a separate invariant value; they form a single exceptional [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action) and have probability zero under an independent continuous base distribution.

Finally, in a transitive [transformation model](../../../statistical-model.md#transformation-model) every invariant [statistic](../../../statistical-inference.md#statistic) is ancillary. Choose $g$ taking $\theta_0$ to $\theta$ and use $X_\theta\overset d=gX_{\theta_0}$; invariance gives $A(X_\theta)\overset d=A(X_{\theta_0})$. Thus the standardized residual configuration provides a natural conditioning variable, while the equivariant fit contains the location and scale information.

## 4

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [statistical functional](../../../statistical-inference.md#statistical-functional) is a map $T$ defined on a class of [probability distributions](../../../probability-theory.md#probability-distribution). Its associated [functional statistic](../../../statistical-inference.md#functional-statistic) is $T(F_n)$, where $F_n=n^{-1}\sum_i\delta_{X_i}$ is the [empirical distribution](../../../information-theory.md#type-information-theory) and each $\delta_{X_i}$ is a [Dirac measure](../../../measure-theory.md#dirac-measure). For example, $T(F)=\int x\,dF(x)$ yields the [sample mean](../../../variance.md#sample-mean). The [influence function](../../../statistical-inference.md#influence-function) records the [derivative](../../../calculus.md#derivative) in the direction of point contamination:

$$
\operatorname{IF}(z;T,F)=\left.\frac{d}{d\varepsilon}T\big((1-\varepsilon)F+\varepsilon\delta_z\big)\right|_{\varepsilon=0+}.
$$

It is a local, infinitesimal robustness diagnostic, not a description of arbitrary large contamination.

Suppose $T$ is differentiable in a sense strong enough to linearize it at the [empirical distribution](../../../information-theory.md#type-information-theory), and that its [derivative](../../../calculus.md#derivative) in a signed direction $G-F$ is $\int\operatorname{IF}(x;T,F)\,d(G-F)(x)$. Averaging the directions $\delta_z-F$ over $z\sim F$ gives the zero direction, so linearity implies $\int\operatorname{IF}\,dF=0$. The resulting [asymptotic linear representation](../../../statistical-inference.md#asymptotic-linear-representation) is

$$
T(F_n)-T(F)=\frac1n\sum_i\operatorname{IF}(X_i;T,F)+o_p(n^{-1/2}).
$$

If $\int\operatorname{IF}^2\,dF<\infty$, the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) and the negligible remainder give

$$
\boxed{\sqrt n\{T(F_n)-T(F)\}\ \xrightarrow{d}\ N\left(0,\int\operatorname{IF}(x;T,F)^2\,dF(x)\right).}
$$

Thus the [asymptotic variance](../../../statistical-modelling.md#asymptotic-variance) is $n^{-1}\int\operatorname{IF}^2\,dF$. For a vector functional the integral is $n^{-1}\int\operatorname{IF}\operatorname{IF}^{\mathsf T}\,dF$. Convergence of the actual finite-sample [variance](../../../variance.md) to this leading expression additionally requires control of second moments of the remainder, or an appropriate [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) condition; [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) alone does not provide that. Existence of a contamination [derivative](../../../calculus.md#derivative) by itself also does not guarantee the required empirical linearization.

Several complementary robustness measures follow. [Gross-error sensitivity](../../../statistical-inference.md#gross-error-sensitivity) is $\gamma^*=\sup_z|\operatorname{IF}(z)|$. Under contamination $(1-\varepsilon)F+\varepsilon H$, the first-order bias is $\varepsilon\int\operatorname{IF}\,dH$, whose worst absolute coefficient is $\gamma^*$; bounded influence therefore bounds infinitesimal gross-error bias. The [local-shift sensitivity](../../../statistical-inference.md#local-shift-sensitivity) is $\lambda^*=\sup_{x\ne y}|\operatorname{IF}(x)-\operatorname{IF}(y)|/|x-y|$, equal to $\sup|\operatorname{IF}'|$ when the [influence function](../../../statistical-inference.md#influence-function) is smoothly differentiable. It measures the effect of moving a contaminant a small distance. The [rejection point of an influence function](../../../statistical-inference.md#rejection-point-of-an-influence-function) is $\rho^*=\inf\{r:\operatorname{IF}(x)=0\text{ for }|x|>r\}$, using centered, standardized coordinates; it is infinite if there is no such cutoff. A finite cutoff completely rejects sufficiently extreme observations to first order. These measures address different aspects of robustness. The integral of squared influence controls asymptotic precision and efficiency, while [breakdown point](../../../statistical-inference.md#breakdown-point) concerns finite amounts of contamination and is not determined by bounded influence alone.

For the [quantile](../../../probability-theory.md#quantile-function), assume $0<p<1$, a unique solution $q=q_p(F)$, and a [density](../../../fluid-mechanics.md#density) continuous and positive at $q$. Define [quantiles](../../../probability-theory.md#quantile-function) of the contaminated distribution by generalized inversion, since a distribution with a point mass need not attain $p$ as an equality. If $z\ne q$, its indicator is constant near $q$ for sufficiently small contamination, and differentiating

$$
(1-\varepsilon)F(q_\varepsilon)+\varepsilon\mathbf1_{z\le q_\varepsilon}=p
$$

at zero gives $-p+f(q)q'_0+\mathbf1_{z\le q}=0$. Hence

$$
\boxed{\operatorname{IF}(z;q_p,F)=\frac{p-\mathbf1_{z\le q}}{f(q)}\quad(F\text{-almost every }z).}
$$

At the exceptional point $z=q$, the generalized-inverse [quantile](../../../probability-theory.md#quantile-function) remains exactly $q$: below $q$ the contaminated [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is below $p$, and its value at $q$ exceeds $p$. Its actual [derivative](../../../calculus.md#derivative) there is zero. The usual step-function expression is an almost-everywhere version, which is all that the [asymptotic variance](../../../statistical-modelling.md#asymptotic-variance) needs. Its mean is zero, and its second moment is

$$
\frac{p(p-1)^2+(1-p)p^2}{f(q)^2}=\frac{p(1-p)}{f(q)^2}.
$$

Therefore the [influence function of a quantile](../../../statistical-inference.md#influence-function-of-a-quantile) gives [asymptotic variance](../../../statistical-modelling.md#asymptotic-variance) $p(1-p)/(nf(q)^2)$ and [gross-error sensitivity](../../../statistical-inference.md#gross-error-sensitivity) $\max(p,1-p)/f(q)$. Its jump makes [local-shift sensitivity](../../../statistical-inference.md#local-shift-sensitivity) infinite, and its nonzero constant tails make its rejection point infinite. If $f(q)=0$ or the [quantile](../../../probability-theory.md#quantile-function) is not unique, this regular derivation does not apply.

## 5

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Discarding zero observations and resolving ties is unnecessary with probability one under the stated independent continuous model. Rank the absolute observations from $1$ to $n$, let $R_i$ be the rank of $|X_i|$, and form the positive [Wilcoxon signed-rank statistic](../../../nonparametric-statistics.md#wilcoxon-signed-rank-statistic)

$$
W^+=\sum_iR_i\mathbf1_{X_i>0}.
$$

Reject the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) for large $W^+$. Under symmetry about zero, each sign is a fair independent binary variable, independent of all the absolute values. To see this [independence](../../../random-variable.md#independent-random-variables), for every [measurable](../../../measure-theory.md#measurability) positive set $B$, symmetry gives $\Pr(X\in B)=\Pr(X\in-B)=\tfrac12\Pr(|X|\in B)$. [Independence](../../../random-variable.md#independent-random-variables) of observations then gives [independence](../../../random-variable.md#independent-random-variables) of the whole sign vector from the absolute-value vector. Conditional on those absolute values, relabeling by rank therefore gives

$$
W^+\overset d=\sum_{r=1}^n rB_r,\qquad B_r\text{ independent Bernoulli}(1/2).
$$

The null distribution is consequently independent of the unknown symmetric shape. Its [probability generating function](../../../probability-theory.md#probability-generating-function) is $2^{-n}\prod_{r=1}^n(1+z^r)$, so the coefficient of $z^w$ gives the exact probability of $W^+=w$. Choose an upper critical value with null tail probability at most the desired level, or randomize at the boundary to obtain that level exactly. The observed upper-tail probability is an exact one-sided [p-value](../../../statistical-modelling.md#p-value). A positive translation raises each [Walsh average](../../../nonparametric-statistics.md#walsh-average), as established below, so this upper-tail rule has the correct direction against positive centers for every fixed symmetric shape.

The independent-sign representation proves

$$
\boxed{E_0W^+=\frac12\sum_{r=1}^n r=\frac{n(n+1)}4,\qquad \operatorname{Var}_0W^+=\frac14\sum_{r=1}^n r^2=\frac{n(n+1)(2n+1)}{24}.}
$$

The asymptotic null distribution, stated without proof, is

$$
\boxed{\frac{W^+-n(n+1)/4}{\sqrt{n(n+1)(2n+1)/24}}\ \xrightarrow{d}\ N(0,1).}
$$

This supplies the usual upper [normal distribution](../../../probability-theory.md#normal-distribution) critical value when exact calculation is inconvenient; for the discrete upper tail $\Pr(W^+\ge c)$, use $c-1/2$ in the [continuity correction](../../../convergence-of-random-variables.md#continuity-correction).

For exact equivalence with the proposed [statistic](../../../statistical-inference.md#statistic), reorder the observations so $|X_{(1)}|<\cdots<|X_{(n)}|$. Partition the unordered pairs, including diagonals, by the member with larger absolute value. The block belonging to $X_{(r)}$ consists of the $r-1$ pairs with an earlier member and its diagonal pair. For an earlier member $X_{(j)}$, the strict inequality $|X_{(j)}|<|X_{(r)}|$ means the sign of $X_{(j)}+X_{(r)}$ is the sign of $X_{(r)}$; the diagonal sum has that same sign. Thus the entire block supplies exactly $r$ positive averages when $X_{(r)}>0$, and none otherwise. Summing the blocks proves

$$
\boxed{\#\{(i,j):i\le j,\ (X_i+X_j)/2>0\}=\sum_{r=1}^n r\mathbf1_{X_{(r)}>0}=W^+.}
$$

The two tests therefore have exactly the same [statistic](../../../statistical-inference.md#statistic), critical values and [p-values](../../../statistical-modelling.md#p-value), not merely the same limiting distribution. The [Walsh averages](../../../nonparametric-statistics.md#walsh-average) are dependent, so their positivity indicators must not instead be treated as an independent binomial sample. For a translation $X_i=Z_i+\theta$ of any null-symmetric sample, every [Walsh average](../../../nonparametric-statistics.md#walsh-average) increases by $\theta$; their positive count is nondecreasing, which also verifies the direction of the one-sided test.

## 6

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Saddlepoint approximation methods retain the nonquadratic shape of a distribution through its [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function). Suppose $X_1,\ldots,X_n$ are independent and identically distributed, $K(t)=\log E(e^{tX_1})$ is finite on an open interval containing zero, and $K''>0$. For an interior target mean $x$, solve the saddlepoint equation $K'(t)=x$. Introduce [exponential tilting](../../../probability-theory.md#exponential-tilting) by

$$
dP_t(y)=e^{ty-K(t)}\,dP(y).
$$

Under the tilted distribution the mean and [variance](../../../variance.md) are $K'(t)=x$ and $K''(t)$. For the product sample the [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) is $e^{t\sum_iX_i-nK(t)}$. Consequently the exact [density](../../../fluid-mechanics.md#density) relation for the [sample mean](../../../variance.md#sample-mean) is

$$
f_{\overline X}(x)=e^{n(K(t)-tx)}f_{\overline X,t}(x).
$$

A local central limit approximation to the tilted [density](../../../fluid-mechanics.md#density) at its own mean gives $f_{\overline X,t}(x)\simeq\sqrt{n/(2\pi K''(t))}$. Hence

$$
\boxed{f_{\overline X}(x)\simeq\sqrt{\frac n{2\pi K''(t)}}\exp\{n(K(t)-tx)\},\qquad K'(t)=x.}
$$

For the sum $S_n$, the equivalent expression is $f_{S_n}(s)\simeq e^{nK(t)-ts}/\sqrt{2\pi nK''(t)}$, with $K'(t)=s/n$. Under the usual smooth nonlattice [density](../../../fluid-mechanics.md#density) conditions this approximation has relative error of order $n^{-1}$ for a fixed interior target. In the tilted [Edgeworth expansion](../../../probability-theory.md#edgeworth-series) the order $n^{-1/2}$ odd term vanishes at the mean. The exponent retains the Legendre-transform rate $I(x)=tx-K(t)$, rather than a quadratic Taylor approximation to that rate, explaining the useful tail and skewness behavior. Normalization is not automatic, and accuracy statements need their regularity and range restrictions.

For a [normal distribution](../../../probability-theory.md#normal-distribution), $K(t)=\mu t+\sigma^2t^2/2$ and $t=(x-\mu)/\sigma^2$. Substitution recovers exactly the normal [density](../../../fluid-mechanics.md#density) of the [sample mean](../../../variance.md#sample-mean). For an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\lambda$, $K(t)=-\log(1-t/\lambda)$, $t=\lambda-1/x$ and $K''(t)=x^2$. The approximation becomes

$$
\sqrt{\frac n{2\pi}}\,\lambda^n e^n x^{n-1}e^{-n\lambda x},\qquad x>0.
$$

It has exactly the gamma [density](../../../fluid-mechanics.md#density) shape. Replacing its leading constant by the exact [normalizing constant](../../../continuous-probability-distribution.md#normalizing-constant) makes it exact, illustrating why exactness of shape and exactness of the unnormalized approximation are separate questions.

For a vector [sample mean](../../../variance.md#sample-mean), tilt by $e^{t^{\mathsf T}y-K(t)}$, solve $\nabla K(t)=x$, and use the local multivariate normal [density](../../../fluid-mechanics.md#density) at the tilted mean. This gives

$$
f_{\overline X}(x)\simeq\frac{(n/(2\pi))^{d/2}}{\sqrt{\det K''(t)}}\exp\{n(K(t)-t^{\mathsf T}x)\}.
$$

Joint and marginal saddlepoint densities can also be divided to approximate conditional densities, for example after conditioning on a nuisance [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic). The [p\* approximation](../../../probability-theory.md#p-star-approximation) uses [likelihood](../../../statistical-modelling.md#likelihood-function) and fitted-information coordinates to obtain a closely related approximation to a [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator)'s [density](../../../fluid-mechanics.md#density), usually conditional on an [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic).

Tail probabilities need a corresponding integration approximation. The [Lugannani-Rice saddlepoint tail approximation](../../../probability-theory.md#lugannani-rice-saddlepoint-tail-approximation) uses

$$
w=\operatorname{sgn}(t)\sqrt{2n\{tx-K(t)\}},\qquad u=t\sqrt{nK''(t)},
$$

and gives

$$
\boxed{\Pr(\overline X\le x)\simeq\Phi(w)+\phi(w)\left(\frac1w-\frac1u\right).}
$$

Here $\Phi,\phi$ are the standard [normal distribution](../../../probability-theory.md#normal-distribution) functions. The upper-tail correction has the opposite sign: $1-\Phi(w)+\phi(w)(1/u-1/w)$. Inverting a [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) introduces a pole in addition to the [density](../../../fluid-mechanics.md#density)'s saddlepoint; treating both supplies the correction term, which is why simply integrating a normal approximation at the untilted mean is less accurate. At $x=K'(0)$ the apparent singularities cancel. With $v=K''(0)$ and $k=K'''(0)$, expansions give $w=t\sqrt{nv}(1+kt/(3v)+O(t^2))$ and $u=t\sqrt{nv}(1+kt/(2v)+O(t^2))$, so $1/w-1/u\to k/(6\sqrt n\,v^{3/2})$. For the [normal distribution](../../../probability-theory.md#normal-distribution) the correction is zero everywhere.

These methods require care for lattice distributions, where summation and lattice corrections replace the [density](../../../fluid-mechanics.md#density) inversion, and near boundaries or singular [covariance](../../../variance.md#covariance) matrices. A distribution with no [moment-generating function](../../../probability-theory.md#moment-generating-function) in a neighborhood of zero does not satisfy the starting assumptions. A successful saddlepoint approximation is therefore a structured refinement of regular asymptotic inference, not a formula guaranteed uniformly in every tail or for every model.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Partition a regular parameter as $(\psi,\lambda)$, with interest $\psi$ and nuisance $\lambda$. [Orthogonal statistical parameters](../../../statistical-modelling.md#orthogonal-statistical-parameters) have zero cross-block of expected [Fisher information](../../../statistical-modelling.md#fisher-information-matrix),

$$
I_{\psi\lambda}=E(U_\psi U_\lambda^{\mathsf T})=-E\ell_{\psi\lambda}=0.
$$

This may hold at one parameter value or throughout a parametrization. It is expected-information orthogonality, and does not generally force the [observed information](../../../statistical-modelling.md#observed-fisher-information) cross-block to vanish in each sample.

First, the asymptotic [covariance](../../../variance.md#covariance) of the joint [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is the inverse information. Orthogonality makes this matrix block diagonal, giving first-order asymptotic [independence](../../../random-variable.md#independent-random-variables) of interest and nuisance fits. The [efficient information](../../../statistical-inference.md#efficient-information) with unknown nuisance is

$$
I_{\psi\psi\cdot\lambda}=I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

For orthogonal parameters it equals $I_{\psi\psi}$. Thus estimating the nuisance creates no first-order information loss relative to knowing it, at the orthogonal point. This is a local asymptotic statement, not a general finite-sample [independence](../../../random-variable.md#independent-random-variables) theorem.

Second, orthogonality stabilizes constrained nuisance estimates. Differentiating $\ell_\lambda(\psi,\widetilde\lambda_\psi)=0$ gives

$$
\frac{d\widetilde\lambda_\psi}{d\psi}=-j_{\lambda\lambda}^{-1}j_{\lambda\psi}.
$$

When the expected cross-information vanishes, regular sampling fluctuations give $j_{\lambda\psi}=O_p(\sqrt n)$ and $j_{\lambda\lambda}=O_p(n)$. The [derivative](../../../calculus.md#derivative) is therefore $O_p(n^{-1/2})$ locally. Changing the interest parameter by $O_p(n^{-1/2})$ changes its constrained nuisance fit by only $O_p(n^{-1})$, smaller than the ordinary nuisance estimation error. This reduces sensitivity to how the nuisance is fitted and simplifies higher-order [likelihood](../../../statistical-modelling.md#likelihood-function) adjustments.

For scalar interest, [local orthogonal nuisance reparametrization](../../../statistical-modelling.md#local-orthogonal-nuisance-reparametrization) can often be constructed explicitly. Keep $\psi$ and write the original nuisance as $\lambda(\psi,\eta)$. The transformed interest score is $U_\psi+\lambda_\psi^{\mathsf T}U_\lambda$. Its [covariance](../../../variance.md#covariance) with the new nuisance score vanishes when

$$
\frac{\partial\lambda}{\partial\psi}=-I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

With smooth nonsingular nuisance information, this ordinary differential equation has a local solution for suitable initial nuisance coordinates. For several interest coordinates the corresponding equations need compatibility conditions; global orthogonality is not automatic.

The normal model gives a transparent example. For independent observations with mean $\mu$ and [variance](../../../variance.md) $\nu$, direct score expectations give

$$
I_{\mu\mu}=\frac n\nu,\qquad I_{\nu\nu}=\frac n{2\nu^2},\qquad I_{\mu\nu}=0.
$$

The cross-information is zero because the centered normal third [moment](../../../probability-theory.md#moment) is zero. When fitting $\nu$ at fixed $\mu$,

$$
\widetilde\nu_\mu=\frac1n\sum_i(X_i-\mu)^2=\widehat\nu+(\mu-\overline X)^2,
$$

so the change is indeed quadratic in a local change of the mean.

Orthogonality is also useful for removing nuisance effects beyond first order. Take [variance](../../../variance.md) $\nu$ as interest and mean $\mu$ as nuisance. Put $Q=\sum_i(X_i-\overline X)^2$. The [profile log-likelihood](../../../statistical-modelling.md#profile-log-likelihood) is $\ell_p(\nu)=-\tfrac n2\log\nu-Q/(2\nu)$ up to a constant. The constrained mean is $\widetilde\mu_\nu=\overline X$ for all $\nu$, so its sample-coordinate [Jacobian determinant](../../../calculus.md#jacobian-determinant) is one, and $j_{\mu\mu}=n/\nu$. The information adjustment gives

$$
\boxed{\ell_m(\nu)=\ell_p(\nu)-\tfrac12\log(n/\nu)=-\frac{n-1}2\log\nu-\frac Q{2\nu}+\text{constant}.}
$$

This agrees with the exact [likelihood](../../../statistical-modelling.md#likelihood-function) based on $Q/\nu\sim\chi^2_{n-1}$: estimating the mean has used one degree of freedom. In this setting the [Cox-Reid adjusted profile likelihood](../../../statistical-modelling.md#cox-reid-adjusted-profile-likelihood) has the same form. The exact distribution follows by projecting the centered normal vector onto the $(n-1)$-dimensional subspace orthogonal to the constant vector; an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) there supplies $n-1$ independent standard normal coordinates whose squares sum to $Q/\nu$.

The example shows both the benefit and the limits. Orthogonality organizes first-order precision and nuisance stability; it does not eliminate all higher-order nuisance effects. Nor does it identify an [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) or justify dropping the sample-coordinate factor in every [modified profile likelihood](../../../statistical-modelling.md#modified-profile-likelihood). In the exponential regression calculation that factor cancels the information adjustment, so an information-only correction would give a different answer.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

An [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) has a [sampling distribution](../../../statistical-modelling.md#sampling-distribution) independent of the unknown parameter. It describes a realized aspect of the sample configuration without supplying a marginal [likelihood](../../../statistical-modelling.md#likelihood-function) for the parameter. Its observed value can nevertheless be crucial to the precision of inference from the rest of the data. In a transitive [transformation model](../../../statistical-model.md#transformation-model), invariance gives a common distribution under every parameter value, so [maximal invariants](../../../statistical-model.md#maximal-invariant) provide natural ancillaries, such as the standardized configuration in a [location-scale family](../../../statistical-model.md#location-scale-family).

Conditional inference uses the [sampling distribution](../../../statistical-modelling.md#sampling-distribution) of an estimator or [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) conditional on the observed ancillary. With joint coordinates $(T,A)$, the factorization

$$
f_\theta(t,a)=f_\theta(t\mid a)f_A(a)
$$

shows that the conditional [likelihood](../../../statistical-modelling.md#likelihood-function) and the joint [likelihood](../../../statistical-modelling.md#likelihood-function) differ only by a parameter-free data factor. Conditional reference distributions, [confidence intervals](../../../statistical-inference.md#confidence-interval) and [p-values](../../../statistical-modelling.md#p-value) can still differ markedly from unconditional ones, because they adapt to the realized configuration. For a continuous ancillary one uses a [regular conditional distribution](../../../probability-theory.md#regular-conditional-distribution) or [conditional density](../../../probability-theory.md#conditional-density); dividing by the zero probability of a single ancillary value is not a valid definition.

An exact example makes this adaptation visible. Let independent observations be uniform on $(\theta-1/2,\theta+1/2)$, with $n\ge2$. Put $U=X_{(1)}$, $V=X_{(n)}$, $R=V-U$ and $C=(U+V)/2$. Specifying the minimum and maximum contributes $n(n-1)$ choices of observations, while each remaining observation must lie between them. Hence

$$
f_{U,V}(u,v)=n(n-1)(v-u)^{n-2},\quad \theta-\tfrac12<u<v<\theta+\tfrac12.
$$

The transformation $u=c-r/2$, $v=c+r/2$ has unit absolute [Jacobian determinant](../../../calculus.md#jacobian-determinant). Its support is $0<r<1$, $|c-\theta|<(1-r)/2$. Integrating over $c$ gives

$$
f_R(r)=n(n-1)r^{n-2}(1-r),\qquad 0<r<1,
$$

which is independent of $\theta$, proving that the range is ancillary. Dividing the joint [density](../../../fluid-mechanics.md#density) by this marginal [density](../../../fluid-mechanics.md#density) gives

$$
C\mid R=r\sim\operatorname{Uniform}\left(\theta-\frac{1-r}2,\theta+\frac{1-r}2\right).
$$

The centered conditional pivot is uniform, so

$$
\boxed{\left[C-\frac{(1-\alpha)(1-R)}2,\ C+\frac{(1-\alpha)(1-R)}2\right]}
$$

has conditional coverage $1-\alpha$ at every $0<r<1$, and hence unconditional coverage $1-\alpha$ as well. A large realized range leaves little room for translating the interval and gives more precise inference. This is [range-conditioned uniform location inference](../../../probability-and-statistics.md#range-conditioned-uniform-location-inference). The range and center are not independent: the conditional spread depends on the range, even though the range is ancillary.

Completeness can give [independence](../../../random-variable.md#independent-random-variables) in other models. Suppose $S$ is a [complete sufficient statistic](../../../probability-and-statistics.md#complete-sufficient-statistic) and $A$ is ancillary. For any bounded [measurable](../../../measure-theory.md#measurability) $h$, sufficiency makes $g(S)=E_\theta(h(A)\mid S)$ a function independent of $\theta$, while ancillarity makes $c=E_\theta h(A)$ independent of $\theta$. Since $E_\theta(g(S)-c)=0$ for every $\theta$, completeness implies $g(S)=c$ almost surely. Taking all bounded indicator functions $h$ proves [independence](../../../random-variable.md#independent-random-variables) of $A$ and $S$. This is the content of [Basu's theorem](../../../probability-and-statistics.md#basu-s-theorem), with the proof displaying precisely where sufficiency and completeness are used. Without completeness the conclusion fails: in the uniform location example the minimum and maximum are sufficient, and contain the nondegenerate ancillary range.

There are practical qualifications. Ancillaries need not be unique, and some models supply only approximate ancillary coordinates; one must specify the conditioning surface and the accuracy intended. Conditioning on a [statistic](../../../statistical-inference.md#statistic) sufficient for a [nuisance parameter](../../../statistical-model.md#nuisance-parameter) is a different device: it may remove that nuisance even though the [statistic](../../../statistical-inference.md#statistic) is not ancillary for the full parameter. Conditioning indiscriminately can discard useful information. In higher-order [likelihood](../../../statistical-modelling.md#likelihood-function) inference, the ancillary coordinates specify how the fitted data are varied, entering both the p\* [density](../../../fluid-mechanics.md#density) and the sample [derivatives](../../../calculus.md#derivative) in the [modified profile likelihood](../../../statistical-modelling.md#modified-profile-likelihood). Their role is therefore substantive, rather than merely a label for an extra [statistic](../../../statistical-inference.md#statistic).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
