# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper41.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $\Lambda=\sum_{i=1}^m\lambda_i$. For $\Lambda>0$, the resulting [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution) has

$$
\boxed{\text{count parameter }\Lambda,\qquad
F(x)=\sum_{i=1}^m\frac{\lambda_i}{\Lambda}F_i(x).}
$$

Thus the merged [claim size](../../../actuarial-statistics.md#claim-size) [probability distribution](../../../probability-theory.md#probability-distribution) is a rate-weighted [mixture distribution](../../../probability-theory.md#mixture-distribution), not an equally weighted [mixture distribution](../../../probability-theory.md#mixture-distribution) unless the rates agree.

To prove this without any [moment-generating function](../../../probability-theory.md#moment-generating-function) assumption, let $\chi_i(t)$ be the [characteristic function](../../../probability-theory.md#characteristic-function) of a claim of type $i$. Conditioning on its [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) count gives

$$
\mathbb Ee^{itS_i}=\exp\{\lambda_i(\chi_i(t)-1)\}.
$$

[Independence](../../../random-variable.md#independent-random-variables) of the aggregate risks therefore gives

$$
\mathbb Ee^{itS}
=\prod_i\exp\{\lambda_i(\chi_i(t)-1)\}
=\exp\left\{\Lambda\left(\sum_i\frac{\lambda_i}{\Lambda}\chi_i(t)-1\right)\right\}.
$$

The weighted [characteristic function](../../../probability-theory.md#characteristic-function) inside is precisely that of the displayed [mixture distribution](../../../probability-theory.md#mixture-distribution). This is the transform of a sum of [independent](../../../random-variable.md#independent-random-variables) claims with [independent](../../../random-variable.md#independent-random-variables) count $\operatorname{Pois}(\Lambda)$, proving the claim by uniqueness of [characteristic functions](../../../probability-theory.md#characteristic-function). This is [Poisson superposition of insurance portfolios](../../../actuarial-statistics.md#poisson-superposition-of-insurance-portfolios). If $\Lambda=0$, all risks make no claims [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and $S=0$; the severity law is then irrelevant.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use the preceding construction with type-$i$ claims of deterministic size $a_i$. For $\Lambda=\sum_i\lambda_i>0$, the answer is

$$
\boxed{N\sim\operatorname{Pois}(\Lambda),\qquad
\mathbb P(X=a_i)=\frac{\lambda_i}{\Lambda},\qquad
F_X(x)=\sum_{i:a_i\le x}\frac{\lambda_i}{\Lambda}.}
$$

The [characteristic function](../../../probability-theory.md#characteristic-function) verifies this directly:

$$
\mathbb Ee^{itT}=\prod_i\exp\{\lambda_i(e^{ita_i}-1)\}
=\exp\{\Lambda(\mathbb Ee^{itX}-1)\}.
$$

Hence $T$ has the stated [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution). Distinctness of the $a_i$ makes the atomic [probabilities](../../../probability-theory.md#probability) unambiguous.

A zero coefficient is allowed. It corresponds to zero-sized claims in this representation and contributes nothing to $T$. If a representation using only positive claims is preferred, remove that category: its count parameter becomes $\Lambda_+=\sum_{i:a_i>0}\lambda_i$, with [probabilities](../../../probability-theory.md#probability) $\lambda_i/\Lambda_+$ on the positive values. The [zero claim sizes in a compound Poisson representation](../../../actuarial-statistics.md#zero-claim-sizes-in-a-compound-poisson-representation) explain why the count parameter need not be unique. If $\Lambda=0$, or if all positive-size categories have zero rate, the aggregate is identically zero.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Define $N_i=\sum_{k=1}^N\mathbf1_{\{X_k=a_i\}}$. Grouping equal [claim sizes](../../../actuarial-statistics.md#claim-size) gives the pathwise identity

$$
\boxed{\widetilde T=\sum_{i=1}^m a_iN_i.}
$$

Conditional on $N=n$, the $n$ [independent](../../../random-variable.md#independent-random-variables) claims receive category labels with [probabilities](../../../probability-theory.md#probability) $p_i$. There are $n!/(n_1!\cdots n_m!)$ assignments producing prescribed category counts, and every assignment has [probability](../../../probability-theory.md#probability) $\prod_i p_i^{n_i}$. Thus the conditional [probability distribution](../../../probability-theory.md#probability-distribution) is a [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution):

$$
\mathbb P(N_1=n_1,\ldots,N_m=n_m\mid N=n)
=\frac{n!}{\prod_i n_i!}\prod_i p_i^{n_i}
$$

when the nonnegative counts sum to $n$, and is zero otherwise.

For $0\le z_i\le1$, condition first on $N$ and use the [probability generating function](../../../probability-theory.md#probability-generating-function) of a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution):

$$
\mathbb E\prod_i z_i^{N_i}
=\mathbb E\left(\sum_i p_i z_i\right)^N
=\exp\left\{\lambda\left(\sum_i p_i z_i-1\right)\right\}
=\prod_i\exp\{\lambda p_i(z_i-1)\}.
$$

This factorization is the joint [probability generating function](../../../probability-theory.md#probability-generating-function) of [independent](../../../random-variable.md#independent-random-variables) [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) variables. Hence

$$
\boxed{N_i\sim\operatorname{Pois}(\lambda p_i)\quad\text{independently}.}
$$

A category with $p_i=0$ has zero count [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The [categorical thinning of a Poisson claim count](../../../probability-theory.md#categorical-thinning-of-a-poisson-claim-count) produces [independence](../../../random-variable.md#independent-random-variables) after averaging over the random total, even though the counts are constrained to sum to $n$ conditional on that total.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $M_X(t)=\mathbb Ee^{tX}$. Conditioning on $N\sim\operatorname{Pois}(\lambda)$ gives

$$
\mathbb Ee^{tS}=\mathbb E[M_X(t)^N]
=\exp\{\lambda(M_X(t)-1)\},\qquad
\boxed{K_S(t)=\lambda(M_X(t)-1).}
$$

Where the [moment-generating function](../../../probability-theory.md#moment-generating-function) is finite around zero, differentiating the [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) gives

$$
\boxed{\kappa_j(S)=K_S^{(j)}(0)=\lambda\mathbb E[X^j].}
$$

In particular $\mathbb ES=\lambda\mathbb EX$ and $\operatorname{Var}S=\lambda\mathbb EX^2$. These [compound Poisson cumulants](../../../actuarial-statistics.md#compound-poisson-cumulants) use raw claim [moments](../../../probability-theory.md#moment). The first two formulas also follow by conditioning: $\mathbb E[S\mid N]=N\mathbb EX$ and $\operatorname{Var}(S\mid N)=N\operatorname{Var}X$, so

$$
\operatorname{Var}S=\mathbb E[N]\operatorname{Var}X+\operatorname{Var}N(\mathbb EX)^2
=\lambda\mathbb EX^2.
$$

This is the [law of total variance](../../../probability-theory.md#law-of-total-variance). They therefore remain valid with finite first two [moments](../../../probability-theory.md#moment) even when no positive exponential [moment](../../../probability-theory.md#moment) exists.

Under per-claim [excess of loss reinsurance](../../../actuarial-statistics.md#excess-of-loss-reinsurance), put $Y=\min(X,M)$ and let $W=(X-M)_+$ be the [positive part](../../../function.md#positive-part-of-a-real-valued-function) of the excess. The insurer and reinsurer totals are sums of these payments over the same [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) count. Write $\overline F(x)=\mathbb P(X>x)$. Using the [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments) on the tail [probabilities](../../../probability-theory.md#probability) of $Y$ and $W$ gives

$$
\boxed{\begin{aligned}
\mathbb ES_I&=\lambda\int_0^M\overline F(x)\,dx,&
\operatorname{Var}S_I&=2\lambda\int_0^M x\overline F(x)\,dx,\\
\mathbb ES_R&=\lambda\int_M^\infty\overline F(x)\,dx,&
\operatorname{Var}S_R&=2\lambda\int_M^\infty(x-M)\overline F(x)\,dx.
\end{aligned}}
$$

For example, $\mathbb EY^2=\int_0^\infty\mathbb P(Y^2>t)dt=2\int_0^M x\overline F(x)dx$ after $t=x^2$, and shifting by $M$ gives the reinsurer formula. The [moment](../../../probability-theory.md#moment) formulas are finite whenever the corresponding claim [moments](../../../probability-theory.md#moment) are finite.

For the specified [Pareto distribution](../../../continuous-probability-distribution.md#pareto-distribution), with shape three and minimum $d>0$,

$$
\overline F(x)=\begin{cases}1,&0\le x\le d,\\d^3/x^3,&x\ge d,\end{cases}
\qquad\mathbb EX=3d/2,\quad\mathbb EX^2=3d^2.
$$

If $0\le M\le d$, every claim exceeds the [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention). Therefore

$$
\begin{aligned}
\mathbb ES_I&=\lambda M,&\operatorname{Var}S_I&=\lambda M^2,\\
\mathbb ES_R&=\lambda(3d/2-M),&\operatorname{Var}S_R&=\lambda(3d^2-3dM+M^2).
\end{aligned}
$$

If $M\ge d$, the tail integrals instead give

$$
\begin{aligned}
\mathbb ES_I&=\lambda\left(\frac{3d}{2}-\frac{d^3}{2M^2}\right),&
\operatorname{Var}S_I&=\lambda\left(3d^2-\frac{2d^3}{M}\right),\\
\mathbb ES_R&=\frac{\lambda d^3}{2M^2},&
\operatorname{Var}S_R&=\frac{\lambda d^3}{M}.
\end{aligned}
$$

Consequently the requested sum of [variances](../../../variance.md) is

$$
V(M)=\lambda\begin{cases}
3d^2-3dM+2M^2,&0\le M\le d,\\
3d^2-d^3/M,&M\ge d.
\end{cases}
$$

On the first branch, $V'(M)=\lambda(4M-3d)$; it decreases until $M=3d/4$ and then increases. On the second branch $V'(M)=\lambda d^3/M^2>0$. For $\lambda>0$ the minimum is unique; if $\lambda=0$, all [variances](../../../variance.md) are zero and every [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention) minimizes them. Thus

$$
\boxed{M^*=\frac{3d}{4},\qquad V(M^*)=\frac{15}{8}\lambda d^2.}
$$

The curve starts at $3\lambda d^2$, reaches this minimum, passes through $V(d)=2\lambda d^2$ with matching slope $\lambda d$ on both branches, and then increases concavely toward the horizontal [asymptote](../../../topology.md#asymptote) $3\lambda d^2$. The [variance-minimizing retention for shape-three Pareto claims](../../../actuarial-statistics.md#variance-minimizing-retention-for-shape-three-pareto-claims) is shown below.

<a id="2/image-sum-of-insurer-and-reinsurer-aggregate-variances-for-shape-three-pareto-claims-minimized-at-retention-three-quarters-of-the-minimum-claim-size"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-41-retention.png)

**[Figure 1](#2/image-sum-of-insurer-and-reinsurer-aggregate-variances-for-shape-three-pareto-claims-minimized-at-retention-three-quarters-of-the-minimum-claim-size). Sum of insurer and reinsurer aggregate variances for shape-three Pareto claims, minimized at retention three quarters of the minimum claim size**.

The two aggregate payouts are dependent. Conditioning on the common count gives [covariance](../../../variance.md#covariance) $\lambda\operatorname{Cov}(Y,W)+\lambda\mathbb EY\mathbb EW=\lambda\mathbb E[YW]=\lambda M\mathbb EW$, so $V(M)+2\operatorname{Cov}(S_I,S_R)=3\lambda d^2$ for every [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention), as required by $S_I+S_R=S$. The [covariance of two components of a compound Poisson sum](../../../actuarial-statistics.md#covariance-of-two-components-of-a-compound-poisson-sum) accounts for this distinction between a sum of [variances](../../../variance.md) and the [variance](../../../variance.md) of a sum.

There is a [moment](../../../probability-theory.md#moment) domain qualification for this heavy-tailed example. For every $t>0$, $\int_d^\infty e^{tx}3d^3x^{-4}dx=\infty$, and [moments](../../../probability-theory.md#moment) of order $j\ge3$ also diverge. Thus its positive [moment-generating function](../../../probability-theory.md#moment-generating-function) is not finite and higher finite [cumulants](../../../probability-theory.md#cumulant) cannot be obtained by differentiating around zero. Its [mean](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) calculations above are valid by conditioning or by the first two right derivatives at zero of the [Laplace transform of a nonnegative random variable](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable).

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For nontrivial positive [claim sizes](../../../actuarial-statistics.md#claim-size) in the [classical risk model](../../../actuarial-statistics.md#classical-risk-model) and $\lambda>0$, the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) is the unique positive solution

$$
\boxed{\lambda(M_X(R)-1)=cR,\qquad 0<R<r_\infty.}
$$

Indeed, $h(r)=\lambda(M_X(r)-1)-cr$ has $h(0)=0$, $h'(0)=\lambda\mu-c<0$, and is [strictly convex](../../../real-analysis.md#strictly-convex-function). It becomes positive near the right endpoint of the [moment-generating function](../../../probability-theory.md#moment-generating-function) domain. For a finite endpoint this follows from the assumed divergence; for an infinite endpoint, $\mathbb P(X\ge\varepsilon)>0$ for some $\varepsilon>0$ gives an exponential lower bound on $M_X(r)$, which eventually exceeds any linear function. [Convexity](../../../real-analysis.md#convex-function) gives existence and uniqueness of the positive crossing and $\lambda M_X'(R)-c>0$.

Put $q=\lambda\mu/c$ and $\overline F=1-F$. Substituting $\varphi=1-\psi$ into the supplied [survival renewal equation for a classical risk model](../../../actuarial-statistics.md#survival-renewal-equation-for-a-classical-risk-model), and using $\int_0^\infty\overline F(x)dx=\mu$, yields

$$
\psi(u)=\frac{\lambda}{c}\int_u^\infty\overline F(x)\,dx
+\frac{\lambda}{c}\int_0^u\psi(u-x)\overline F(x)\,dx.
$$

Multiplying by $e^{Ru}$ gives the proper renewal-type equation

$$
\boxed{Z(u)=g_R(u)+\int_0^u Z(u-x)k_R(x)\,dx,}
\qquad
k_R(x)=\frac{\lambda}{c}e^{Rx}\overline F(x),\quad
g_R(u)=\frac{\lambda}{c}e^{Ru}\int_u^\infty\overline F(x)\,dx.
$$

The [exponential tilt of the ruin renewal kernel](../../../probability-theory.md#exponential-tilt-of-the-ruin-renewal-kernel) turns a defective kernel into a [probability density function](../../../continuous-probability-distribution.md#probability-density-function), because the tail integration identity gives

$$
\int_0^\infty k_R(x)dx
=\frac{\lambda}{c}\frac{M_X(R)-1}{R}=1.
$$

This identity follows also by integrating $e^{RX}-1=R\int_0^X e^{Rx}dx$ and applying [Tonelli theorem](../../../measure-theory.md#tonelli-theorem). The tilted [probability density function](../../../continuous-probability-distribution.md#probability-density-function) defines a [nonarithmetic distribution](../../../probability-theory.md#nonarithmetic-distribution), even if the [claim size](../../../actuarial-statistics.md#claim-size) [probability distribution](../../../probability-theory.md#probability-distribution) itself has atoms.

Differentiate $(M_X(R)-1)/R$ to calculate its [mean](../../../probability-theory.md#expected-value):

$$
m_R=\int_0^\infty xk_R(x)dx
=\frac{\lambda}{c}\frac{RM_X'(R)-M_X(R)+1}{R^2}
=\frac{\lambda M_X'(R)-c}{cR}.
$$

It is finite and positive because $R$ is inside the finite [moment-generating function](../../../probability-theory.md#moment-generating-function) domain. Next, reversing the order of integration gives

$$
\begin{aligned}
\int_0^\infty g_R(u)du
&=\frac{\lambda}{c}\int_0^\infty\overline F(x)\int_0^x e^{Ru}du\,dx\\
&=\frac{\lambda}{cR}\left(\frac{M_X(R)-1}{R}-\mu\right)
=\frac{c-\lambda\mu}{cR}.
\end{aligned}
$$

The forcing function is [directly Riemann integrable](../../../real-analysis.md#direct-riemann-integrability). Choose $\varepsilon>0$ with $M_X(R+\varepsilon)<\infty$. [Markov's inequality](../../../probability-inequality.md#markov-inequality) bounds $\overline F(x)$ by $M_X(R+\varepsilon)e^{-(R+\varepsilon)x}$, so $g_R(u)$ is bounded by a constant times $e^{-\varepsilon u}$. It is continuous; on finite intervals continuity controls its [Riemann sums](../../../real-analysis.md#riemann-sum), and the exponential envelope controls the tails. These are sufficient conditions for [direct Riemann integrability](../../../real-analysis.md#direct-riemann-integrability).

Iterating the [renewal equation](../../../probability-theory.md#renewal-equation) by [convolution](../../../fourier-analysis.md#convolution) gives $Z=g_R*U_R$, where $U_R=\sum_{n\ge0}k_R^{*n}$ is the [renewal measure](../../../probability-theory.md#renewal-measure). The remainder after $n$ iterations is bounded on each fixed interval by a constant times the chance that a sum of $n$ positive interarrivals remains in that interval, which tends to zero. The [key renewal theorem](../../../probability-theory.md#key-renewal-theorem), applicable to this [nonarithmetic distribution](../../../probability-theory.md#nonarithmetic-distribution) of finite [mean](../../../probability-theory.md#expected-value) and the directly integrable forcing, now gives the [interior adjustment coefficient ruin prefactor](../../../actuarial-statistics.md#interior-adjustment-coefficient-ruin-prefactor):

$$
\boxed{A=\lim_{u\to\infty}e^{Ru}\psi(u)
=\frac{\int_0^\infty g_R(u)du}{m_R}
=\frac{c-\lambda\mu}{\lambda M_X'(R)-c}.}
$$

Both numerator and denominator are positive, so $0<A<\infty$.

For the unit-rate shape-two [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution), $\mu=2$, $M_X(r)=(1-r)^{-2}$ and $M_X'(r)=2(1-r)^{-3}$. Write $\delta=\lambda/c$, so positive loading requires $0<\delta<1/2$. Dividing the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation by its nonzero root gives $\delta(2-R)=(1-R)^2$. Thus

$$
\boxed{R=1-\frac{\delta+\sqrt{\delta^2+4\delta}}2,\qquad
A=\frac{1-2\delta}{2\delta(1-R)^{-3}-1}
=\frac{(1-R)(3-2R)}{3-R}.}
$$

The last simplification uses $\delta=(1-R)^2/(2-R)$; it is the [Erlang shape-two ruin prefactor](../../../actuarial-statistics.md#erlang-shape-two-ruin-prefactor). Its value depends on the premium-to-arrival ratio, which is not specified numerically.

For the final exponential representation, evaluating at zero in the [survival renewal equation for a classical risk model](../../../actuarial-statistics.md#survival-renewal-equation-for-a-classical-risk-model) gives **$\lambda\mu/c=\psi(0)=a+b$**. If the slower term is present, necessarily $a>0$ and $e^u\psi(u)\to a$. Comparing with the finite positive asymptotic constant just proved yields

$$
\boxed{R=1,\qquad A=a,\qquad\lambda\mu/c=a+b\quad(a>0).}
$$

A smaller [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) would make the limit zero and a larger one would make it infinite. Here the [leading exponential term determines a ruin adjustment coefficient](../../../actuarial-statistics.md#leading-exponential-term-determines-a-ruin-adjustment-coefficient). The coefficient $b$ need not be assumed positive to identify the leading term.

The wording does not specify that $a$ is nonzero. If $a=0$ and $b>0$, the only surviving term instead gives **$R=6$, $A=b$ and $\lambda\mu/c=b$**. This case is realizable: claims with an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\beta=6+\lambda/c$ have [ultimate ruin probability](../../../actuarial-statistics.md#ultimate-ruin-probability) $(\lambda/(c\beta))e^{-6u}$. Negative $a$ would make the [ultimate ruin probability](../../../actuarial-statistics.md#ultimate-ruin-probability) negative for large $u$, and both coefficients zero are incompatible with a nontrivial positive claim rate and [mean](../../../probability-theory.md#expected-value). These observations specify the coefficient qualification needed for the usual $R=1$ answer.

## 4

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the shape-rate convention for the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) $\theta\sim\operatorname{Gamma}(\alpha,\beta)$, with [prior distribution](../../../statistical-inference.md#prior-probability) [probability density function](../../../continuous-probability-distribution.md#probability-density-function) proportional to $\theta^{\alpha-1}e^{-\beta\theta}$. The observations are [independent](../../../random-variable.md#independent-random-variables) conditional on the common parameter $\theta$. Unconditionally a common nondegenerate [prior distribution](../../../statistical-inference.md#prior-probability) induces [covariance](../../../variance.md#covariance) $\alpha/\beta^2$ between distinct observations, so the [Bayesian inference](../../../statistical-inference.md#bayesian-statistics) model requires conditional [independence](../../../random-variable.md#independent-random-variables).

For unit-exposure counts, the [likelihood](../../../statistical-modelling.md#likelihood-function) is proportional to $\theta^{\sum_i x_i}e^{-n\theta}$. Multiplying by the [prior distribution](../../../statistical-inference.md#prior-probability) gives

$$
\theta\mid\mathbf x\sim\operatorname{Gamma}\left(\alpha+\sum_{i=1}^n x_i,\ \beta+n\right).
$$

The future count has [conditional expectation](../../../measure-theory.md#conditional-expectation) $\theta$, so [posterior distribution](../../../statistical-inference.md#bayesian-posterior) averaging gives

$$
\boxed{\mathbb E[X_{n+1}\mid\mathbf x]
=\frac{\alpha+\sum_i x_i}{\beta+n}
=\frac{n}{n+\beta}\overline x+\frac{\beta}{n+\beta}\frac\alpha\beta.}
$$

This is an exact [Bayesian credibility](../../../actuarial-statistics.md#bayesian-credibility) estimate, with [credibility factor](../../../actuarial-statistics.md#credibility-factor) $Z=n/(n+\beta)$ and collective [mean](../../../probability-theory.md#expected-value) $\alpha/\beta$.

For the [insurance exposure](../../../actuarial-statistics.md#insurance-exposure) and [claims inflation](../../../actuarial-statistics.md#claims-inflation) calculation put $c_j=c(1+r)^j$, assuming $c>0$, $1+r>0$ and positive policy counts $n_j$. Let $K_j$ be the total claim count in year $j$. [Conditional independence](../../../random-variable.md#conditional-independence) of the policy counts gives $K_j\mid\theta\sim\operatorname{Pois}(n_j\theta)$, and the observed average amount satisfies

$$
Y_j=\frac{c_jK_j}{n_j},\qquad k_j=\frac{n_jy_j}{c_j}.
$$

For possible observations, the recovered $k_j$ are nonnegative integers. If they are not, the data have zero [likelihood](../../../statistical-modelling.md#likelihood-function) under the model and no conditional [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is defined for those impossible values.

Write $W=\sum_{j=1}^n n_j$ and $K=\sum_{j=1}^n k_j$. Since $Y_j$ and $K_j$ determine each other, conditioning on the observed average amounts is equivalent to conditioning on these counts. The [independent](../../../random-variable.md#independent-random-variables) yearly count [likelihood](../../../statistical-modelling.md#likelihood-function) is

$$
\prod_{j=1}^n e^{-n_j\theta}\frac{(n_j\theta)^{k_j}}{k_j!}
\propto\theta^K e^{-W\theta}.
$$

The [Poisson-gamma conjugacy with unequal exposures](../../../statistical-inference.md#poisson-gamma-conjugacy-with-unequal-exposures) therefore gives

$$
\boxed{\theta\mid\mathbf y\sim\operatorname{Gamma}(\alpha+K,\beta+W).}
$$

For the future year, $\mathbb E[Y_{n+1}\mid\theta]=c_{n+1}\theta$; the number of future policies cancels because $Y_{n+1}$ is a per-policy average. Hence

$$
\boxed{\mathbb E[Y_{n+1}\mid\mathbf y]
=c_{n+1}\frac{\alpha+K}{\beta+W}
=Z\,m(\mathbf y)+(1-Z)m,}
$$

with

$$
\boxed{\begin{aligned}
Z&=\frac{W}{W+\beta},\\
m&=c(1+r)^{n+1}\frac\alpha\beta,\\
m(\mathbf y)&=c_{n+1}\frac KW
=\frac1W\sum_{j=1}^n n_j(1+r)^{n+1-j}y_j.
\end{aligned}}
$$

The collective [mean](../../../probability-theory.md#expected-value) $m$ is the [prior distribution](../../../statistical-inference.md#prior-probability) expected claim amount per policy in the future year's monetary units. The experience [mean](../../../probability-theory.md#expected-value) $m(\mathbf y)$ first inflates each past per-policy amount to that same future year and then averages with policy-exposure weights. Equivalently, it estimates annual claim frequency by total observed claims divided by total past [insurance exposure](../../../actuarial-statistics.md#insurance-exposure) and converts that frequency to the future claim cost. This is [inflation-adjusted Poisson-gamma credibility](../../../actuarial-statistics.md#inflation-adjusted-poisson-gamma-credibility).

For fixed [prior distribution](../../../statistical-inference.md#prior-probability) parameters, $Z$ increases strictly with total past [insurance exposure](../../../actuarial-statistics.md#insurance-exposure): $dZ/dW=\beta/(W+\beta)^2>0$, and **$Z\to1$ as $W\to\infty$**. The [prior distribution](../../../statistical-inference.md#prior-probability) weight decreases to zero; $\beta$ acts as equivalent [prior distribution](../../../statistical-inference.md#prior-probability) [insurance exposure](../../../actuarial-statistics.md#insurance-exposure). With no past [insurance exposure](../../../actuarial-statistics.md#insurance-exposure) the appropriate weight is zero and the prediction is $m$, without defining an empirical experience [mean](../../../probability-theory.md#expected-value).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
