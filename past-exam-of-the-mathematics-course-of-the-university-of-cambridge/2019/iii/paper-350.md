# Paper 350

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_350.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_350.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 350](paper-350.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\pi_0$ be the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of the unknown and $\rho$ that of the noise, both relative to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). By [independence of random variables](../../../random-variable.md#independent-random-variables), the [conditional distribution](../../../probability-theory.md#conditional-distribution) of the measurement given $u$ has density $\rho(m-Au)$. Thus its [likelihood function](../../../statistical-modelling.md#likelihood-function) and the joint density are

$$
\pi(m\mid u)=\rho(m-Au),\qquad
\pi(u,m)=\pi_0(u)\rho(m-Au).
$$

The [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence) is the marginal data density

$$
Z(m)=\int_{\mathbb R^d}\pi_0(v)\rho(m-Av)\,dv.
$$

[Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives the [posterior density](../../../statistical-inference.md#posterior-density) solving this [Bayesian inverse problem](../../../stochastic-process.md#bayesian-inverse-problem):

$$
\boxed{\pi^m(u)=\frac{\pi_0(u)\rho(m-Au)}{Z(m)}.}
$$

This formula applies when $0<Z(m)<\infty$. Since $\int Z(m)\,dm=1$ by [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), these conditions hold [almost everywhere](../../../measure-theory.md#almost-everywhere) under the marginal data law. Values of a [conditional distribution](../../../probability-theory.md#conditional-distribution) at exceptional data are not determined by the joint law. The [posterior mean](../../../statistical-inference.md#posterior-mean) or a [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) can then give a point estimate, while the full [posterior density](../../../statistical-inference.md#posterior-density) describes the remaining uncertainty.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $a=(2,1)^T$, so the data map is $a^Tu$. The [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood) and [prior distribution](../../../statistical-inference.md#prior-probability) give

$$
\pi^m(u)\propto\exp\left[-\frac12u^Tu-\frac{(m-a^Tu)^2}{2\delta^2}\right].
$$

[Completing the square](../../../polynomial.md#completing-the-square), or using [Gaussian conjugacy for a normal linear model](../../../statistical-modelling.md#gaussian-conjugacy-for-a-normal-linear-model), identifies a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) with [precision matrix](../../../variance.md#precision-matrix) $C_\delta^{-1}=I_2+\delta^{-2}aa^T$. Since $a^Ta=5$, its [posterior mean](../../../statistical-inference.md#posterior-mean) and [covariance matrix](../../../variance.md#covariance-matrix) are

$$
\boxed{u\mid m\sim\mathcal N(b_\delta,C_\delta).}
$$

The parameters are

$$
\begin{aligned}
b_\delta&=\frac{m}{5+\delta^2}\begin{pmatrix}2\\1\end{pmatrix},\\
C_\delta&=I_2-\frac{aa^T}{5+\delta^2}
=\frac1{5+\delta^2}\begin{pmatrix}1+\delta^2&-2\\-2&4+\delta^2\end{pmatrix}.
\end{aligned}
$$

For example, $(I_2+\delta^{-2}aa^T)C_\delta=I_2$, which checks the square completion.

The [orthogonal vectors](../../../linear-algebra.md#orthogonal-vectors)

$$
e_\parallel=\frac1{\sqrt5}(2,1)^T,\qquad
e_\perp=\frac1{\sqrt5}(-1,2)^T
$$

are [eigenvectors](../../../linear-operator-theory.md#eigenvector) of the [covariance matrix](../../../variance.md#covariance-matrix). Their respective [variances](../../../variance.md) are

$$
\boxed{\operatorname{Var}(e_\parallel^Tu\mid m)=\frac{\delta^2}{5+\delta^2},\qquad
\operatorname{Var}(e_\perp^Tu\mid m)=1.}
$$

They are independent under the [posterior distribution](../../../statistical-inference.md#bayesian-posterior), by [independence of uncorrelated jointly normal variables](../../../probability-and-statistics.md#independence-of-uncorrelated-jointly-normal-variables). Thus uncertainty is different in the two directions even for positive noise: the data constrain $e_\parallel$, whereas $e_\perp$ spans the [null space](../../../linear-algebra.md#kernel-of-a-linear-map) of the data map.

As $\delta\to0$, the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) converges to the law of

$$
\frac m5(2,1)^T+Ze_\perp,\qquad Z\sim\mathcal N(0,1).
$$

This is supported on $2u_1+u_2=m$, and its [posterior mean](../../../statistical-inference.md#posterior-mean) is the [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). The [prior distribution](../../../statistical-inference.md#prior-probability) still determines the distribution along the unobserved [null space](../../../linear-algebra.md#kernel-of-a-linear-map); it has not disappeared. This example of a [Gaussian posterior in the zero-noise limit](../../../statistical-modelling.md#gaussian-posterior-in-the-zero-noise-limit) distinguishes exact recovery of an observed component from recovery of the whole unknown.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the [Hellinger distance](../../../probability-and-statistics.md#hellinger-distance) convention in the original PDF:

$$
d_{\mathrm{Hell}}(\mu,\mu')^2=\frac12\int(\sqrt p-\sqrt q)^2\,d\nu
=1-\int\sqrt{pq}\,d\nu,
\qquad p=\frac{d\mu}{d\nu},\quad q=\frac{d\mu'}{d\nu}.
$$

The TeX transcription incorrectly places the integral outside the outer square root in the definition; the displayed formula for the squared distance and the original PDF both use the convention above. Although [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) is not a probability measure, we may use it as the common dominating measure: the integral is unchanged by replacing it with any equivalent dominating [probability measure](../../../probability-theory.md#probability-measure).

For unit-variance [normal distributions](../../../probability-theory.md#normal-distribution), put $\bar\theta=(\theta_1+\theta_2)/2$ and $\Delta=\theta_1-\theta_2$. The product of the square roots of their [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) is

$$
\sqrt{p_1(x)p_2(x)}
=\frac1{\sqrt{2\pi}}\exp\left[-\frac{(x-\theta_1)^2+(x-\theta_2)^2}{4}\right]
=e^{-\Delta^2/8}\frac1{\sqrt{2\pi}}e^{-(x-\bar\theta)^2/2}.
$$

The final factor integrates to one, so

$$
\boxed{d_{\mathrm{Hell}}(\mu_1,\mu_2)^2=1-e^{-(\theta_1-\theta_2)^2/8}.}
$$

For the bound at arbitrary $\sigma_1,\sigma_2>0$, use the given formula for the [Hellinger distance between normal distributions](../../../probability-and-statistics.md#hellinger-distance-between-normal-distributions) and write

$$
S=\sigma_1^2+\sigma_2^2,\qquad
B=\sqrt{\frac{2\sigma_1\sigma_2}{S}}\leq1,\qquad
x=\frac{(\theta_1-\theta_2)^2}{4S}.
$$

Since $1-e^{-x}\leq x$ for $x\geq0$,

$$
\begin{aligned}
d_{\mathrm{Hell}}^2
&=(1-B)+B(1-e^{-x})\\
&\leq\frac{1-B^2}{1+B}+x\\
&=\frac{(\sigma_1-\sigma_2)^2}{S(1+B)}
+\frac{(\theta_1-\theta_2)^2}{4S}\\
&\leq\frac{(\sigma_1-\sigma_2)^2+(\theta_1-\theta_2)^2}{S}.
\end{aligned}
$$

Therefore one valid choice is $\boxed{C_{\sigma_1,\sigma_2}=1/(\sigma_1^2+\sigma_2^2)}$. In particular this bound is uniform when the two standard deviations stay bounded away from zero.

## 2

↑ **Parent:** [Paper 350](paper-350.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The conditional mean estimator is the [posterior mean](../../../statistical-inference.md#posterior-mean)

$$
\boxed{\widehat u_{\mathrm{CM}}(m)=\mathbb E[u\mid m]
=\int_{\mathbb R^d}u\pi^m(u)\,du,}
$$

provided the first [moment](../../../probability-theory.md#moment) is finite. A [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) is any maximizer of the [posterior density](../../../statistical-inference.md#posterior-density) relative to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure):

$$
\boxed{\widehat u_{\mathrm{MAP}}(m)\in\operatorname*{arg\,max}_{u\in\mathbb R^d}\pi^m(u).}
$$

Existence of the [posterior density](../../../statistical-inference.md#posterior-density) alone does not guarantee a finite [posterior mean](../../../statistical-inference.md#posterior-mean) or existence of a maximizing point.

For the stated [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) and independent standard [Gaussian noise](../../../probability-theory.md#gaussian-noise), the negative log of the [posterior density](../../../statistical-inference.md#posterior-density), up to a constant, is

$$
\frac12\|m-Au\|^2+\frac12u^T\Sigma^{-1}u.
$$

Its [precision matrix](../../../variance.md#precision-matrix) $A^TA+\Sigma^{-1}$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), so [Gaussian conjugacy for a normal linear model](../../../statistical-modelling.md#gaussian-conjugacy-for-a-normal-linear-model) gives

$$
\boxed{\widehat u_{\mathrm{CM}}=(A^TA+\Sigma^{-1})^{-1}A^Tm
=\Sigma A^T(A\Sigma A^T+I_k)^{-1}m.}
$$

The two forms agree because

$$
(A^TA+\Sigma^{-1})\Sigma A^T=A^T(A\Sigma A^T+I_k).
$$

The [covariance matrix](../../../variance.md#covariance-matrix) is $(A^TA+\Sigma^{-1})^{-1}$, and the [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) equals the [posterior mean](../../../statistical-inference.md#posterior-mean) for this [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A simple choice is an independent [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution) at each pixel, giving a [Laplace prior for sparse images](../../../continuous-probability-distribution.md#laplace-prior-for-sparse-images):

$$
\boxed{\pi_0(u)=\left(\frac\lambda2\right)^d
\exp\left(-\lambda\sum_{j=1}^d|u_j|\right),\qquad\lambda>0.}
$$

Its negative log density penalizes the [L1 norm](../../../functional-analysis.md#l1-norm). Relative to a [normal distribution](../../../probability-theory.md#normal-distribution), it combines a sharp peak at zero with heavier tails, allowing most pixels to lie near the background level while a few have appreciable intensity. Quantitatively, $\mathbb P(|u_j|>\tau)=e^{-\lambda\tau}$, so the expected number of appreciable pixels is $de^{-\lambda\tau}$. Choosing $\lambda\tau$ large makes this small. This is a simple sparsity model: it does not enforce that nearby active pixels form connected objects, nor does its continuous density give exact zero pixels positive probability. Additional spatial modelling would be needed to insist on contiguous shapes.

To sample, draw independent $U_j\sim\mathcal U(0,1)$ and use [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling):

$$
\boxed{u_j=\begin{cases}
\lambda^{-1}\log(2U_j),&0<U_j\leq\tfrac12,\\
-\lambda^{-1}\log(2(1-U_j)),&\tfrac12<U_j<1.
\end{cases}}
$$

The endpoint events have probability zero and can be assigned arbitrary finite values. To justify the rule, the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) of a centered [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution) is

$$
F(x)=\begin{cases}
\tfrac12e^{\lambda x},&x\leq0,\\
1-\tfrac12e^{-\lambda x},&x\geq0.
\end{cases}
$$

The displayed rule is $F^{-1}(U_j)$, so $\mathbb P(u_j\leq x)=\mathbb P(U_j\leq F(x))=F(x)$. [Independence of random variables](../../../random-variable.md#independent-random-variables) then gives the stated product [prior distribution](../../../statistical-inference.md#prior-probability).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the shape-rate convention for the [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution). Define

$$
B=A^TA,\qquad u_* = B^{-1}A^Tm,\qquad
r=m-Au_*,\qquad
a=\alpha+\frac k2,\qquad
b(u)=\beta+\frac12\|m-Au\|^2.
$$

The zero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) assumption makes $B$ a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), and $u_*$ is the unique [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) solution. The [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood) contributes $\gamma^{k/2}$, which must be retained because $\gamma$ is unknown. Multiplying it by the [improper prior](../../../statistical-inference.md#improper-prior) and the [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) gives the [normal-gamma posterior with a flat prior](../../../statistical-modelling.md#normal-gamma-posterior-with-a-flat-prior):

$$
\boxed{\pi^m(u,\gamma)=\frac1{\mathcal Z}\gamma^{a-1}e^{-\gamma b(u)},\qquad u\in\mathbb R^d,\quad\gamma>0.}
$$

Here the constant density of the [improper prior](../../../statistical-inference.md#improper-prior) cancels on normalization. Put

$$
b_0=\beta+\tfrac12\|r\|^2>0,\qquad
s=a-\tfrac d2=\alpha+\tfrac{k-d}{2}>0.
$$

The [normal equation](../../../statistical-modelling.md#normal-equation) $A^Tr=0$ makes the residual orthogonal to the range of $A$. The [orthogonal decomposition by a closed subspace](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) into that range and its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) gives

$$
b(u)=b_0+\tfrac12(u-u_*)^TB(u-u_*).
$$

Integration over $u$ by the [Gaussian integral](../../../calculus.md#gaussian-integral), followed by integration over $\gamma$ using the [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution), yields

$$
\mathcal Z=\frac{(2\pi)^{d/2}}{\sqrt{\det B}}\frac{\Gamma(s)}{b_0^s}<\infty.
$$

Thus the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is proper, despite the [improper prior](../../../statistical-inference.md#improper-prior); here $k\geq d$ follows from the zero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) assumption.

[Completing the square](../../../polynomial.md#completing-the-square) in $u$ and collecting the powers of $\gamma$ give the two [conditional distributions](../../../probability-theory.md#conditional-distribution):

$$
\boxed{u\mid\gamma,m\sim\mathcal N(u_*,\gamma^{-1}B^{-1}),\qquad
\gamma\mid u,m\sim\operatorname{Gamma}(a,b(u)).}
$$

Explicitly their [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) are

$$
\pi(u\mid\gamma,m)=\frac{\gamma^{d/2}\sqrt{\det B}}{(2\pi)^{d/2}}
e^{-\frac\gamma2(u-u_*)^TB(u-u_*)},\qquad
\pi(\gamma\mid u,m)=\frac{b(u)^a}{\Gamma(a)}\gamma^{a-1}e^{-b(u)\gamma}.
$$

For a joint [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) relative to $du\,d\gamma$, first fix $\gamma>0$. The unique maximizing $u$ is $u_*$. The remaining log density is $(a-1)\log\gamma-b_0\gamma$ plus a constant. Consequently, if $a>1$,

$$
\boxed{\widehat u_{\mathrm{MAP}}=u_*,\qquad
\widehat\gamma_{\mathrm{MAP}}=\frac{\alpha+k/2-1}{\beta+\|r\|^2/2}.}
$$

The stated assumptions do not always imply $a>1$. If $a=1$, the supremum occurs as $\gamma\downarrow0$ but is not attained on $\gamma>0$; if $a<1$, the density is unbounded there. In either case there is no joint [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) in the stated parameter space. Calling zero a boundary mode does not make it an admissible positive precision.

If “MAP estimators” instead means separate modes of the [marginal distributions](../../../probability-theory.md#marginal-distribution), integration gives

$$
\pi(u\mid m)\propto\left[b_0+\tfrac12(u-u_*)^TB(u-u_*)\right]^{-a},\qquad
\gamma\mid m\sim\operatorname{Gamma}(s,b_0).
$$

Thus the marginal [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) of $u$ is always $u_*$, and that of $\gamma$ is $(s-1)/b_0$ when $s>1$, with the same nonattainment at zero when $s\leq1$. Joint and marginal maximization are different operations; the usual joint interpretation gives the preceding boxed pair.

## 3

↑ **Parent:** [Paper 350](paper-350.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Cameron-Martin space of a Gaussian measure](../../../stochastic-process.md#cameron-martin-space-of-a-gaussian-measure) $\mu=\mathcal N(0,\Sigma)$ is

$$
\boxed{E=\operatorname{Ran}\Sigma^{1/2},\qquad
\langle h,g\rangle_E=\langle\Sigma^{-1/2}h,\Sigma^{-1/2}g\rangle_{\mathcal H}.}
$$

The inverse is defined on the range of $\Sigma^{1/2}$. In this infinite-dimensional setting “positive definite” must mean $\langle\Sigma h,h\rangle>0$ for every nonzero $h$, rather than a uniform lower bound: a [trace-class operator](../../../compact-operator.md#trace-class-operator) cannot be uniformly positive on an infinite-dimensional [Hilbert space](../../../hilbert-space.md).

By the [spectral theorem for compact Hermitian operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators), choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_j)$ with $\Sigma e_j=\lambda_je_j$, $\lambda_j>0$, and $\sum_j\lambda_j<\infty$. (A strictly positive [trace-class operator](../../../compact-operator.md#trace-class-operator) also forces the ambient [Hilbert space](../../../hilbert-space.md) to be separable.) In coordinates $h_j=\langle h,e_j\rangle$,

$$
E=\left\{h\in\mathcal H:\sum_j\frac{h_j^2}{\lambda_j}<\infty\right\},\qquad
\|h\|_E^2=\sum_j\frac{h_j^2}{\lambda_j}.
$$

This is a [Hilbert space](../../../hilbert-space.md) with its indicated norm, even though its range need not be closed in the ambient norm.

The [Cameron-Martin theorem for a Gaussian measure](../../../stochastic-process.md#cameron-martin-theorem-for-a-gaussian-measure) states that the translated law $\mu_h(B)=\mu(B-h)=\mathcal N(h,\Sigma)(B)$ is an [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure) to $\mu$ exactly when $h\in E$. For such $h$, its [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) is

$$
\boxed{\frac{d\mu_h}{d\mu}(x)=\exp\left(\ell_h(x)-\tfrac12\|h\|_E^2\right),\qquad
\ell_h(x)=\lim_{N\to\infty}\sum_{j=1}^N\frac{h_jx_j}{\lambda_j}.}
$$

The series has [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) and converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) under $\mu$, since its independent summands have total [variance](../../../variance.md) $\sum_jh_j^2/\lambda_j$. Its law is $\mathcal N(0,\|h\|_E^2)$, so the density has [expected value](../../../probability-theory.md#expected-value) one. It is sometimes formally written $\ell_h(x)=\langle h,x\rangle_E$, but a typical infinite-dimensional Gaussian sample is not in $E$; the series interpretation is essential. If $h\notin E$, the two laws are [mutually singular measures](../../../measure-theory.md#mutually-singular-measures).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The notation $P_0=\mathcal N(0,I)$ denotes generalized [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) over $H=L^2(\mathbb R^2)$, not a [Gaussian measure](../../../stochastic-process.md#gaussian-measure) supported on $H$: the identity is not a [trace-class operator](../../../compact-operator.md#trace-class-operator) there. For example, realize the observation on a suitable space of [tempered distributions](../../../fourier-analysis.md#tempered-distribution). Its [Cameron-Martin space of a Gaussian measure](../../../stochastic-process.md#cameron-martin-space-of-a-gaussian-measure) is $H$. For deterministic $h\in H$, the stochastic pairing $W_m(h)$ has [normal distribution](../../../probability-theory.md#normal-distribution) $\mathcal N(0,\|h\|_H^2)$ under $P_0$ and is the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process) indexed by $H$.

Interpret the stated maps between [Sobolev spaces](../../../sobolev-space.md) as bounded [linear operators](../../../vector-space.md#linear-operator), as usual. In particular $K:H\to H^2(\mathbb R^2)\subset H$ is bounded, so its [adjoint operator](../../../hilbert-space.md#adjoint-operator) $K^*$ is bounded on $H$. Hence $A=K^*K$ maps $H$ into $H$, which is the property needed here. The stronger smoothing follows by [Sobolev duality](../../../sobolev-space.md#sobolev-duality): boundedness of $K:H^{-4}\to H^{-2}$ gives $K^*:H^2\to H^4$, and therefore $A:H\to H^4\subset H$. As $\Pi(H)=1$, the shift $Au$ belongs to the noise [Cameron-Martin space of a Gaussian measure](../../../stochastic-process.md#cameron-martin-space-of-a-gaussian-measure) for $\Pi$-almost every $u$.

The [white-noise likelihood for a square-integrable shift](../../../stochastic-process.md#white-noise-likelihood-for-a-square-integrable-shift), obtained from the [Cameron-Martin theorem for a Gaussian measure](../../../stochastic-process.md#cameron-martin-theorem-for-a-gaussian-measure) in its white-noise form, is

$$
L(u,m)=\frac{dP_u}{dP_0}(m)
=\exp\left(W_m(Au)-\tfrac12\|Au\|_H^2\right)
=e^{-\Phi(u;m)},\qquad
\Phi(u;m)=\tfrac12\|Au\|_H^2-W_m(Au).
$$

Here $P_u$ is the law of $Au+\eta$. In an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_j)$ of $H$, with white-noise coordinates $m_j$, the pairing under $P_0$ is

$$
W_m(Au)=\lim_{N\to\infty}\sum_{j=1}^Nm_j\langle Au,e_j\rangle_H.
$$

For fixed $u$ this has [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) and converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), since $\sum_j|\langle Au,e_j\rangle|^2=\|Au\|_H^2$. The stipulated joint measurability allows the likelihood to be used under $\nu_0(du,dm)=\Pi(du)P_0(dm)$. One must not replace this expression by a finite $\|m-Au\|_H^2$, because white noise is not $H$-valued. On the unbounded domain $\mathbb R^2$, membership of white noise in a global unweighted negative [Sobolev space](../../../sobolev-space.md) must not be assumed either; the stochastic pairing avoids that issue.

Let $\nu(du,dm)=\Pi(du)P_u(dm)$ be the actual joint law. The shift formula gives $\nu\ll\nu_0$ with [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) $L$. Define

$$
Z(m)=\int_HL(u,m)\,\Pi(du).
$$

For each fixed admissible $u$, the [moment-generating function of a normal distribution](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) gives

$$
\int L(u,m)\,P_0(dm)=
e^{-\|Au\|_H^2/2}\mathbb E^{P_0}e^{W_m(Au)}=1.
$$

By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), $\int Z(m)P_0(dm)=1$, so $Z(m)<\infty$ for $P_0$-almost every $m$. The likelihood is finite and strictly positive for $\nu_0$-almost every $(u,m)$; [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) then gives $Z(m)>0$ for $P_0$-almost every $m$. The marginal observation law is $Z(m)P_0(dm)$ and is an [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure) to $P_0$.

The [Bayes formula for a dominated observation model](../../../stochastic-process.md#bayes-formula-for-a-dominated-observation-model) therefore defines

$$
\boxed{\frac{d\Pi^m}{d\Pi}(u)=\frac1{Z(m)}
\exp\left(W_m(Au)-\tfrac12\|Au\|_{L^2}^2\right).}
$$

To verify that it is the [conditional distribution](../../../probability-theory.md#conditional-distribution), for measurable sets $B$ of unknowns and $C$ of data,

$$
\int_C\Pi^m(B)Z(m)\,P_0(dm)
=\int_{B\times C}L(u,m)\,\nu_0(du,dm)=\nu(B\times C).
$$

Thus the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is well defined for almost every observation under the actual data law. This is the appropriate almost-everywhere assertion supplied by [Bayes' theorem](../../../probability-theory.md#bayes-theorem); the stated assumptions do not prescribe a canonical posterior at every exceptional generalized datum.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose the common dominating [probability measure](../../../probability-theory.md#probability-measure) $\nu=(\mu+\mu')/2$ and let $p=d\mu/d\nu$, $q=d\mu'/d\nu$ be the [Radon-Nikodym derivatives](../../../measure-theory.md#radon-nikodym-derivative). The assumed second [moments](../../../probability-theory.md#moment) imply first-moment integrability by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Since $Y$ is a separable [Banach space](../../../banach-space.md), the measurable $f$ is a [strongly measurable function](../../../measure-theory.md#strongly-measurable-function), and both [expected values](../../../probability-theory.md#expected-value) exist as [Bochner integrals](../../../measure-theory.md#bochner-integral).

The difference of these [Bochner integrals](../../../measure-theory.md#bochner-integral) satisfies

$$
\begin{aligned}
\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|_Y
&=\left\|\int_Xf(p-q)\,d\nu\right\|_Y\\
&\leq\int_X\|f\|_Y\,|\sqrt p-\sqrt q|(\sqrt p+\sqrt q)\,d\nu\\
&\leq\left(\int_X\|f\|_Y^2(\sqrt p+\sqrt q)^2\,d\nu\right)^{1/2}
\left(\int_X(\sqrt p-\sqrt q)^2\,d\nu\right)^{1/2}.
\end{aligned}
$$

The first inequality is the norm bound for a [Bochner integral](../../../measure-theory.md#bochner-integral), and the second is the scalar [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Since $(\sqrt p+\sqrt q)^2\leq2(p+q)$, the first factor is at most

$$
\sqrt{2}\left(\mathbb E^\mu\|f\|_Y^2+\mathbb E^{\mu'}\|f\|_Y^2\right)^{1/2}.
$$

With the [Hellinger distance](../../../probability-and-statistics.md#hellinger-distance) convention of the original PDF, the second factor is $\sqrt2\,d_{\mathrm{Hell}}(\mu,\mu')$. Multiplication proves the [Hellinger bound for differences of expectations](../../../probability-and-statistics.md#hellinger-bound-for-differences-of-expectations):

$$
\boxed{\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|_Y
\leq2\left(\mathbb E^\mu\|f\|_Y^2+\mathbb E^{\mu'}\|f\|_Y^2\right)^{1/2}
d_{\mathrm{Hell}}(\mu,\mu').}
$$

The proof uses only the two laws and their common dominating measure; no [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) assumption between $\mu$ and $\mu'$ is needed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
