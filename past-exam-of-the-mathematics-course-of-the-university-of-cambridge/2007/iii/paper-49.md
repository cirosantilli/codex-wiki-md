# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper49.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [cubic spline](../../../uniform-approximation.md#cubic-spline) belongs to $C^2[a,b]$ and is a [polynomial](../../../polynomial.md) of degree at most three on each interval separated by the [spline knots](../../../uniform-approximation.md#spline-knot). A [natural cubic spline](../../../uniform-approximation.md#natural-cubic-spline) is additionally an [affine function](../../../vector-space.md#affine-function) on the exterior intervals $[a,x_1]$ and $[x_n,b]$. On $[x_1,x_n]$ this is equivalent to the endpoint conditions $s''(x_1)=s''(x_n)=0$; these conditions remain part of the definition when an outer knot coincides with $a$ or $b$.

Let $s$ be the [natural cubic spline interpolant](../../../uniform-approximation.md#natural-cubic-spline-interpolant) of the prescribed values, and let $v$ be any other interpolating $C^2$ function. Set $u=v-s$, so $u(x_i)=0$. On the interval $[x_i,x_{i+1}]$, [integration by parts](../../../calculus.md#integration-by-parts) twice gives

$$
\int_{x_i}^{x_{i+1}}s''u''=[s''u']_{x_i}^{x_{i+1}}-[s'''u]_{x_i}^{x_{i+1}},
$$

because the fourth [derivative](../../../calculus.md#derivative) of each cubic piece is zero. The second boundary term is zero because $u$ vanishes at the [spline knots](../../../uniform-approximation.md#spline-knot). After summing the first terms, the interior contributions cancel by [continuity](../../../calculus.md#continuous-function) of $s''$ and $u'$, and the two remaining terms vanish by the natural endpoint conditions. On the exterior intervals $s''=0$. Thus $\int_a^b s''u''=0$, and the [second derivative roughness penalty](../../../uniform-approximation.md#second-derivative-roughness-penalty) satisfies

$$
R(v'')=R(s'')+R(u'')\geq R(s'').
$$

If equality holds, the continuous nonnegative function $(u'')^2$ has zero integral, so $u''=0$ everywhere. Hence $u$ is an [affine function](../../../vector-space.md#affine-function), and its zeros at two distinct [spline knots](../../../uniform-approximation.md#spline-knot) force $u=0$. This proves the [minimum roughness property of the natural cubic spline interpolant](../../../uniform-approximation.md#minimum-roughness-property-of-the-natural-cubic-spline-interpolant) and its equality case: **the unique minimum-roughness interpolant is $s$**.

For the [fixed-design nonparametric regression](../../../nonparametric-statistics.md#fixed-design-nonparametric-regression) fit, use the [penalized least squares](../../../statistical-learning.md#penalized-least-squares) criterion

$$
\boxed{S_\lambda(v)=\sum_{i=1}^n\{Y_i-v(x_i)\}^2+\lambda\int_a^b v''(x)^2\,dx.}
$$

Let $s_z$ be the [natural cubic spline interpolant](../../../uniform-approximation.md#natural-cubic-spline-interpolant) with value [vector](../../../vector-space.md#vector) $z=(z_1,\ldots,z_n)^T$. Replacing $v$ by $s_z$ for $z_i=v(x_i)$ leaves the residual sum unchanged and reduces the [second derivative roughness penalty](../../../uniform-approximation.md#second-derivative-roughness-penalty), strictly unless $v=s_z$. It therefore remains to minimize the finite-dimensional [quadratic form](../../../linear-algebra.md#quadratic-form)

$$
Q_\lambda(z)=\|Y-z\|^2+\lambda z^TKz.
$$

The supplied [spline roughness penalty matrix](../../../uniform-approximation.md#spline-roughness-penalty-matrix) $K$ is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix). For every nonzero [vector](../../../vector-space.md#vector) $w$,

$$
w^T(I+\lambda K)w=\|w\|^2+\lambda w^TKw>0.
$$

Consequently $I+\lambda K$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), and $Q_\lambda$ is [strictly convex](../../../real-analysis.md#strictly-convex-function). Its [normal equations for linear least squares](../../../linear-regression.md#normal-equations-for-linear-least-squares) have the unique solution

$$
\boxed{\widehat z=(I+\lambda K)^{-1}Y,\qquad \widehat g_\lambda=s_{\widehat z}.}
$$

The preceding strict reduction also proves uniqueness over the whole class $C^2[a,b]$, not just over the [natural cubic splines](../../../uniform-approximation.md#natural-cubic-spline). This is the [cubic smoothing spline](../../../nonparametric-statistics.md#cubic-smoothing-spline). If the residual criterion is divided by $n$ instead, the corresponding formula is $(I+n\lambda K)^{-1}Y$, reflecting a change in the numerical convention for the [smoothing parameter](../../../nonparametric-statistics.md#smoothing-parameter).

The [independence](../../../random-variable.md#independent-random-variables) and specified error [mean](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) are not needed for existence or uniqueness of this minimizer. They do imply, with [smoothing matrix](../../../nonparametric-statistics.md#smoothing-matrix) $A_\lambda=(I+\lambda K)^{-1}$ and $g_X=(g(x_i))_i$, that $\mathbb E\widehat z=A_\lambda g_X$ and $\operatorname{Cov}(\widehat z)=\sigma^2A_\lambda^2$. The [null space](../../../linear-algebra.md#kernel-of-a-linear-map) of $K$ consists of sampled [affine functions](../../../vector-space.md#affine-function): these have zero roughness, and conversely zero roughness forces their [natural cubic spline interpolant](../../../uniform-approximation.md#natural-cubic-spline-interpolant) to be an [affine function](../../../vector-space.md#affine-function). Thus these functions are reproduced without [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator), while other components are smoothed.

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

At a target $t$, [local polynomial regression](../../../nonparametric-statistics.md#local-polynomial-regression) fits a [polynomial](../../../polynomial.md) of degree at most $p$ by [weighted least squares](../../../statistical-modelling.md#weighted-least-squares):

$$
\widehat\beta=\arg\min_{\beta\in\mathbb R^{p+1}}\sum_{i=1}^nK\!\left(\frac{x_i-t}{h}\right)\left\{Y_i-\sum_{j=0}^p\beta_j(x_i-t)^j\right\}^2.
$$

Define the response [vector](../../../vector-space.md#vector) $Y=(Y_1,\ldots,Y_n)^T$, the [design matrix](../../../linear-regression.md#design-matrix) $X$ by $X_{i,j+1}=(x_i-t)^j$ for $j=0,\ldots,p$, and the [diagonal matrix](../../../linear-algebra.md#diagonal-matrix) $W$ by $W_{ii}=K((x_i-t)/h)$. The [normal equations for linear least squares](../../../linear-regression.md#normal-equations-for-linear-least-squares) give

$$
\boxed{\widehat\beta=(X^TWX)^{-1}X^TWY,\qquad\widehat m_h(t;p)=\widehat\beta_0.}
$$

This formula assumes the [local polynomial Gram matrix](../../../nonparametric-statistics.md#local-polynomial-gram-matrix) $X^TWX$ is invertible. It is invertible whenever at least $p+1$ distinct sites have positive weights: a nonzero degree-$p$ [polynomial](../../../polynomial.md) cannot vanish at all of them. With fixed $p$, a nonzero continuous [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression), and $nh\to\infty$, this condition holds eventually at the target points considered here. Using weights $h^{-1}K((x_i-t)/h)$ instead gives exactly the same fit.

Use the usual unit-integral normalization $\mu_0(K)=1$. A [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression) need not intrinsically have unit integral, but multiplying all weights by a positive constant leaves [local polynomial regression](../../../nonparametric-statistics.md#local-polynomial-regression) unchanged. With unnormalized raw moments the interior coefficient below is $\mu_2(K)/\mu_0(K)$; the version written using $\mu_2(K)$ alone requires this normalization. A zero [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression) cannot define an estimator.

Write the local moment sums as

$$
A_r(t)=\frac1{nh}\sum_{i=1}^n(x_i-t)^rK\!\left(\frac{x_i-t}{h}\right),\qquad r=0,1,2,\ldots.
$$

The [local constant estimator](../../../nonparametric-statistics.md#nadaraya-watson-estimator) is $\widehat m_h(t;0)=\sum_iK((x_i-t)/h)Y_i/\sum_iK((x_i-t)/h)$. Since the errors have zero [mean](../../../probability-theory.md#expected-value), its [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) is the corresponding weighted average of $m(x_i)-m(t)$. By the second-order [Taylor expansion](../../../calculus.md#taylor-expansion), uniformly for contributing sites with $|x_i-t|\leq h$,

$$
m(x_i)-m(t)=m'(t)(x_i-t)+\frac12m''(t)(x_i-t)^2+r_{i,n},\qquad |r_{i,n}|\leq\eta_n|x_i-t|^2,
$$

where $\eta_n\to0$. This uniform remainder follows from uniform [continuity](../../../calculus.md#continuous-function) of $m''$ on $[0,1]$. Nonnegativity of the [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression) therefore gives

$$
\operatorname{Bias}\{\widehat m_h(t;0)\}=m'(t)\frac{A_1(t)}{A_0(t)}+\frac12m''(t)\frac{A_2(t)}{A_0(t)}+o(h^2)
$$

whenever $A_0$ tends to a positive limit and $A_2=O(h^2)$.

For fixed interior $x$, the moment approximations give $A_0(x)=1+o(1)$, $A_1(x)=O(n^{-1})$, and $A_2(x)=h^2\mu_2(K)+o(h^2)$. The hypothesis $nh^2\to\infty$ makes $n^{-1}=o(h^2)$, so the odd-moment contribution is negligible at second order. Thus

$$
\boxed{\mathbb E\widehat m_h(x;0)-m(x)=\frac12h^2\mu_2(K)m''(x)+o(h^2).}
$$

The symmetry of the [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression) is what removes the first-order interior [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator).

At $z_n=\alpha h$, the rescaled observation window is truncated to $[-\alpha,1]$. Put $\mu_{r,\alpha}=\int_{-\alpha}^1u^rK(u)\,du$ and $\beta_r=\mu_{r,\alpha}/\mu_{0,\alpha}$. Symmetry, nonnegativity, and unit mass give $\mu_{0,\alpha}\geq1/2$. The supplied moment approximations already imply the leading [boundary bias of local constant regression](../../../nonparametric-statistics.md#boundary-bias-of-local-constant-regression):

$$
\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(0)+o(h).
$$

To retain the second-order term rigorously, we need slightly more precise control of the first moment. The rescaled grid $u_i=i/(nh)-\alpha$ has spacing $1/(nh)$. Each truncated function $u^rK(u)\mathbf1_{[-\alpha,1]}$ has [bounded variation](../../../real-analysis.md#total-variation-of-a-function), because $K$ is continuously differentiable on its support. The [Riemann sum](../../../real-analysis.md#riemann-sum) error is bounded by this variation times the grid spacing: summing the oscillation bounds on the grid cells proves

$$
\frac{A_r(z_n)}{h^r}=\mu_{r,\alpha}+O((nh)^{-1}).
$$

Endpoint cells, including the omitted site at zero, contribute the same error order. Consequently

$$
\frac{A_1(z_n)}{A_0(z_n)}=h\beta_1+O(n^{-1}),\qquad
\frac{A_2(z_n)}{A_0(z_n)}=h^2\beta_2+O(h/n).
$$

Both discretization errors are $o(h^2)$ under $nh^2\to\infty$. The preceding [Taylor expansion](../../../calculus.md#taylor-expansion) therefore proves the [second-order boundary expansion for local constant regression](../../../nonparametric-statistics.md#second-order-boundary-expansion-for-local-constant-regression):

$$
\boxed{\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(z_n)+\frac12h^2\beta_2m''(z_n)+o(h^2).}
$$

Equivalently, expanding the [derivatives](../../../calculus.md#derivative) about zero gives

$$
\boxed{\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(0)+h^2\left(\alpha\beta_1+\frac12\beta_2\right)m''(0)+o(h^2).}
$$

In general the truncated first moment is nonzero, so the boundary [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) has order $h$, although it can be smaller when $m'(0)=0$ or the omitted part of the [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression) carries no mass.

For [local linear regression](../../../nonparametric-statistics.md#local-linear-regression), the [polynomial reproduction property of local polynomial regression](../../../nonparametric-statistics.md#polynomial-reproduction-property-of-local-polynomial-regression) removes the constant and linear terms exactly. Let $\Delta=A_0A_2-A_1^2$. Its [effective kernel weights](../../../nonparametric-statistics.md#effective-kernel-weight) are

$$
l_i(t)=\frac{K((x_i-t)/h)}{nh}\frac{A_2-A_1(x_i-t)}{\Delta},
$$

so $\sum_i l_i=1$, $\sum_i l_i(x_i-t)=0$, and

$$
\sum_i l_i(x_i-t)^2=\frac{A_2^2-A_1A_3}{\Delta}.
$$

At either an interior or the specified boundary target, $\Delta$ is asymptotic to a positive constant times $h^2$. At the boundary that constant is $\mu_{0,\alpha}\mu_{2,\alpha}-\mu_{1,\alpha}^2>0$, the mass squared times the [variance](../../../variance.md) of the continuous normalized truncated [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression). Moreover $\sum_i|l_i|=O(1)$, as follows by bounding $|A_2-A_1(x_i-t)|=O(h^2)$ in the window. Thus the [Taylor remainder](../../../calculus.md#taylor-remainder) still contributes $o(h^2)$, even though some [effective kernel weights](../../../nonparametric-statistics.md#effective-kernel-weight) may be negative. In particular,

$$
\operatorname{Bias}\{\widehat m_h(z_n;1)\}=\frac12h^2m''(0)\frac{\mu_{2,\alpha}^2-\mu_{1,\alpha}\mu_{3,\alpha}}{\mu_{0,\alpha}\mu_{2,\alpha}-\mu_{1,\alpha}^2}+o(h^2).
$$

At an interior point this coefficient reduces to $\mu_2(K)$ by symmetry and normalization. Hence **local linear regression has bias $O(h^2)$ at both interior and boundary points**; its linear reproduction removes the generic order-$h$ boundary term.

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A nondegenerate [distribution function](../../../probability-theory.md#cumulative-distribution-function) $G$ is a [max-stable distribution](../../../probability-theory.md#max-stable-distribution) if, for every integer $r\geq1$, there are $a_r>0$ and $b_r\in\mathbb R$ such that

$$
G(a_rx+b_r)^r=G(x)\qquad(x\in\mathbb R).
$$

Equivalently, the suitably centered and positively scaled [sample maximum](../../../probability-theory.md#sample-maximum) of $r$ [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with law $G$ again has law $G$. The [extremal types theorem](../../../probability-theory.md#extremal-types-theorem) states that every nondegenerate limiting law of normalized [sample maxima](../../../probability-theory.md#sample-maximum) is a [max-stable distribution](../../../probability-theory.md#max-stable-distribution). Thus this property identifies all possible limiting types, although a particular starting [distribution function](../../../probability-theory.md#cumulative-distribution-function) need not admit any such limiting normalization.

The three standard types are the [Gumbel distribution](../../../probability-theory.md#gumbel-distribution)

$$
\Lambda(x)=\exp(-e^{-x}),\qquad x\in\mathbb R,
$$

the [Fréchet distribution](../../../probability-theory.md#frechet-distribution), with $\alpha>0$,

$$
\Phi_\alpha(x)=\begin{cases}0,&x\leq0,\\ \exp(-x^{-\alpha}),&x>0,\end{cases}
$$

and the [negative Weibull distribution](../../../probability-theory.md#negative-weibull-distribution), with $\alpha>0$,

$$
\Psi_\alpha(x)=\begin{cases}\exp(-(-x)^\alpha),&x<0,\\1,&x\geq0.\end{cases}
$$

They are [max-stable distributions](../../../probability-theory.md#max-stable-distribution), as follows respectively by taking $(a_r,b_r)=(1,\log r)$, $(r^{1/\alpha},0)$, and $(r^{-1/\alpha},0)$. The necessary and sufficient classification is: **$G$ is max-stable exactly when $G(x)=H((x-b)/a)$ for $a>0$, $b\in\mathbb R$, and one of these three types $H$**. A positive [affine map](../../../geometry-and-topology.md#affine-map) sends a [max-stable distribution](../../../probability-theory.md#max-stable-distribution) to another [max-stable distribution](../../../probability-theory.md#max-stable-distribution).

For the requested threshold equivalence, set $p_n=1-F(u_n)$. By [independence](../../../random-variable.md#independent-random-variables),

$$
\mathbb P(X_{(n)}\leq u_n)=(1-p_n)^n.
$$

If $np_n\to\tau<\infty$, then $p_n\to0$ and the expansion $\log(1-p)=-p+O(p^2)$ gives $n\log(1-p_n)\to-\tau$, since $np_n^2=(np_n)p_n\to0$. Exponentiation proves the claimed limit. Conversely, if $(1-p_n)^n\to e^{-\tau}>0$, then $p_n\to0$: any subsequence with $p_n\geq\delta>0$ would have its powers tending to zero. Taking [logarithms](../../../calculus.md#logarithm) now gives $-n\log(1-p_n)\to\tau$. Since $-\log(1-p)/p\to1$, including the continuous extension at $p=0$, it follows that $np_n\to\tau$. Hence

$$
\boxed{\mathbb P(X_{(n)}\leq u_n)\to e^{-\tau}\ \Longleftrightarrow\ n\{1-F(u_n)\}\to\tau.}
$$

The exceedance count $S_n$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $n,p_n$. For $\tau>0$ and each fixed nonnegative integer $s$, its [probability mass function](../../../probability-theory.md#probability-mass-function) satisfies

$$
\mathbb P(S_n=s)=\frac{(n)_s}{s!}p_n^s(1-p_n)^{n-s}\longrightarrow e^{-\tau}\frac{\tau^s}{s!},
$$

where $(n)_s=n(n-1)\cdots(n-s+1)$ and $(n)_0=1$. Indeed $(n)_s/n^s\to1$, $(np_n)^s\to\tau^s$, and $(1-p_n)^{n-s}\to e^{-\tau}$. If $\tau=0$, the bound $\mathbb P(S_n\geq1)\leq\mathbb ES_n=np_n\to0$ gives the degenerate [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) at zero. Summing the finitely many terms proves, in both cases,

$$
\boxed{\mathbb P(S_n\leq k)\longrightarrow e^{-\tau}\sum_{s=0}^k\frac{\tau^s}{s!},\qquad k=0,1,2,\ldots.}
$$

This derives the needed instance of the [Poisson limit theorem](../../../convergence-of-random-variables.md#poisson-limit-theorem) directly.

Finally fix $x$ with $G(x)>0$ and put $u_n=a_nx+b_n$. The assumed limit for the normalized [sample maximum](../../../probability-theory.md#sample-maximum) and the proved equivalence give $np_n\to-\log G(x)$. The second-largest [order statistic](../../../probability-theory.md#order-statistic) is at most $u_n$ exactly when at most one observation is strictly greater than $u_n$. This event identity holds even if observations have ties. Apply the preceding [Poisson limit theorem](../../../convergence-of-random-variables.md#poisson-limit-theorem) with $k=1$ to obtain

$$
\boxed{\mathbb P\!\left(\frac{W_n-b_n}{a_n}\leq x\right)\longrightarrow G(x)\{1-\log G(x)\}.}
$$

The endpoint $G(x)=1$ corresponds to $\tau=0$ and is already included. This is the case $r=2$ of the [exceedance count limit for extreme order statistics](../../../probability-theory.md#exceedance-count-limit-for-extreme-order-statistics).

## 4

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In [kernel density estimation](../../../nonparametric-statistics.md#kernel-density-estimation), take a [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) $K$ that is nonnegative, symmetric, and has integral one, finite $\mu_2(K)=\int u^2K(u)\,du>0$, and finite $R(K)=\int K(u)^2\,du$. Its [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) $h>0$ gives $K_h(u)=h^{-1}K(u/h)$ and the [kernel density estimator](../../../nonparametric-statistics.md#kernel-density-estimation)

$$
\widehat f_{h,K}(x)=\frac1n\sum_{i=1}^nK_h(x-X_i)
$$

from an [independent and identically distributed](../../../random-variable.md#independent-and-identically-distributed-random-variables) sample with [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $f$. Nonnegativity and unit mass make the estimate itself a [probability density function](../../../continuous-probability-distribution.md#probability-density-function). We compare [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) shapes by their optimized [mean integrated squared error](../../../statistical-modelling.md#integrated-mean-squared-error), rather than by their performance at an arbitrarily common numerical [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth).

For the usual second-order theory, assume, for example, that $f$ belongs to the [Sobolev space](../../../sobolev-space.md) $H^2(\mathbb R)$ and $0<R(f'')<\infty$, and let $h\to0$, $nh\to\infty$. The [expectation](../../../probability-theory.md#expected-value) is the [convolution](../../../fourier-analysis.md#convolution) $K_h*f$. The vanishing first moment of the symmetric [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) and the integral [Taylor remainder](../../../calculus.md#taylor-remainder) give

$$
K_h*f-f=h^2\int_{\mathbb R}u^2K(u)\int_0^1(1-t)f''(\,\cdot-thu)\,dt\,du.
$$

Continuity of translations in the [L2 norm](../../../real-analysis.md#l2-norm), with domination by $u^2K(u)\|f''\|_2$, shows that $h^{-2}(K_h*f-f)\to\mu_2(K)f''/2$ in the [L2 norm](../../../real-analysis.md#l2-norm). Hence the integrated squared [bias of a kernel density estimator](../../../nonparametric-statistics.md#bias-of-a-kernel-density-estimator) is

$$
\|K_h*f-f\|_2^2=\frac14h^4\mu_2(K)^2R(f'')+o(h^4).
$$

By [independence](../../../random-variable.md#independent-random-variables), the exact [integrated variance of a kernel density estimator](../../../nonparametric-statistics.md#integrated-variance-of-a-kernel-density-estimator) is

$$
\int\operatorname{Var}\{\widehat f_{h,K}(x)\}\,dx=\frac1n\left\{\frac{R(K)}h-R(K_h*f)\right\}.
$$

Indeed the integrated second moment of a single summand is $R(K)/h$, and its integrated squared [mean](../../../probability-theory.md#expected-value) is $R(K_h*f)$. The latter quantity is bounded by $R(f)$, by [Young's convolution inequality](../../../fourier-analysis.md#young-s-convolution-inequality), so its contribution is $O(n^{-1})$. The [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error) therefore yields the leading criterion

$$
\operatorname{AMISE}_K(h)=\frac{R(K)}{nh}+\frac14h^4\mu_2(K)^2R(f'').
$$

This [asymptotic mean integrated squared error](../../../statistical-modelling.md#asymptotic-mean-integrated-squared-error) displays the [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff): a small [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) increases integrated [variance](../../../variance.md), while a large one increases squared [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator).

Differentiating the [asymptotic mean integrated squared error](../../../statistical-modelling.md#asymptotic-mean-integrated-squared-error) with respect to $h$ gives $-R(K)/(nh^2)+h^3\mu_2(K)^2R(f'')$. It changes sign once, from negative to positive, so its unique minimum is

$$
\boxed{h_{*,K}=\left\{\frac{R(K)}{n\mu_2(K)^2R(f'')}\right\}^{1/5}.}
$$

At this minimum the integrated [variance](../../../variance.md) term is four times the squared [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) term. Substitution gives

$$
\boxed{\inf_{h>0}\operatorname{AMISE}_K(h)=\frac54C(K)R(f'')^{1/5}n^{-4/5},\qquad C(K)=R(K)^{4/5}\mu_2(K)^{2/5}.}
$$

Thus the leading rate is $n^{-4/5}$, and the shape comparison reduces to minimizing $C(K)$.

There is an essential scale ambiguity: if $K_c(u)=c^{-1}K(u/c)$, then $\widehat f_{h,K_c}=\widehat f_{ch,K}$. Changing the scale of the [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) merely changes the numerical convention for the [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth). Moreover

$$
R(K_c)=c^{-1}R(K),\qquad \mu_2(K_c)=c^2\mu_2(K),\qquad C(K_c)=C(K).
$$

A comparison at the same raw $h$ is therefore not a fair comparison of shape. One can normalize the second moment to one, but that does not make the optimal [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) independent of shape.

The [canonical kernel for density estimation](../../../nonparametric-statistics.md#canonical-kernel-for-density-estimation) instead chooses the unique scale

$$
\boxed{c_K=\left\{\frac{R(K)}{\mu_2(K)^2}\right\}^{1/5},\qquad K^{\mathrm{can}}(u)=c_K^{-1}K(u/c_K).}
$$

It satisfies $R(K^{\mathrm{can}})=\mu_2(K^{\mathrm{can}})^2=C(K)$, and so

$$
\operatorname{AMISE}_{K^{\mathrm{can}}}(h)=C(K)\left\{\frac1{nh}+\frac14h^4R(f'')\right\}.
$$

Consequently **all canonical kernels share the same leading optimal bandwidth $h_*=[nR(f'')]^{-1/5}$**. Only the multiplicative constant $C(K)$ depends on shape. This is precisely the separation of shape choice and scale choice that makes the [canonical kernel](../../../nonparametric-statistics.md#canonical-kernel-for-density-estimation) normalization useful. For an original unscaled [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation), its corresponding optimal [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) is $c_Kh_*$.

To prove optimal shape, scale a candidate [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) to have second moment one. Let $B=\sqrt5$ and

$$
E(u)=\frac{3}{4B^3}(B^2-u^2)_+=\frac3{4\sqrt5}\left(1-\frac{u^2}5\right)_+.
$$

Direct integration gives $\int E=1$, $\int u^2E(u)\,du=B^2/5=1$, and $R(E)=3/(5B)$. Thus $E$ is a rescaled [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel). For any admissible $K$ with the same mass and second moment,

$$
\int_{\mathbb R}(B^2-u^2)(K-E)\,du=0.
$$

Outside $[-B,B]$, $E=0$ and $(B^2-u^2)K\leq0$, because $K\geq0$. The integral inside $[-B,B]$ is therefore nonnegative, and multiplying by $3/(4B^3)$ gives $\int E(K-E)\geq0$. Expanding the square now proves

$$
R(K)-R(E)=\int(K-E)^2+2\int E(K-E)\geq0.
$$

Equality forces $K=E$ almost everywhere. At fixed second moment, minimizing $R(K)$ is equivalent to minimizing $C(K)$. Since $C(K)$ is scale invariant, this proves the [optimality of the Epanechnikov kernel](../../../nonparametric-statistics.md#optimality-of-the-epanechnikov-kernel) over all nonnegative symmetric second-order [kernels for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation), including the equality case up to rescaling.

In its usual scale, the optimal [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel) is

$$
\boxed{K_E(u)=\frac34(1-u^2)\mathbf1_{\{|u|\leq1\}},\qquad \mu_2(K_E)=\frac15,\qquad R(K_E)=\frac35.}
$$

Its canonical scale is $c_E=15^{1/5}$, giving

$$
K_E^{\mathrm{can}}(u)=\frac3{4\,15^{1/5}}\left(1-\frac{u^2}{15^{2/5}}\right)_+.
$$

The optimal [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel) shape is therefore a truncated parabola, rather than a particular support radius. The [canonical kernel](../../../nonparametric-statistics.md#canonical-kernel-for-density-estimation) and unit-second-moment version represent the same shape but different scale conventions.

The numerical gains over other reasonable [kernels for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) are modest. Define [asymptotic relative efficiency](../../../statistical-inference.md#asymptotic-relative-efficiency) against the optimal [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel) by the sample-size fraction giving the same optimized leading [mean integrated squared error](../../../statistical-modelling.md#integrated-mean-squared-error):

$$
\operatorname{Eff}(K)=\left\{\frac{C(K_E)}{C(K)}\right\}^{5/4}=\frac{R(K_E)\sqrt{\mu_2(K_E)}}{R(K)\sqrt{\mu_2(K)}}\leq1.
$$

For the [Gaussian density kernel](../../../nonparametric-statistics.md#gaussian-density-kernel) $K_N(u)=(2\pi)^{-1/2}e^{-u^2/2}$, $R(K_N)=1/(2\sqrt\pi)$ and $\mu_2(K_N)=1$, so its efficiency is $6\sqrt\pi/(5\sqrt5)\simeq0.9512$. For the [uniform smoothing kernel](../../../nonparametric-statistics.md#uniform-smoothing-kernel) $K_U(u)=\tfrac12\mathbf1_{\{|u|\leq1\}}$, $R(K_U)=1/2$ and $\mu_2(K_U)=1/3$, giving efficiency $6\sqrt3/(5\sqrt5)\simeq0.9295$. The [Gaussian density kernel](../../../nonparametric-statistics.md#gaussian-density-kernel) is infinitely smooth, whereas the optimal [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel) has compact support and allows each observation to affect only a finite window. Such computational and smoothness considerations may outweigh a small leading-efficiency difference.

In practice $R(f'')$ is unknown. A [plug-in estimator](../../../statistical-inference.md#plug-in-estimator) estimates this roughness functional from a pilot estimate of the [second derivative](../../../calculus.md#second-derivative) and substitutes it into the optimal [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) formula. Alternatively, [Leave-one-out cross-validation](../../../statistical-learning.md#leave-one-out-cross-validation) minimizes

$$
\operatorname{CV}(h)=\int\widehat f_{h,K}(x)^2\,dx-\frac2n\sum_{i=1}^n\widehat f_{-i,h,K}(X_i),
$$

where $\widehat f_{-i,h,K}$ uses the other $n-1$ observations. By [independence](../../../random-variable.md#independent-random-variables), the [expectation](../../../probability-theory.md#expected-value) of the second term is $2\int(K_h*f)f$, so $\mathbb E\operatorname{CV}(h)=\operatorname{MISE}(h)-R(f)$. Thus it targets integrated error without knowing $f$. The choice of [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth) remains important: even for the optimal [Epanechnikov kernel](../../../nonparametric-statistics.md#epanechnikov-kernel), setting $h=t h_{*,K}$ multiplies the leading minimum error by $(4t^{-1}+t^4)/5$.

The preceding optimum concerns nonnegative second-order [kernels for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) and twice-smooth densities on the real line. Signed [kernels of order ell](../../../nonparametric-statistics.md#kernel-of-order-ell) can cancel higher moments for smoother densities and yield different rates, but may produce negative density estimates. A support boundary or a density jump also requires separate [bias of a kernel density estimator](../../../nonparametric-statistics.md#bias-of-a-kernel-density-estimator) analysis. These settings do not contradict the proved second-order [optimality of the Epanechnikov kernel](../../../nonparametric-statistics.md#optimality-of-the-epanechnikov-kernel).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
