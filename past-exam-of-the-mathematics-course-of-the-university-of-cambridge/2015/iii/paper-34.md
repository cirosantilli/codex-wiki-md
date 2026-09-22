# Paper 34

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_34.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_34.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $m_X=\mathbb E X_1$ and $v_X=\operatorname{Var}(X_1)$. For the [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims), conditioning on $N$ gives

$$
\mathbb E[S\mid N]=Nm_X,\qquad \operatorname{Var}(S\mid N)=Nv_X.
$$

The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) and the [law of total variance](../../../probability-theory.md#law-of-total-variance) therefore give **the aggregate moments**

$$
\boxed{\mathbb ES=(\mathbb EN)m_X,\qquad
\operatorname{Var}(S)=(\mathbb EN)v_X+\operatorname{Var}(N)m_X^2.}
$$

The first term in the [variance](../../../variance.md) measures variation of the individual claims at a fixed count; the second measures variation of the count itself. These formulas require the indicated moments to be finite.

For the [moment-generating function](../../../probability-theory.md#moment-generating-function), [independent random variables](../../../random-variable.md#independent-random-variables) give

$$
\mathbb E[e^{tS}\mid N]=M_X(t)^N,
\qquad
\boxed{M_S(t)=G_N(M_X(t)),}
$$

where $G_N(z)=\mathbb E[z^N]$ is the [probability generating function](../../../probability-theory.md#probability-generating-function). This identity holds wherever the expectations are finite; in particular a [moment-generating function](../../../probability-theory.md#moment-generating-function) need not exist for positive $t$ for an arbitrary positive claim distribution. The empty sum for $N=0$ is zero.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with [expected value](../../../probability-theory.md#expected-value) $\mu$,

$$
\mathbb EX_1=\mu,\qquad \operatorname{Var}(X_1)=\mu^2.
$$

The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has both [expected value](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) equal to $\lambda$. Substitution into the [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims) formulas gives **the portfolio A moments**

$$
\boxed{\mathbb E S_A=\lambda\mu,\qquad \operatorname{Var}(S_A)=2\lambda\mu^2.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

To distinguish the random intensity from its possible values, write it as $\Lambda$. Its law is a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $2$ and rate $p/q$. Hence

$$
\boxed{\lambda_0=\mathbb E\Lambda=\frac{2q}{p}},\qquad
\operatorname{Var}(\Lambda)=\frac{2q^2}{p^2}.
$$

For the [Poisson mixture](../../../discrete-probability-distribution.md#poisson-mixture), [conditional expectation](../../../measure-theory.md#conditional-expectation) and [conditional variance](../../../variance.md#conditional-variance) both equal $\Lambda$. The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) and the [law of total variance](../../../probability-theory.md#law-of-total-variance) yield

$$
\mathbb EN=\frac{2q}{p},\qquad
\operatorname{Var}(N)=\mathbb E\Lambda+\operatorname{Var}(\Lambda)
=\frac{2q}{p^2},
$$

where $p+q=1$. Applying the [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims) formulas with the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of the claim sizes gives **the portfolio B moments**

$$
\boxed{\mathbb ES_B=\frac{2q\mu}{p},\qquad
\operatorname{Var}(S_B)=\frac{2q(1+p)\mu^2}{p^2}.}
$$

At the matched intensity $\lambda_0$, the [expected value](../../../probability-theory.md#expected-value) for portfolio A is also $2q\mu/p$, whereas its [variance](../../../variance.md) is $4q\mu^2/p$. Thus **the expected totals agree, but mixing increases the variance**:

$$
\boxed{\operatorname{Var}(S_B)-\operatorname{Var}(S_A)
=\frac{2q^2\mu^2}{p^2}>0.}
$$

The extra term is precisely $\mu^2\operatorname{Var}(\Lambda)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Conditioning on the intensity in the [Poisson mixture](../../../discrete-probability-distribution.md#poisson-mixture) gives

$$
G_N(z)=\mathbb E[e^{\Lambda(z-1)}]
=\left(\frac{p}{1-qz}\right)^2.
$$

Thus $N$ has the [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) with two successes and success probability $p$, counting failures; explicitly $\mathbb P(N=j)=(j+1)p^2q^j$ for $j\geq0$. The [probability generating function](../../../probability-theory.md#probability-generating-function) is finite for real $z<1/q$.

The claim-size [moment-generating function](../../../probability-theory.md#moment-generating-function) is $M_X(t)=(1-\mu t)^{-1}$. Substituting into the aggregate [moment-generating function](../../../probability-theory.md#moment-generating-function) and using $p+q=1$ gives

$$
\boxed{M_S(t)=\left(\frac{p(1-\mu t)}{p-\mu t}\right)^2},
\qquad t<\frac p\mu.
$$

Put $L(t)=p/(p-\mu t)$, the [moment-generating function](../../../probability-theory.md#moment-generating-function) of an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with rate $p/\mu$. The identity

$$
\frac{p(1-\mu t)}{p-\mu t}=p+qL(t)
$$

then yields

$$
M_S(t)=p^2+2pqL(t)+q^2L(t)^2.
$$

The [gamma-mixed Poisson aggregate with exponential claims](../../../actuarial-statistics.md#gamma-mixed-poisson-aggregate-with-exponential-claims) has three nonnegative [mixture weights](../../../statistical-modelling.md#mixture-weight) summing to one. By uniqueness of the [moment-generating function](../../../probability-theory.md#moment-generating-function) near zero, **the aggregate distribution is**

$$
\boxed{\mathcal L(S)=p^2\delta_0+
2pq\,\operatorname{Exp}(p/\mu)+
q^2\,\operatorname{Gamma}(2,\text{rate }p/\mu).}
$$

Here $\delta_0$ is the [Dirac measure](../../../measure-theory.md#dirac-measure) at zero. In particular $\mathbb P(S=0)=p^2$, consistently with $\mathbb P(N=0)$. The positive components have respective [expected values](../../../probability-theory.md#expected-value) $\mu/p$ and $2\mu/p$; their [mixture distribution](../../../probability-theory.md#mixture-distribution) accounts for the possibility of no aggregate payout.

## 2

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For [quota share reinsurance](../../../actuarial-statistics.md#quota-share-reinsurance), each claim and therefore its aggregate are retained in the same proportion. For [aggregate stop loss reinsurance](../../../actuarial-statistics.md#aggregate-stop-loss-reinsurance), the insurer pays the aggregate up to the retention, and the reinsurer pays the excess. Thus **the insurer's payouts are**

$$
\boxed{S_I^*=\alpha S,\qquad \widetilde S_I=\min(S,M)
=S-(S-M)_+.}
$$

The subscript $+$ denotes the [positive part](../../../function.md#positive-part-of-a-real-valued-function). The stop loss contract here applies to the annual aggregate, rather than separately to each claim.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [expected value](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) under [quota share reinsurance](../../../actuarial-statistics.md#quota-share-reinsurance) follow by scaling the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution):

$$
\boxed{\mathbb E S_I^*=\alpha\mu_S,\qquad
\operatorname{Var}(S_I^*)=\alpha^2\mu_S^2.}
$$

The [retained stop loss moments for an exponential aggregate](../../../actuarial-statistics.md#retained-stop-loss-moments-for-an-exponential-aggregate) follow from the payout $Y=\min(S,M)$, its [survival function](../../../survival-analysis.md#survival-function) equals $e^{-x/\mu_S}$ for $0\leq x<M$ and zero for $x\geq M$. The [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments) gives, with $m=M/\mu_S$ and $r=e^{-m}$,

$$
\mathbb EY=\int_0^M e^{-x/\mu_S}\,dx=\mu_S(1-r),
\qquad
\mathbb EY^2=2\int_0^M xe^{-x/\mu_S}\,dx
=2\mu_S^2[1-(1+m)r].
$$

Consequently **the retained moments are**

$$
\boxed{\mathbb E\widetilde S_I=\mu_S(1-e^{-M/\mu_S}),\qquad
\operatorname{Var}(\widetilde S_I)
=\mu_S^2[1-2(M/\mu_S)e^{-M/\mu_S}-e^{-2M/\mu_S}].}
$$

Matching the two [expected values](../../../probability-theory.md#expected-value) forces $\alpha=1-r$, which lies strictly between zero and one. The difference of the [variances](../../../variance.md) simplifies to

$$
\boxed{\operatorname{Var}(S_I^*)-\operatorname{Var}(\widetilde S_I)
=2\mu_S^2e^{-M/\mu_S}
\left(\frac M{\mu_S}-1+e^{-M/\mu_S}\right)\geq0.}
$$

Indeed $h(m)=m-1+e^{-m}$ has $h(0)=0$ and $h'(m)=1-e^{-m}\geq0$ for $m\geq0$. Because $M>0$, the difference is actually positive. At equal retained [expected value](../../../probability-theory.md#expected-value), [aggregate stop loss reinsurance](../../../actuarial-statistics.md#aggregate-stop-loss-reinsurance) reduces the [variance](../../../variance.md) more than [quota share reinsurance](../../../actuarial-statistics.md#quota-share-reinsurance).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $Y=g(S)$ and $Z=\min(S,M)$. Their common [expected value](../../../probability-theory.md#expected-value) is $c$. Expanding about the retention gives **the requested variance identity**

$$
\mathbb E[(Y-M)^2]-(M-c)^2
=\mathbb E[Y^2]-2Mc+M^2-(M^2-2Mc+c^2)
=\boxed{\operatorname{Var}(Y)}.
$$

The [stop loss variance minimization principle](../../../actuarial-statistics.md#stop-loss-variance-minimization-principle) follows from a pointwise comparison. For $0\leq x\leq M$, the constraint $0\leq g(x)\leq x$ implies

$$
|g(x)-M|=M-g(x)\geq M-x
=|\min(x,M)-M|.
$$

For $x>M$, the squared distance of $\min(x,M)=M$ from $M$ is zero, so the same squared-distance comparison is immediate. Therefore

$$
\mathbb E[(Y-M)^2]\geq\mathbb E[(Z-M)^2].
$$

Subtracting the same $(M-c)^2$ proves **optimality of the retained stop loss payout**:

$$
\boxed{\operatorname{Var}(g(S))\geq
\operatorname{Var}(\min(S,M)).}
$$

Since $Z$ is bounded, its [variance](../../../variance.md) is finite; if $\mathbb E[Y^2]=\infty$, the inequality remains valid with infinite [variance](../../../variance.md) on the left. When it is finite, equality requires $g(S)=\min(S,M)$ almost surely, because the pointwise squared-distance inequality is strict whenever the two payouts differ.

## 3

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $c_{\rm prem}$ for the premium income rate, reserving $c$ later for the smaller exponential decay rate. In the [classical risk model](../../../actuarial-statistics.md#classical-risk-model), the surplus is

$$
U_t=u+c_{\rm prem}t-\sum_{j=1}^{N_t}X_j,
\qquad c_{\rm prem}=(1+\rho)\lambda\mu.
$$

Here $\rho$ is the [relative safety loading](../../../actuarial-statistics.md#relative-safety-loading). The aggregate claims form a [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process). Define $L_t=\sum_{j=1}^{N_t}X_j-c_{\rm prem}t$, so ruin occurs when $L_t>u$. By [independent increments](../../../stochastic-process.md#independent-increments) and the [exponential formula for a marked Poisson sum](../../../probability-theory.md#exponential-formula-for-a-marked-poisson-sum),

$$
\mathbb E[e^{R(L_t-L_s)}]
=\exp\{(t-s)[\lambda(M(R)-1)-c_{\rm prem}R]\}=1.
$$

Thus $Z_t=e^{RL_t}$ is a nonnegative [continuous-time martingale](../../../martingale.md#continuous-time-martingale) with $Z_0=1$, because the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) makes the exponent vanish.

Let $\tau=\inf\{t:U_t<0\}$. Apply the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the bounded [stopping time](../../../martingale.md#stopping-time) $\tau\wedge T$. On $\{\tau\leq T\}$, $L_\tau>u$, so

$$
1=\mathbb E[Z_{\tau\wedge T}]
\geq e^{Ru}\mathbb P(\tau\leq T).
$$

Letting $T$ increase proves **the Lundberg inequality and the unscaled limit**:

$$
\boxed{\psi(u)\leq e^{-Ru},\qquad
\lim_{u\to\infty}\psi(u)=0.}
$$

For the precise asymptotic, put

$$
h=\frac{\lambda\mu}{c_{\rm prem}}=\frac1{1+\rho},\quad
z(u)=e^{Ru}\psi(u),\quad
k(x)=h e^{Rx}f_I(x),\quad
g(u)=h e^{Ru}\int_u^\infty f_I(x)\,dx.
$$

The given exponential integral identity makes $k$ a probability density. Multiplying the given [defective renewal equation](../../../probability-theory.md#defective-renewal-equation) by $e^{Ru}$ turns it into the ordinary [renewal equation](../../../probability-theory.md#renewal-equation)

$$
z(u)=g(u)+\int_0^u z(u-x)k(x)\,dx.
$$

For clarity, the version of the [key renewal theorem](../../../probability-theory.md#key-renewal-theorem) used here is: if the interarrival law is nonarithmetic, has mean $m_k\in(0,\infty)$, and $g$ is [directly Riemann integrable](../../../real-analysis.md#direct-riemann-integrability), the locally bounded solution of this [renewal equation](../../../probability-theory.md#renewal-equation) satisfies $z(u)\to m_k^{-1}\int_0^\infty g(v)\,dv$. The infinite-mean version gives zero for nonnegative [directly Riemann integrable](../../../real-analysis.md#direct-riemann-integrability) $g$.

All the hypotheses can be checked here. The density $k$ gives a [nonarithmetic distribution](../../../probability-theory.md#nonarithmetic-distribution). The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
\int_0^\infty g(u)\,du
=h\int_0^\infty f_I(x)\frac{e^{Rx}-1}{R}\,dx
=\frac{1-h}{R}.
$$

Furthermore

$$
g(u)=\int_u^\infty e^{-R(x-u)}k(x)\,dx,\qquad
g'(u)=Rg(u)-k(u)\quad\hbox{almost everywhere}.
$$

Thus $g$ is continuous and integrable, and $\int_0^\infty|g'(u)|\,du\leq R\int g+1<\infty$. On a mesh of width $\delta$, the difference between its upper and lower sums is at most $\delta\int|g'|$; its upper sum is at most $\int g+\delta\int|g'|$. This proves [direct Riemann integrability](../../../real-analysis.md#direct-riemann-integrability) rather than assuming it. Also $0\leq z(u)\leq1$ by the [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality), so the solution is locally bounded. Its [renewal representation](../../../probability-theory.md#renewal-representation) is $z=g*U_k$, where $U_k=\sum_{j\geq0}K^{*j}$ and $K(dx)=k(x)\,dx$; the residual after iteration tends to zero on compact intervals because sums of positive interarrivals tend to infinity.

Writing $J=\int_0^\infty xe^{Rx}f_I(x)\,dx$, the tilted interarrival [expected value](../../../probability-theory.md#expected-value) is $m_k=hJ$. The [key renewal theorem](../../../probability-theory.md#key-renewal-theorem) gives **the [Cramér–Lundberg ruin asymptotic](../../../actuarial-statistics.md#cramer-lundberg-ruin-asymptotic)**

$$
\boxed{\lim_{u\to\infty}e^{Ru}\psi(u)
=\frac{1-h}{RhJ}
=\frac{\rho}{R\displaystyle\int_0^\infty xe^{Rx}f_I(x)\,dx}=A.}
$$

If $J=\infty$, the same formula is interpreted as $A=0$. A positive finite asymptotic constant requires $J<\infty$; this extra integrability is not explicitly stated in the paper.

For the final two-exponential case, evaluate the [defective renewal equation](../../../probability-theory.md#defective-renewal-equation) at zero:

$$
h=\psi(0)=a+b,\qquad
\boxed{\rho=\frac{1-a-b}{a+b}}.
$$

One can identify the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) without silently assuming $A>0$. For $0<r<c$, set

$$
P(r)=\int_0^\infty e^{ru}\psi(u)\,du
=\frac{a}{c-r}+\frac{b}{d-r}.
$$

It is finite and positive. Integrating the nonnegative terms of the [defective renewal equation](../../../probability-theory.md#defective-renewal-equation), using the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), first shows that $F_I(r)=\int_0^\infty e^{rx}f_I(x)\,dx$ is finite and then gives

$$
P(r)=\frac h r[F_I(r)-1]+hP(r)F_I(r),
\qquad
hF_I(r)=\frac{h+rP(r)}{1+rP(r)}.
$$

As $r\uparrow c$, $P(r)\to\infty$ because $a>0$. By [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem), $hF_I(c)=1$. The [integrated tail distribution](../../../probability-theory.md#integrated-tail-distribution) in the [classical risk model](../../../actuarial-statistics.md#classical-risk-model) has density $f_I(x)=\mathbb P(X_1>x)/\mu$, so $F_I(r)=[M(r)-1]/(\mu r)$ by the [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments). Hence $c$ solves the adjustment equation, and its stipulated uniqueness implies $R=c$. Finally the displayed form of $\psi$ gives **the remaining constants**

$$
\boxed{R=c,\qquad A=a,\qquad \rho=\frac{1-a-b}{a+b}.}
$$

In particular the decay exponent $d$ and the coefficient $b$ do not affect $R$ or $A$. The $c$ in these final answers is the printed decay rate, not $c_{\rm prem}$.

## 4

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In the [Bühlmann model](../../../actuarial-statistics.md#buhlmann-model), a latent risk parameter $\Theta$ is drawn from a population distribution. Conditional on $\Theta$, the yearly observations are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables), with [conditional expectation](../../../measure-theory.md#conditional-expectation) $m(\Theta)$ and [conditional variance](../../../variance.md#conditional-variance) $v(\Theta)$. Define the structural parameters

$$
m=\mathbb E[m(\Theta)],\qquad
v=\mathbb E[v(\Theta)],\qquad
a=\operatorname{Var}(m(\Theta)).
$$

Here $v$ is the [expected process variance](../../../actuarial-statistics.md#expected-process-variance), while $a$ is the [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means). The [Bühlmann credibility premium](../../../actuarial-statistics.md#buhlmann-credibility-premium) is the best affine estimate of $m(\Theta)$ from the observed claims, under [mean squared error](../../../statistical-modelling.md#mean-squared-error). Predicting the next claim gives the same affine estimate: the extra conditional observation noise contributes the constant $v$ to the prediction error.

The [law of total variance](../../../probability-theory.md#law-of-total-variance) and [conditional independence](../../../random-variable.md#conditional-independence) give

$$
\operatorname{Var}(X_j)=a+v,\qquad
\operatorname{Cov}(X_i,X_j)=a\quad(i\ne j),\qquad
\operatorname{Cov}(m(\Theta),X_j)=a.
$$

An affine estimate can be written as $\widehat m=m+\sum_{j=1}^n b_j(X_j-m)$: for any chosen $b_j$, optimizing the constant makes its [expected value](../../../probability-theory.md#expected-value) equal to $m$. The normal equations for the [linear least-squares projection](../../../probability-and-statistics.md#linear-least-squares-projection) are

$$
v b_i+a\sum_{j=1}^n b_j=a,\qquad i=1,\ldots,n.
$$

For $v>0$ they force all $b_i$ to agree, with $b_i=a/(v+na)$. Thus **the credibility factor and premium are**

$$
\boxed{Z=\frac{na}{v+na}=\frac{n}{n+v/a},\qquad
\widehat m=Z\overline X+(1-Z)m,}
\qquad \overline X=\frac1n\sum_{j=1}^nX_j.
$$

The [credibility factor](../../../actuarial-statistics.md#credibility-factor) increases with the observation count and between-risk [variance](../../../variance.md), and decreases with within-risk [variance](../../../variance.md). If $a=0$, the risk mean is known and $Z=0$; if $v=0$ and $a>0$, one observation reveals it and $Z=1$. If both vanish, the premium is the fixed value $m$ and the factor is immaterial.

In the specified model, the conditional law is a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $\alpha$ and scale $\theta$. Therefore

$$
m(\theta)=\alpha\theta,\qquad v(\theta)=\alpha\theta^2.
$$

The prior is an [inverse-gamma distribution](../../../continuous-probability-distribution.md#inverse-gamma-distribution) with shape $k$ and scale $\lambda$. To obtain its moments directly, substitute $y=\lambda/\theta$ in the defining integral, obtaining

$$
\mathbb E[\Theta^r]
=\lambda^r\frac{\Gamma(k-r)}{\Gamma(k)},\qquad r<k.
$$

The [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) yields

$$
\mathbb E\Theta=\frac{\lambda}{k-1},\qquad
\mathbb E\Theta^2=\frac{\lambda^2}{(k-1)(k-2)},\qquad
\operatorname{Var}(\Theta)=\frac{\lambda^2}{(k-1)^2(k-2)}.
$$

The assumption $k>2$ makes both structural [variances](../../../variance.md) finite. Hence

$$
m=\frac{\alpha\lambda}{k-1},\qquad
v=\frac{\alpha\lambda^2}{(k-1)(k-2)},\qquad
a=\frac{\alpha^2\lambda^2}{(k-1)^2(k-2)},\qquad
\frac va=\frac{k-1}{\alpha}.
$$

It follows that **the model-specific credibility estimate is**

$$
\boxed{Z=\frac{n\alpha}{n\alpha+k-1},\qquad
\widehat m_{\rm B}
=Z\overline X+(1-Z)\frac{\alpha\lambda}{k-1}
=\frac{\alpha(\lambda+\sum_{j=1}^nX_j)}{k+n\alpha-1}.}
$$

For the [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss), the quantity to estimate is $\alpha\Theta$, so the optimum is its [posterior mean](../../../statistical-inference.md#posterior-mean). The [likelihood function](../../../statistical-modelling.md#likelihood-function), viewed as a function of $\theta$, is proportional to

$$
\theta^{-n\alpha}\exp\left(-\frac{\sum_jx_j}{\theta}\right).
$$

Multiplication by the prior shows [gamma scale inverse-gamma conjugacy](../../../exponential-family.md#gamma-scale-inverse-gamma-conjugacy):

$$
\Theta\mid x_1,\ldots,x_n
\sim\operatorname{InvGamma}\left(k+n\alpha,\lambda+\sum_jx_j\right).
$$

Although the printed hint only mentions integer shapes, the same substitution and [Gamma integral](../../../complex-analysis.md#gamma-integral) normalize this posterior for every positive real shape, so no integrality of $\alpha$ is needed. Its [posterior mean](../../../statistical-inference.md#posterior-mean) gives **the Bayesian estimate and comparison**

$$
\boxed{\widehat m_{\rm Bayes}
=\alpha\mathbb E[\Theta\mid X_1,\ldots,X_n]
=\frac{\alpha(\lambda+\sum_{j=1}^nX_j)}{k+n\alpha-1}
=\widehat m_{\rm B}.}
$$

This [exact Bühlmann credibility for gamma claims](../../../exponential-family.md#exact-buhlmann-credibility-for-gamma-claims) holds for every observed sample, not merely on average. Here the [posterior mean](../../../statistical-inference.md#posterior-mean) is affine in the [sample mean](../../../variance.md#sample-mean), so the best affine [Bühlmann credibility premium](../../../actuarial-statistics.md#buhlmann-credibility-premium) is also the unrestricted [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
