# Paper 42

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper42.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper42.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In a [parametric statistical model](../../../statistical-model.md#parametric-statistical-model) $\{P_\theta:\theta\in\Theta\}$, the [likelihood function](../../../statistical-modelling.md#likelihood-function) $L(\theta;y)$ measures the relative support given by the observed sample for different parameter values. [Maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) supplies a point estimate; the sampling distributions of suitable [statistics](../../../statistical-inference.md#statistic) calibrate significance tests and [confidence intervals](../../../statistical-inference.md#confidence-interval). A [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) retains all parameter-dependent information in the [likelihood function](../../../statistical-modelling.md#likelihood-function), so one first seeks a reduction to such a [statistic](../../../statistical-inference.md#statistic) rather than discarding information arbitrarily.

The characteristic conditioning principle in [Fisherian conditional inference](../../../statistical-inference.md#fisherian-conditional-inference) is to calibrate inference conditional on the observed value of an [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic). With no [nuisance parameter](../../../statistical-model.md#nuisance-parameter), a [statistic](../../../statistical-inference.md#statistic) $A$ is ancillary when its law is the same for every $\theta$. Its observed value can nevertheless describe the experimental configuration or precision. Conditional inference uses $\mathcal L_\theta(T\mid A=a)$ for an informative [statistic](../../../statistical-inference.md#statistic) $T$, with $a$ the observed ancillary value. Since the marginal law of $A$ does not depend on $\theta$, conditioning leaves the parameter-dependent [likelihood](../../../statistical-modelling.md#likelihood-function) factor unchanged, while potentially changing the appropriate repeated-sampling reference distribution. Conditioning on a continuous $A$ means using a [regular conditional distribution](../../../probability-theory.md#regular-conditional-distribution), rather than dividing by $\mathbb P(A=a)$.

With parameters $(\psi,\lambda)$, where $\psi$ is the target and $\lambda$ a [nuisance parameter](../../../statistical-model.md#nuisance-parameter), a fully [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic) has a law independent of both. A [partial ancillary statistic](../../../probability-and-statistics.md#partial-ancillary-statistic) for $\psi$ may have a law depending on $\lambda$ but not on $\psi$. To eliminate $\lambda$ by conditioning, one needs the actual conditional law of the informative [statistic](../../../statistical-inference.md#statistic) to be free of $\lambda$; partial ancillarity by itself does not guarantee this. For example, if independent counts have [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) with means $\lambda\psi$ and $\lambda(1-\psi)$, their total $N$ has [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\lambda$, independent of $\psi$. The first count conditional on $N=m$ has [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $(m,\psi)$. Conditioning removes the nuisance intensity $\lambda$ exactly. More generally, nuisance-free [pivotal quantities](../../../probability-and-statistics.md#pivotal-quantity) or [conditional likelihoods](../../../statistical-modelling.md#conditional-likelihood) can be used where available; there is no universal conditioning device that removes every [nuisance parameter](../../../statistical-model.md#nuisance-parameter).

For a concrete example of [non-uniqueness of maximal ancillary statistics](../../../probability-and-statistics.md#non-uniqueness-of-maximal-ancillary-statistics), consider one observed pair $(U,V)\in\{0,1\}^2$, with

$$
P_\theta(0,0)=P_\theta(1,1)=\frac\theta2,\qquad
P_\theta(0,1)=P_\theta(1,0)=\frac{1-\theta}{2},\qquad0<\theta<1.
$$

Both $U$ and $V$ have [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with success probability $1/2$, independent of $\theta$, so each is an [ancillary statistic](../../../probability-and-statistics.md#ancillary-statistic). Their generated partitions are different and incomparable. Moreover, each is maximal: refining either two-point cell singles out a point whose probability is $\theta/2$ or $(1-\theta)/2$, which is parameter-dependent. Their joint [statistic](../../../statistical-inference.md#statistic) is not ancillary, since $P_\theta(U=V)=\theta$. Thus there is no common finer ancillary partition that reconciles the two choices. The conditional laws differ as labelled experiments: $P_\theta(V=U\mid U)=\theta$ and $P_\theta(U=V\mid V)=\theta$, but they condition on different observed information. This illustrates why “condition on a maximal ancillary” need not specify a unique procedure.

For the [location-scale family](../../../statistical-model.md#location-scale-family), write $Y_i=\mu+\sigma Z_i$, where the $Z_i$ are independent with the fixed density $f_0$. Let $s_Z^2=n^{-1}\sum_i(Z_i-\bar Z)^2$. The transformation gives

$$
\widehat\mu=\bar Y=\mu+\sigma\bar Z,\qquad
\widehat\sigma=\sigma s_Z,
$$

and therefore

$$
\boxed{A_i=\frac{Y_i-\widehat\mu}{\widehat\sigma}
=\frac{Z_i-\bar Z}{s_Z}.}
$$

For $n\geq2$, $s_Z>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), because an independent sample from a density has probability zero of all observations coinciding. The right side depends only on a sample from the fixed base law, so the entire vector $A$ has a law independent of $(\mu,\sigma)$: $\boxed{A\text{ is ancillary}.}$ No finite population mean or [variance](../../../variance.md) is needed for this algebraic argument. With one observation the displayed standardization is undefined, so at least two observations are implicitly required.

The pair $(\widehat\mu,\widehat\sigma)$ together with $A$ reconstructs the full sample through $Y_i=\widehat\mu+\widehat\sigma A_i$. Thus [conditional inference in a location-scale family](../../../statistical-model.md#conditional-inference-in-a-location-scale-family) uses

$$
\boxed{\mathcal L_{\mu,\sigma}(\widehat\mu,\widehat\sigma\mid A=a),}
$$

where $a$ is the observed residual configuration. Equivalently one can use the parameter-free conditional law of $((\widehat\mu-\mu)/\sigma,\widehat\sigma/\sigma)$ given $A=a$. To see this explicitly, the centered residual subspace has dimension $n-1$, so its radial coordinate $t=\widehat\sigma$ contributes a [Jacobian determinant](../../../calculus.md#jacobian-determinant) factor proportional to $t^{n-2}$. The [conditional density](../../../probability-theory.md#conditional-density) of $\widehat\mu=m$, $\widehat\sigma=t>0$ is therefore proportional to

$$
t^{n-2}\sigma^{-n}\prod_{i=1}^nf_0\!\left(\frac{m+ta_i-\mu}{\sigma}\right).
$$

Setting $u=(m-\mu)/\sigma$ and $v=t/\sigma$ gives a [conditional density](../../../probability-theory.md#conditional-density) proportional to $v^{n-2}\prod_i f_0(u+va_i)$, with no unknown parameter. The normalizing factor can depend on $a$, but not on $\mu$ or $\sigma$. These statements concern almost every attainable ancillary value.

## 2

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $M_n=\max_{1\leq j\leq n}W_j$ for [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with [distribution function](../../../probability-theory.md#cumulative-distribution-function) $F$. Then $P(M_n\leq u)=F(u)^n$. Membership in the [maximum domain of attraction](../../../probability-theory.md#maximum-domain-of-attraction) of a nondegenerate [distribution function](../../../probability-theory.md#cumulative-distribution-function) $G$ means that some deterministic $a_n>0$ and $b_n\in\mathbb R$ satisfy

$$
\boxed{\frac{M_n-b_n}{a_n}\xrightarrow{d}Z,\qquad P(Z\leq x)=G(x),}
$$

or equivalently $F(a_nx+b_n)^n\to G(x)$ at every continuity point of $G$.

Under the stated convergence, put $Z_n=(M_n-b_n)/a_n$, $r_n=\alpha_n/a_n\to a>0$, and $s_n=(\beta_n-b_n)/a_n\to b$. The [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) says that combining a sequence with [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) with sequences converging in [probability](../../../probability-theory.md#probability) to constants preserves the corresponding sum, product and ratio limits, provided a limiting denominator is nonzero. Applying it here gives

$$
\frac{M_n-\beta_n}{\alpha_n}=\frac{Z_n-s_n}{r_n}\xrightarrow{d}\frac{Z-b}{a}.
$$

The limiting [distribution function](../../../probability-theory.md#cumulative-distribution-function) is $P((Z-b)/a\leq x)=G(ax+b)$, continuous for every real $x$ because $G$ is continuous and $a>0$. Consequently,

$$
\boxed{F(\alpha_nx+\beta_n)^n\longrightarrow G(ax+b)\quad\text{for every real }x.}
$$

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For large $t$, write the [survival function](../../../survival-analysis.md#survival-function) as

$$
\overline F(t)=t^{-2}\ell(t),\qquad \ell(t)=\frac{C}{\log t\,\log\log t}.
$$

A positive [function](../../../function.md) $\ell$ is [slowly varying](../../../real-analysis.md#slowly-varying-function) if $\ell(tu)/\ell(t)\to1$ for every fixed $u>0$. Here

$$
\frac{\ell(tu)}{\ell(t)}
=\frac{\log t\,\log\log t}{\log(tu)\,\log\log(tu)}\longrightarrow1,
$$

since $\log(tu)=\log t+\log u$ and $\log\log(tu)-\log\log t\to0$. Thus $\overline F$ has [regular variation](../../../real-analysis.md#regular-variation) of index $-2$.

The relevant extreme-value criterion is that an infinite right endpoint and a [survival function](../../../survival-analysis.md#survival-function) regularly varying with index $-r$, $r>0$, give attraction to the standard [Fréchet distribution](../../../probability-theory.md#frechet-distribution) of shape $r$. Its [distribution function](../../../probability-theory.md#cumulative-distribution-function) is $G_r(x)=e^{-x^{-r}}$ for $x>0$ and zero for $x\leq0$. Here is a direct verification, so no additional theorem is needed to establish the criterion in this example. Choose $a_n\to\infty$ satisfying $n\overline F(a_n)\to1$ and set $b_n=0$. For $x>0$,

$$
n\overline F(a_nx)
=n\overline F(a_n)\frac{\overline F(a_nx)}{\overline F(a_n)}\longrightarrow x^{-2}.
$$

If $u_n\to0$ and $nu_n\to c$, then $n\log(1-u_n)=-nu_n+O(nu_n^2)\to-c$. Applying this with $u_n=\overline F(a_nx)$ gives $F(a_nx)^n\to e^{-x^{-2}}$. For $x\leq0$, the [distribution function](../../../probability-theory.md#cumulative-distribution-function) is zero because the observations are supported on $[10,\infty)$. Therefore

$$
\boxed{G(x)=\begin{cases}e^{-x^{-2}},&x>0,\\0,&x\leq0,\end{cases}\qquad F\in D(G).}
$$

For example, elementary asymptotic normalizers are

$$
a_n=\left(\frac{2Cn}{\log n\,\log\log n}\right)^{1/2},\qquad b_n=0,
$$

for sufficiently large $n$, with arbitrary positive definitions at smaller indices. Indeed $\log a_n\sim\tfrac12\log n$ and $\log\log a_n\sim\log\log n$, so $a_n^2\log a_n\log\log a_n\sim Cn$. The precise valid choice of $C$ at the lower endpoint does not change the limiting shape.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Gumbel distribution](../../../probability-theory.md#gumbel-distribution) for maxima has [distribution function](../../../probability-theory.md#cumulative-distribution-function) $G(x)=\exp(-e^{-x})$ on the whole real line. For $n\geq2$ set

$$
\boxed{\beta_n=(\log n)^2,\qquad \alpha_n=2\log n.}
$$

Both the centering and scale are elementary, and the scale is positive. For any fixed real $x$, the normalized threshold $\beta_n+\alpha_nx$ is positive for all sufficiently large $n$. Writing $L=\log n$, a [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
\sqrt{\beta_n+\alpha_nx}
=L\sqrt{1+\frac{2x}{L}}
=L+x+O(L^{-1}).
$$

Consequently,

$$
n\overline F(\beta_n+\alpha_nx)
=n\exp\!\left(-\sqrt{\beta_n+\alpha_nx}\right)
\longrightarrow e^{-x}.
$$

The logarithm calculation in part (i) now gives

$$
\boxed{F(\alpha_nx+\beta_n)^n\longrightarrow\exp(-e^{-x})\quad(x\in\mathbb R).}
$$

Thus $F$ belongs to the [maximum domain of attraction](../../../probability-theory.md#maximum-domain-of-attraction) of the standard [Gumbel distribution](../../../probability-theory.md#gumbel-distribution). The scale also has the [Gumbel auxiliary function](../../../probability-theory.md#gumbel-auxiliary-function) interpretation: the reciprocal [hazard function](../../../survival-analysis.md#hazard-function) is $2\sqrt t$, whose [derivative](../../../calculus.md#derivative) $1/\sqrt t$ tends to zero at the infinite right endpoint. This agrees with the [Von Mises conditions for extreme values](../../../probability-theory.md#von-mises-conditions-for-extreme-values), and at $t=\beta_n$ gives exactly $\alpha_n=2\log n$.

## 3

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Iterating the recurrence yields

$$
\boxed{X_j=\rho^{j-1}Y_1+\sqrt{1-\rho^2}\sum_{k=2}^j\rho^{j-k}Y_k.}
$$

Thus every finite collection of the $X_j$ is a [linear transformation](../../../vector-space.md#linear-map) of independent [standard normal random variables](../../../probability-theory.md#standard-normal-random-variable), and has a [multivariate Gaussian distribution](../../../probability-theory.md#multivariate-gaussian-distribution). The [expected values](../../../probability-theory.md#expected-value) are zero. Independence of the $Y_k$ gives

$$
\operatorname{Var}(X_j)=\rho^{2(j-1)}+(1-\rho^2)\sum_{l=0}^{j-2}\rho^{2l}=1.
$$

For $i<j$, the recurrence writes $X_j=\rho^{j-i}X_i$ plus a sum of future innovations independent of $X_i$. Hence $\operatorname{Cov}(X_i,X_j)=\rho^{j-i}$. The required vector law is

$$
\boxed{(X_1,\ldots,X_n)^T\sim N_n(0,R_n),\qquad (R_n)_{ij}=\rho^{|i-j|}.}
$$

The [covariance matrix](../../../variance.md#covariance-matrix) is positive definite: the lower-triangular transformation from $(Y_1,\ldots,Y_n)$ has nonzero diagonal entries $1,\sqrt{1-\rho^2},\ldots,\sqrt{1-\rho^2}$. This also identifies a stationary [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one), with marginal density $f=\phi$.

With the [standard normal density](../../../probability-theory.md#standard-normal-density) as the [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation), the two [characteristic functions](../../../probability-theory.md#characteristic-function) are $\psi(t)=e^{-t^2/2}$ and $\psi_K(ht)=e^{-h^2t^2/2}$. The [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) $X_1-X_{j+1}$ has mean zero and [variance](../../../variance.md) $2(1-\rho^j)$, so

$$
\mathbb E e^{it(X_1-X_{j+1})}=e^{-(1-\rho^j)t^2}.
$$

This expression is real. Substitution in the given integrated covariance expression, followed by the [Gaussian integral](../../../calculus.md#gaussian-integral) $\int_{\mathbb R}e^{-at^2}\,dt=\sqrt{\pi/a}$ for $a>0$, gives

$$
\begin{aligned}
g(j)&=\int_{\mathbb R}\left[e^{-(1+h^2-\rho^j)t^2}-e^{-(1+h^2)t^2}\right]dt\\
&=\boxed{\sqrt\pi\left[\frac1{\sqrt{1+h^2-\rho^j}}-\frac1{\sqrt{1+h^2}}\right].}
\end{aligned}
$$

To bound the total [Gaussian autoregressive kernel variance correction](../../../nonparametric-statistics.md#gaussian-autoregressive-kernel-variance-correction), apply the [mean value theorem](../../../calculus.md#mean-value-theorem) to $u\mapsto u^{-1/2}$. For $j\geq1$, the whole interval between $1+h^2-\rho^j$ and $1+h^2$ is bounded below by $1-\rho>0$. Therefore

$$
0\leq g(j)\leq\frac{\sqrt\pi\,\rho^j}{2(1-\rho)^{3/2}}.
$$

Summing the [geometric series](../../../real-analysis.md#geometric-series) gives the uniform bound

$$
0\leq\sum_{j=1}^{n-1}\left(1-\frac jn\right)g(j)
\leq\frac{\sqrt\pi}{2(1-\rho)^{3/2}}\frac\rho{1-\rho}.
$$

It follows from the supplied [variance](../../../variance.md) identity that

$$
\boxed{\int\operatorname{Var}(\widehat f_h(x))\,dx
=\int\operatorname{Var}(\widehat f_h^*(x))\,dx+O(n^{-1}).}
$$

The constant depends on the fixed $\rho$, but not on $h$ or $n$. In particular this applies to the requested shrinking-bandwidth regime; the covariance bound itself does not need $nh\to\infty$.

All observations have the same marginal density $f$, so dependence changes the [variance](../../../variance.md) but not the [bias of a kernel density estimator](../../../nonparametric-statistics.md#bias-of-a-kernel-density-estimator): $\mathbb E\widehat f_h=K_h*f$. Write $R(q)=\int_{\mathbb R}q^2$ and $\mu_2(K)=\int u^2K(u)\,du$. For a smooth density with $f''\in L^2$, the [integrated variance of a kernel density estimator](../../../nonparametric-statistics.md#integrated-variance-of-a-kernel-density-estimator) in the independent case is $R(K)/(nh)+O(n^{-1})$. A second-order [Taylor expansion](../../../calculus.md#taylor-expansion) of the [convolution](../../../fourier-analysis.md#convolution) gives $K_h*f-f=(h^2\mu_2(K)/2)f''+o(h^2)$ in the [L2 norm](../../../real-analysis.md#l2-norm). Thus the [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error) gives

$$
\operatorname{MISE}(h)=\frac{R(K)}{nh}+\frac{\mu_2(K)^2R(f'')}{4}h^4+o(h^4)+O(n^{-1}).
$$

The first two terms are the [asymptotic mean integrated squared error](../../../statistical-modelling.md#asymptotic-mean-integrated-squared-error). The additional dependence term is smaller than $n^{-4/5}$, so the leading optimal bandwidth and optimal rate are the same as for independent data:

$$
\boxed{h_{\mathrm{AMISE}}=\left[\frac{R(K)}{n\mu_2(K)^2R(f'')}\right]^{1/5},\qquad
\operatorname{MISE}(h_{\mathrm{AMISE}})\asymp n^{-4/5}.}
$$

Here both $K$ and $f$ are the [standard normal density](../../../probability-theory.md#standard-normal-density). Since $f''(x)=(x^2-1)\phi(x)$, direct [Gaussian integrals](../../../calculus.md#gaussian-integral) give

$$
R(K)=\frac1{2\sqrt\pi},\qquad \mu_2(K)=1,\qquad
R(f'')=\frac1{2\pi}\int(x^2-1)^2e^{-x^2}\,dx=\frac3{8\sqrt\pi}.
$$

Consequently the explicit leading bandwidth is

$$
\boxed{h_{\mathrm{AMISE}}=\left(\frac4{3n}\right)^{1/5},\qquad
\operatorname{MISE}(h_{\mathrm{AMISE}})\sim\frac5{8\sqrt\pi}\left(\frac34\right)^{1/5}n^{-4/5}.}
$$

At this bandwidth the leading integrated [variance](../../../variance.md) is four times the leading integrated squared bias, which is also a check on the minimization constant.

## 4

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let the summands be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with mean $\mu$, [variance](../../../variance.md) $\sigma^2>0$, and standardized third [cumulant](../../../probability-theory.md#cumulant) $\gamma_1=\mathbb E[(Y_1-\mu)^3]/\sigma^3$. Define

$$
S_n^*=\frac{\sum_{i=1}^n(Y_i-\mu)}{\sigma\sqrt n}.
$$

An [Edgeworth expansion](../../../probability-theory.md#edgeworth-series) refines the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) using the higher [cumulants](../../../probability-theory.md#cumulant) of one summand. Some smoothness and moment assumptions are essential: finite [variance](../../../variance.md) alone does not supply a density expansion. A convenient sufficient set for the expansions here is a smooth density whose [derivatives](../../../calculus.md#derivative) decay faster than every inverse power, together with $\mathbb E e^{\delta|Y_1|}<\infty$ for some $\delta>0$. These assumptions give all required moments, Fourier smoothing and the nonlattice characteristic-function condition. Less restrictive sufficient conditions are possible, but this set covers the logistic model below.

Write $\phi$ and $\Phi$ for the [standard normal density](../../../probability-theory.md#standard-normal-density) and [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). The first-order density [Edgeworth expansion](../../../probability-theory.md#edgeworth-series) is

$$
\boxed{p_{S_n^*}(x)=\phi(x)\left[1+\frac{\gamma_1}{6\sqrt n}(x^3-3x)\right]+O(n^{-1}).}
$$

The remainder is uniform on every fixed compact interval under the stated assumptions. To see the origin of the correction, for $Z=(Y_1-\mu)/\sigma$ the [cumulant expansion](../../../probability-theory.md#cumulant-expansion) of its [characteristic function](../../../probability-theory.md#characteristic-function) gives

$$
n\log\mathbb E e^{itZ/\sqrt n}
=-\frac{t^2}{2}+\frac{\gamma_1(it)^3}{6\sqrt n}+O(n^{-1}).
$$

Exponentiating and using [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) yields the displayed correction, since the inverse transform of $(it)^3e^{-t^2/2}$ is $-\phi^{(3)}(x)=(x^3-3x)\phi(x)$. The [Probabilists' Hermite polynomial](../../../numerical-analysis.md#probabilists-hermite-polynomial) convention is being used: $H_2(x)=x^2-1$ and $H_3(x)=x^3-3x$.

The corresponding [distribution function](../../../probability-theory.md#cumulative-distribution-function) expansion is

$$
\boxed{F_{S_n^*}(x)=\Phi(x)-\frac{\gamma_1}{6\sqrt n}(x^2-1)\phi(x)+O(n^{-1}),}
$$

uniformly on fixed compact intervals. The sign follows from $\frac{d}{dx}[H_2(x)\phi(x)]=-H_3(x)\phi(x)$. These are expansions of both the density and [distribution function](../../../probability-theory.md#cumulative-distribution-function); a uniform density error alone would not justify integrating an error bound over the entire real line without the accompanying tail control.

For a fixed $\alpha\in(0,1)$, write $z=z_\alpha=\Phi^{-1}(\alpha)$. At leading order the proposed [quantile](../../../probability-theory.md#quantile-function) expansion gives $\Phi(p_0(z))=\Phi(z)$, and strict monotonicity gives $p_0(z)=z$. Substitute $y_\alpha=z+p_1(z)n^{-1/2}+O(n^{-1})$ into the [distribution function](../../../probability-theory.md#cumulative-distribution-function) expansion. A [Taylor expansion](../../../calculus.md#taylor-expansion) at $z$ gives

$$
F_{S_n^*}(y_\alpha)
=\alpha+\frac{\phi(z)}{\sqrt n}\left[p_1(z)-\frac{\gamma_1}{6}(z^2-1)\right]+O(n^{-1}).
$$

Since $\phi(z)>0$, the coefficient of $n^{-1/2}$ must vanish. Thus the first [Cornish-Fisher expansion](../../../probability-theory.md#cornish-fisher-expansion) coefficients are

$$
\boxed{p_0(z)=z,\qquad p_1(z)=\frac{\gamma_1}{6}(z^2-1).}
$$

For the [logistic distribution](../../../statistical-modelling.md#logistic-distribution), set $Z_i=Y_i-\theta$. Its density $q(z)=e^z/(1+e^z)^2$ satisfies $q(-z)=q(z)$ and has exponentially decreasing tails. Symmetry and integrability give $\mathbb E Z_i=0$, and the supplied integral gives

$$
\mathbb E Z_i^2=2\int_0^\infty\frac{z^2e^z}{(1+e^z)^2}\,dz=\frac{\pi^2}{3}.
$$

Therefore $\mathbb E Y_i=\theta$, $\operatorname{Var}(Y_i)=\pi^2/3$, and the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives

$$
T_n=\frac{\sqrt n(\bar Y-\theta)}{\pi/\sqrt3}\xrightarrow{d}N(0,1).
$$

Writing $z_-=z_{\alpha/2}$ and $z_+=z_{1-\alpha/2}$, the condition $z_-\leq T_n\leq z_+$ is equivalent to

$$
\bar Y-\frac{\pi}{\sqrt{3n}}z_+\leq\theta\leq
\bar Y-\frac{\pi}{\sqrt{3n}}z_-.
$$

Consequently the [confidence interval](../../../statistical-inference.md#confidence-interval)

$$
\boxed{\left(\bar Y-\frac{\pi}{\sqrt{3n}}z_{1-\alpha/2},\quad
\bar Y-\frac{\pi}{\sqrt{3n}}z_{\alpha/2}\right)}
$$

has limiting coverage $\Phi(z_+)-\Phi(z_-)=1-\alpha$. Whether the finite endpoints are included makes no probability difference because the sample mean has a density.

The centered [logistic distribution](../../../statistical-modelling.md#logistic-distribution) is symmetric, so $\gamma_1=0$. Its smooth density and exponentially decreasing [derivatives](../../../calculus.md#derivative) satisfy the conditions stated above; in particular all moments exist and Fourier smoothing is available. The first correction in the [Edgeworth expansion](../../../probability-theory.md#edgeworth-series) vanishes, leaving $F_{T_n}(z)=\Phi(z)+O(n^{-1})$ at each of the two fixed [quantiles](../../../probability-theory.md#quantile-function). Subtracting gives the stronger conclusion

$$
\boxed{P_\theta(\theta\text{ lies in the interval})=1-\alpha+O(n^{-1}).}
$$

The standardized law is independent of $\theta$, so this coverage-error conclusion holds with the same bound for every location parameter.

## 5

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

An [exponential dispersion family of order one](../../../exponential-family.md#exponential-dispersion-family-of-order-one) has density or mass function, relative to a fixed dominating measure, of the form

$$
p(y;\theta,\phi)=\exp\!\left\{\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)\right\},
$$

where $\theta$ is a scalar [natural parameter](../../../exponential-family.md#natural-parameter-of-an-exponential-family), $\phi>0$ is the [dispersion parameter](../../../exponential-family.md#dispersion-parameter), and the support does not depend on $\theta$. For regular families, $b$ is twice differentiable on an open natural-parameter domain and $b''>0$. Known observation weights $w$ replace $\phi$ by $\phi/w$. “Order one” refers to the scalar canonical [statistic](../../../statistical-inference.md#statistic) $y$, rather than an arbitrary vector of canonical [statistics](../../../statistical-inference.md#statistic).

Differentiate the normalization $\int p(y;\theta,\phi)\,dy=1$, or its discrete counterpart, assuming differentiation under the integral is valid. The first [derivative](../../../calculus.md#derivative) gives $\mathbb E(Y-b'(\theta))=0$. The second [derivative](../../../calculus.md#derivative) gives

$$
0=\mathbb E\!\left[\frac{(Y-b'(\theta))^2}{\phi^2}-\frac{b''(\theta)}\phi\right].
$$

Consequently,

$$
\boxed{\mu=\mathbb E Y=b'(\theta),\qquad \operatorname{Var}(Y)=\phi b''(\theta).}
$$

The [variance function](../../../exponential-family.md#variance-function) expresses the second [derivative](../../../calculus.md#derivative) in terms of the mean:

$$
\boxed{V(\mu)=b''((b')^{-1}(\mu)),\qquad \operatorname{Var}(Y)=\phi V(\mu)/w.}
$$

A [generalized linear model](../../../statistical-modelling.md#generalized-linear-model) specifies independent responses from an [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model), a [linear predictor](../../../statistical-modelling.md#linear-predictor) $\eta_i=x_i^T\beta$, and a differentiable monotone [link function](../../../statistical-modelling.md#link-function) relating it to the response mean by $g(\mu_i)=\eta_i$. The family, [variance function](../../../exponential-family.md#variance-function), covariate design, [link function](../../../statistical-modelling.md#link-function) and dispersion specification together define the model. The [canonical link function](../../../statistical-modelling.md#canonical-link-function) identifies the [linear predictor](../../../statistical-modelling.md#linear-predictor) with the [natural parameter](../../../exponential-family.md#natural-parameter-of-an-exponential-family):

$$
\boxed{g(\mu)=(b')^{-1}(\mu),\qquad\theta_i=x_i^T\beta.}
$$

One advantage is that the [likelihood](../../../statistical-modelling.md#likelihood-function) equations become particularly simple. With known weights $w_i$ and common dispersion $\phi$, the [score function](../../../statistical-modelling.md#informant-function) and negative [Hessian matrix](../../../calculus.md#hessian-matrix) for $\beta$ are

$$
U_\beta=\frac1\phi\sum_i w_ix_i(Y_i-\mu_i),\qquad
-\ell_{\beta\beta}=\frac1\phi\sum_iw_iV(\mu_i)x_ix_i^T.
$$

The latter does not explicitly depend on the responses, so it equals the expected [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) at the same parameter. With full-rank design and positive [variances](../../../variance.md) the [likelihood](../../../statistical-modelling.md#likelihood-function) is strictly concave in $\beta$, simplifying optimization. These statements concern the coefficient block at a fixed dispersion value.

Three explicit examples, taking unit weights, are as follows.

For a [normal distribution](../../../probability-theory.md#normal-distribution) with mean $\mu$ and [variance](../../../variance.md) $\phi$,

$$
\log p(y)=\frac{y\mu-\mu^2/2}{\phi}-\frac{y^2}{2\phi}-\frac12\log(2\pi\phi).
$$

Thus $\theta=\mu$, $b(\theta)=\theta^2/2$, $c(y,\phi)=-y^2/(2\phi)-\tfrac12\log(2\pi\phi)$, and $V(\mu)=1$. Its [canonical link function](../../../statistical-modelling.md#canonical-link-function) is $\boxed{g(\mu)=\mu}$, the [identity link](../../../statistical-modelling.md#identity-link).

For a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\mu>0$ and support $\{0,1,\ldots\}$,

$$
\log p(y)=y\log\mu-\mu-\log(y!).
$$

Here $\phi=1$, $\theta=\log\mu$, $b(\theta)=e^\theta$, and $c(y,1)=-\log(y!)$. Therefore $b'(\theta)=b''(\theta)=e^\theta$, $V(\mu)=\mu$, and the [Poisson canonical link](../../../statistical-modelling.md#poisson-canonical-link) is $\boxed{g(\mu)=\log\mu}$.

For a [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with success probability $\mu\in(0,1)$,

$$
\log p(y)=y\log\frac\mu{1-\mu}+\log(1-\mu),\qquad y\in\{0,1\}.
$$

Taking $\phi=1$, $\theta=\log(\mu/(1-\mu))$, $b(\theta)=\log(1+e^\theta)$, and $c(y,1)=0$ gives the required form. Its mean and [variance function](../../../exponential-family.md#variance-function) are $b'(\theta)=e^\theta/(1+e^\theta)=\mu$ and $V(\mu)=\mu(1-\mu)$. Its [canonical link function](../../../statistical-modelling.md#canonical-link-function) is $\boxed{g(\mu)=\log(\mu/(1-\mu))}$, the [logit link](../../../statistical-modelling.md#logit). The fixed dispersion values in the Poisson and Bernoulli cases are part of those models; an arbitrary continuous dispersion is not being asserted for them.

To test $H_0:\beta_j=0$, first fit the unrestricted model and then the restricted model with that component fixed at zero, estimating all [nuisance parameters](../../../statistical-model.md#nuisance-parameter), including dispersion when applicable, in each fit. If $\widehat\vartheta$ and $\widetilde\vartheta$ denote their full fitted parameter vectors, the [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) uses

$$
\boxed{D=2\{\ell(\widehat\vartheta)-\ell(\widetilde\vartheta)\}.}
$$

For identifiable regular models, an interior null parameter and a fixed-dimensional full-rank design with increasing information, the [Wilks theorem](../../../statistical-inference.md#wilks-theorem) gives $D\xrightarrow{d}\chi_1^2$ under $H_0$. A level-$\alpha$ test rejects for $D$ greater than the $(1-\alpha)$-[quantile](../../../probability-theory.md#quantile-function) of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with one [degree of freedom](../../../classical-mechanics.md#degree-of-freedom).

Alternatively the [Wald test](../../../statistical-modelling.md#wald-test) uses $W=\widehat\beta_j^2/\widehat{\operatorname{Var}}(\widehat\beta_j)$, with the [variance](../../../variance.md) obtained from the appropriate inverse full [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix); it has the same limiting $\chi_1^2$ null law. The [score test](../../../statistical-modelling.md#score-test) fits only the restricted model. If $\lambda$ collects its [nuisance parameters](../../../statistical-model.md#nuisance-parameter), its efficient information is $I_{jj\cdot\lambda}=I_{jj}-I_{j\lambda}I_{\lambda\lambda}^{-1}I_{\lambda j}$, and the [statistic](../../../statistical-inference.md#statistic) is $U_j(\widetilde\vartheta)^2/I_{jj\cdot\lambda}(\widetilde\vartheta)$, again asymptotically $\chi_1^2$. Accounting for the nuisance block is necessary rather than using the unadjusted diagonal information.

## 6

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For ordinary homoscedastic [fixed-design nonparametric regression](../../../nonparametric-statistics.md#fixed-design-nonparametric-regression), take observations $Y_i=g(x_i)+\epsilon_i$ at known distinct sites, with independent mean-zero errors of common [variance](../../../variance.md). A degree-$p$ [local polynomial estimator](../../../nonparametric-statistics.md#local-polynomial-regression) at a target $u$ solves the finite-dimensional [weighted least squares](../../../statistical-modelling.md#weighted-least-squares) problem

$$
\widehat\beta(u)=\operatorname*{argmin}_{\beta\in\mathbb R^{p+1}}
\sum_i K\!\left(\frac{x_i-u}{h}\right)
\left[Y_i-\sum_{r=0}^p\beta_r(x_i-u)^r\right]^2.
$$

Here $K$ is a nonnegative [regression kernel](../../../nonparametric-statistics.md#kernel-for-nonparametric-regression), $h>0$ is the [smoothing bandwidth](../../../nonparametric-statistics.md#smoothing-bandwidth), and sufficient local design rank ensures uniqueness. The estimate of the [regression function](../../../statistical-learning.md#regression-function) is $\widehat g(u)=\widehat\beta_0(u)$. Each target has its own locally fitted [polynomial](../../../polynomial.md); this is not one global [polynomial](../../../polynomial.md) fit. The bandwidth controls the localization and the [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff).

A [natural cubic smoothing spline](../../../nonparametric-statistics.md#cubic-smoothing-spline) instead solves the global penalized problem

$$
\widehat g_\lambda=\operatorname*{argmin}_{v\in H^2[a,b]}
\left\{\sum_i[Y_i-v(x_i)]^2+\lambda\int_a^b[v''(x)]^2\,dx\right\},\qquad\lambda>0.
$$

The [Sobolev space](../../../sobolev-space.md) here consists of functions with square-integrable weak [derivatives](../../../calculus.md#derivative) through order two. The minimizer is a [natural cubic spline](../../../uniform-approximation.md#natural-cubic-spline) with knots at the observation sites and linear tails outside the extreme sites. Equivalently one may perform the minimization on that finite-dimensional spline space: the [minimum roughness property of the natural cubic spline interpolant](../../../uniform-approximation.md#minimum-roughness-property-of-the-natural-cubic-spline-interpolant) shows that replacing a candidate by the natural spline with the same site values preserves the data loss and decreases the second-[derivative](../../../calculus.md#derivative) penalty. The [smoothing parameter](../../../nonparametric-statistics.md#smoothing-parameter) $\lambda$ controls curvature; it differs from the local bandwidth $h$.

For the interval-average observation problem, the printed upper limit in the loss is an indexing error: there are only $n-1$ responses and intervals, so a term with $i=n$ would involve the undefined $Y_n$ and $x_{n+1}$. The coherent loss uses the upper limit $n-1$. Put $\Delta_i=x_{i+1}-x_i$ and define the linear observation functionals

$$
L_iv=\frac1{\Delta_i}\int_{x_i}^{x_{i+1}}v(x)\,dx,\qquad1\leq i\leq n-1.
$$

The intended criterion on $C^1[a,b]$ is therefore

$$
S_\lambda(v)=\sum_{i=1}^{n-1}(Y_i-L_iv)^2+\lambda\int_a^b[v'(x)]^2\,dx.
$$

Unlike the ordinary [cubic smoothing spline](../../../nonparametric-statistics.md#cubic-smoothing-spline), this uses interval averages as data and a first-[derivative](../../../calculus.md#derivative) penalty; the resulting spline degree will be two.

Fix any candidate $v\in C^1[a,b]$. By the supplied interpolation property, there is a unique [quadratic spline](../../../uniform-approximation.md#quadratic-spline) $q\in C^1[a,b]$ with knots $x_1,\ldots,x_n$, constant on both exterior intervals, such that $L_iq=L_iv$ for every $i$. Put $d=v-q$. Then

$$
\int_{x_i}^{x_{i+1}}d(x)\,dx=0\qquad(1\leq i\leq n-1).
$$

On each interior knot interval $q''$ is a constant $c_i$, and on the two exterior intervals $q'=0$. Integrate $q'd'$ by parts separately on the intervals. At every knot the boundary contributions cancel because both $q'$ and $d$ are continuous; the contributions at $a$ and $b$ vanish because $q'$ is zero there. Thus

$$
\int_a^bq'(x)d'(x)\,dx
=-\sum_{i=1}^{n-1}c_i\int_{x_i}^{x_{i+1}}d(x)\,dx=0.
$$

This orthogonality is the key to the [quadratic smoothing spline for interval averages](../../../nonparametric-statistics.md#quadratic-smoothing-spline-for-interval-averages). Expanding the roughness penalty gives

$$
\int_a^b[v'(x)]^2\,dx
=\int_a^b[q'(x)]^2\,dx+\int_a^b[d'(x)]^2\,dx.
$$

The data-fit terms are equal because the interval averages are equal. Consequently,

$$
\boxed{S_\lambda(v)=S_\lambda(q)+\lambda\int_a^b[d'(x)]^2\,dx\geq S_\lambda(q).}
$$

Equality can occur only if $d'=0$ everywhere: the [derivative](../../../calculus.md#derivative) is continuous and its squared integral is zero. Then $d$ is constant, and any of its zero interval averages forces that constant to be zero. Therefore every minimizer must equal its matching [quadratic spline](../../../uniform-approximation.md#quadratic-spline) $q$.

We conclude that **the minimizer is a continuously differentiable quadratic spline with knots at the specified sites and constant tails on both exterior intervals.** Existence and uniqueness also follow from the supplied interpolation property. The interval-average map identifies the finite-dimensional space of these [quadratic splines](../../../uniform-approximation.md#quadratic-spline) with $\mathbb R^{n-1}$, and the criterion becomes a [strictly convex](../../../real-analysis.md#strictly-convex-function) quadratic function of that average vector: its data-fit term is $\|Y-y\|^2$, while its penalty is nonnegative and quadratic. It has a unique minimizer, and the strict equality argument above proves uniqueness in the full function class.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
