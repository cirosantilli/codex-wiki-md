# Paper 216

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_216.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_216.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $a=y_4$ and $b=y_2+y_3$. Dropping factors independent of $\theta$, the [multinomial likelihood](../../../discrete-probability-distribution.md#multinomial-likelihood) and [uniform prior](../../../statistical-inference.md#uniform-prior) give the [posterior density](../../../statistical-inference.md#posterior-density)

$$
\pi(\theta\mid y)\propto(2+\theta)^{y_1}\theta^a(1-\theta)^b\mathbf1_{(0,1)}(\theta).
$$

Multiplying this by the stipulated [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) for the [latent variable](../../../statistical-modelling.md#latent-variable) cancels the factor $(2+\theta)^{y_1}$:

$$
\pi(\theta,z\mid y)\propto\binom{y_1}{z}2^{y_1-z}\theta^{a+z}(1-\theta)^b,
\qquad 0\leq z\leq y_1.
$$

Consequently the two [full conditional distributions](../../../probability-theory.md#full-conditional-distribution) are

$$
\boxed{Z\mid\theta,y\sim\operatorname{Binomial}\!\left(y_1,\frac{\theta}{2+\theta}\right),\qquad
\theta\mid Z=z,y\sim\operatorname{Beta}(a+z+1,b+1).}
$$

Start with $0<\theta_0<1$, sample $Z$ from its [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution), then sample a new $\theta$ from its [Beta distribution](../../../probability-theory.md#beta-distribution), and repeat. The [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) can be sampled by adding $y_1$ independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution). For the [Beta distribution](../../../probability-theory.md#beta-distribution), take independent $A\sim\operatorname{Gamma}(a+z+1,1)$ and $B\sim\operatorname{Gamma}(b+1,1)$ and return $A/(A+B)$; integer-shape [gamma distributions](../../../continuous-probability-distribution.md#gamma-distribution) are sums of independent unit-rate [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution). Both shapes are positive even when some observed counts vanish.

Each [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) update preserves the augmented [posterior distribution](../../../statistical-inference.md#bayesian-posterior), so its $\theta$ [marginal distribution](../../../probability-theory.md#marginal-distribution) is the required [posterior distribution](../../../statistical-inference.md#bayesian-posterior). The positive [full conditional distributions](../../../probability-theory.md#full-conditional-distribution) on the interior allow exploration of the entire support. These iterates are generally dependent; they are not the independent exact draws constructed in the later parts.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[Adaptive rejection sampling](../../../probability-and-statistics.md#adaptive-rejection-sampling) is exact [rejection sampling](../../../probability-and-statistics.md#rejection-sampling) for a differentiable [log-concave probability density](../../../continuous-probability-distribution.md#log-concave-probability-density). Given interior evaluation points $s_j$, construct the upper envelope

$$
u(x)=\min_j\{\ell(s_j)+\ell'(s_j)(x-s_j)\},\qquad \ell(x)=\log h(x),
$$

where $h$ is the unnormalized target [probability density function](../../../continuous-probability-distribution.md#probability-density-function). The [concave function](../../../real-analysis.md#concave-function) $\ell$ lies below all its [tangent lines](../../../calculus.md#tangent-line), so $e^u\geq h$. Interpolation between adjacent evaluation points gives a lower envelope $l\leq\ell$ there, allowing a squeeze test. The normalized upper envelope $g=e^u/\int e^u$ is a piecewise exponential [proposal distribution](../../../statistical-inference.md#proposal-distribution).

Draw $X\sim g$ and an independent $W$ from the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution), and accept when $W\leq e^{\ell(X)-u(X)}$. A squeeze test $W\leq e^{l(X)-u(X)}$ can establish acceptance without evaluating $\ell(X)$. Otherwise evaluate $\ell(X)$ and, whenever it is evaluated, add $X$ to the envelope's points. Repeat until acceptance. On each linear piece $u(x)=r x+s$, its [integral](../../../calculus.md#integral) is $e^s(e^{r d}-e^{r c})/r$ on $[c,d]$, with value $e^s(d-c)$ when $r=0$. These [integrals](../../../calculus.md#integral) select a piece; [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) samples within it.

Here, with $a=y_4$ and $b=y_2+y_3$, the [log-posterior](../../../statistical-inference.md#log-posterior) on $(0,1)$ has

$$
\ell(\theta)=y_1\log(2+\theta)+a\log\theta+b\log(1-\theta),\qquad
\boxed{\ell''(\theta)=-\frac{y_1}{(2+\theta)^2}-\frac{a}{\theta^2}-\frac{b}{(1-\theta)^2}\leq0.}
$$

Choose evaluation points strictly inside $(0,1)$, avoiding any endpoint singularities of the [logarithm](../../../calculus.md#logarithm). Every finite set of [tangent lines](../../../calculus.md#tangent-line) gives a finite upper-envelope [integral](../../../calculus.md#integral) on this bounded interval; slope conditions needed for unbounded supports are unnecessary. When $N=0$ the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is simply the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) and may be sampled directly.

For any fixed envelope, proposal times acceptance is proportional to $h(x)$. Conditional on all past evaluations and rejections, the next accepted value therefore has the same normalized [posterior density](../../../statistical-inference.md#posterior-density). To see that adaptation does not spoil this, at every attempted draw its accepted mass is a scalar times that fixed [posterior density](../../../statistical-inference.md#posterior-density); summing over possible rejection histories preserves it. The acceptance [probability](../../../probability-theory.md#probability) stays bounded below by its positive initial-envelope value because insertion only lowers the upper envelope. Thus acceptance occurs almost surely. With fresh independent randomness, successive accepted values are **exact [independent](../../../random-variable.md#independent-random-variables) samples from the [posterior distribution](../../../statistical-inference.md#bayesian-posterior)**, even when the envelope is retained and improved between them.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

An exact finite [mixture model](../../../statistical-modelling.md#mixture-model) follows from the [binomial theorem](../../../combinatorics.md#binomial-theorem):

$$
(2+\theta)^{y_1}\theta^a(1-\theta)^b
=\sum_{z=0}^{y_1}\binom{y_1}{z}2^{y_1-z}\theta^{a+z}(1-\theta)^b,
\qquad a=y_4,\quad b=y_2+y_3.
$$

Define positive [mixture weights](../../../statistical-modelling.md#mixture-weight)

$$
w_z=\frac{\binom{y_1}{z}2^{y_1-z}B(a+z+1,b+1)}{
\sum_{j=0}^{y_1}\binom{y_1}{j}2^{y_1-j}B(a+j+1,b+1)}.
$$

Here $B$ is the [Beta function](../../../complex-analysis.md#beta-function), so the component [probability distributions](../../../probability-theory.md#probability-distribution) are $\operatorname{Beta}(a+z+1,b+1)$. All coefficients are computable from the observed integer counts.

Use [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) with the supplied $U$ to choose $Z$: writing $C_{-1}=0$ and $C_z=\sum_{j=0}^zw_j$, take $C_{Z-1}\leq U<C_Z$. Then recycle its position inside that interval,

$$
V=\frac{U-C_{Z-1}}{w_Z}.
$$

[Recycling a uniform random variable after discrete sampling](../../../probability-theory.md#recycling-a-uniform-random-variable-after-discrete-sampling) makes $V$ uniform independently of $Z$, since $\Pr(Z=z,V\leq v)=w_zv$. It is also independent of all supplied [random variables](../../../random-variable.md) with [gamma distributions](../../../continuous-probability-distribution.md#gamma-distribution). Transform these by the [probability integral transform](../../../probability-theory.md#probability-integral-transform):

$$
W_i=1-e^{-G_i},\qquad 1\leq i\leq N.
$$

They are independent [random variables](../../../random-variable.md) with [uniform distributions](../../../continuous-probability-distribution.md#continuous-uniform-distribution) because $G_i$ has a unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution).

Conditional on $Z=z$, put $k=a+z+b+1$ and $r=a+z+1$. Form the $k$ values $V,W_1,\ldots,W_{k-1}$ and return their $r$th [order statistic](../../../probability-theory.md#order-statistic). This uses at most the supplied $N$ [random variables](../../../random-variable.md) with [gamma distributions](../../../continuous-probability-distribution.md#gamma-distribution), since $k-1=a+b+z\leq N$. The [uniform order statistic](../../../probability-theory.md#uniform-order-statistic) formula gives

$$
\boxed{\Theta=\operatorname{order}_r(V,W_1,\ldots,W_{k-1}),\qquad
\Theta\mid Z=z\sim\operatorname{Beta}(a+z+1,b+1).}
$$

Averaging these component [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) with weights $w_z$ recovers exactly the normalized [posterior density](../../../statistical-inference.md#posterior-density). Unused inputs can be discarded. When $N=0$, $Z=0$, $k=r=1$, and the output is $U$, as required. Interval endpoints and ties have [probability](../../../probability-theory.md#probability) zero; any consistent convention there is harmless. Exactness here concerns the mathematical algorithm; finite-precision arithmetic can be stabilized with logarithmic [mixture weights](../../../statistical-modelling.md#mixture-weight).

## 2

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $\mathcal E$ for the directed edges from parent to child and $x_v(i)$ for the state at site $i$. The [global Markov property for an undirected graph](../../../statistical-model.md#global-markov-property-for-an-undirected-graph) on this [tree](../../../combinatorics.md#tree-graph-theory), together with the specified parent transitions, gives the complete-data [likelihood function](../../../statistical-modelling.md#likelihood-function)

$$
p_K(x)=4^{-k}\prod_{(v,w)\in\mathcal E}\prod_{i=1}^kK(x_v(i),x_w(i)).
$$

One can obtain the factorization by successively removing terminal subtrees: after conditioning on their parent, each subtree is independent of the rest. The root factor and transition products also show that different sites are independent. Only ancestral states are [latent variables](../../../statistical-modelling.md#latent-variable).

At the current [Markov kernel](../../../markov-process.md#markov-kernel) $K^{(o)}$, define expected transition counts

$$
N_{ab}=\sum_{i=1}^k\sum_{(v,w)\in\mathcal E}
\Pr_{K^{(o)}}(X_v(i)=a,X_w(i)=b\mid\text{observed leaves}).
$$

The E-step of the [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) is

$$
Q(K\mid K^{(o)})=\text{constant}+\sum_{a,b}N_{ab}\log K(a,b).
$$

Maximize separately for each row under $K(a,b)\geq0$ and $\sum_bK(a,b)=1$. For $N_a=\sum_bN_{ab}>0$, the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equation is $N_{ab}/K(a,b)=N_a$, with zero-count entries set to zero at a boundary maximum. Thus the [EM transition-count update on a tree](../../../statistical-modelling.md#em-transition-count-update-on-a-tree) is

$$
\boxed{K^{\mathrm{new}}(a,b)=\frac{N_{ab}}{\sum_cN_{ac}}.}
$$

If $N_a=0$, that row does not occur in $Q$; any row [probability distribution](../../../probability-theory.md#probability-distribution), including its previous value, maximizes the objective.

The expected counts can be computed exactly by the [Felsenstein pruning algorithm](../../../biology.md#felsenstein-pruning-algorithm) and an outward [belief propagation](../../../statistical-model.md#belief-propagation) pass. For one site, let $L_v(a)$ be the [conditional probability](../../../probability-theory.md#conditional-probability) of observations in the subtree below $v$, given state $a$. For a leaf $v$ with observed state $d_v$, $L_v(a)=\mathbf1_{\{a=d_v\}}$. For an internal vertex,

$$
L_v(a)=\prod_{w\text{ child of }v}\sum_bK^{(o)}(a,b)L_w(b),\qquad
Z_i=\frac14\sum_a L_{v_0}(a).
$$

Define $A_v(a)$ as the joint mass of state $a$ at $v$ and all observations outside its subtree. The root has $A_{v_0}(a)=1/4$. For a child $w$ of $v$, put

$$
S_{vw}(a)=\prod_{u\text{ child of }v,\ u\ne w}\sum_cK^{(o)}(a,c)L_u(c),\qquad
A_w(b)=\sum_a A_v(a)S_{vw}(a)K^{(o)}(a,b).
$$

The edge [posterior probability](../../../statistical-inference.md#posterior-probability) required above is

$$
\xi_{vw}^{(i)}(a,b)=\frac{A_v(a)S_{vw}(a)K^{(o)}(a,b)L_w(b)}{Z_i}.
$$

Multiply the inside and outside factors to obtain the joint mass of the observations and endpoint states; division by the site [likelihood function](../../../statistical-modelling.md#likelihood-function) proves this expression. Sum $\xi$ over edges and sites to form $N_{ab}$. The two passes take $O(k|\mathcal E|4^2)=O(kn)$ operations on a binary [tree](../../../combinatorics.md#tree-graph-theory). Scaling messages or computing them logarithmically avoids underflow.

A strictly positive initial [Markov kernel](../../../markov-process.md#markov-kernel) ensures $Z_i>0$ for every observed leaf pattern, so every E-step is defined. At a later boundary iterate, require positive likelihood for the actual data and restrict the [conditional distribution](../../../probability-theory.md#conditional-distribution) to its support. [EM likelihood monotonicity](../../../statistical-modelling.md#em-likelihood-monotonicity) proves that the update cannot decrease observed-data [likelihood function](../../../statistical-modelling.md#likelihood-function). It is a maximum-likelihood iteration, not a guarantee of finding the global [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator); different initial kernels may lead to different stationary points.

## 3

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the shape-rate convention for every [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution), with $a,c>0$. Let $A_i=a+y_i$ and $s=\sum_i\theta_i$. The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) likelihood and the [Gamma–Poisson hierarchical model](../../../statistical-inference.md#gamma-poisson-hierarchical-model) give

$$
\pi(\theta,b\mid y)\propto
b^{na+c-1}e^{-b(1+s)}\prod_{i=1}^n\theta_i^{A_i-1}e^{-t_i\theta_i},
\qquad b>0,\ \theta_i>0.
$$

All factors involving the coordinate being updated must be retained, including $b^{na}$ from the conditional [gamma distributions](../../../continuous-probability-distribution.md#gamma-distribution). The [full conditional distributions](../../../probability-theory.md#full-conditional-distribution) are

$$
\boxed{\theta_i\mid b,y\sim\operatorname{Gamma}(A_i,b+t_i)\quad\text{independently},\qquad
b\mid\theta,y\sim\operatorname{Gamma}(na+c,1+s).}
$$

For a [blocked Gibbs sampler](../../../statistical-inference.md#blocked-gibbs-sampler), draw $b$ from the second [full conditional distribution](../../../probability-theory.md#full-conditional-distribution), then redraw all the $\theta_i$ independently from the first ones. Repeating these two steps preserves the joint [posterior distribution](../../../statistical-inference.md#bayesian-posterior); observing $\theta$ after each complete sweep gives the [Markov chain](../../../markov-process.md#markov-chain) used in the next part. Standard [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) sampling works for noninteger as well as integer shapes. The positive observation-period convention $t_i>0$ is used for the subsequent [geometric drift condition](../../../statistical-inference.md#geometric-drift-condition).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Take observation periods to have positive lengths $t_i>0$, and let $P$ be the [Markov kernel](../../../markov-process.md#markov-kernel) of a sweep which first draws $b$ given the current $\theta$ and then draws the new vector $\Theta'$. Write $A_i=a+y_i$. Conditional on $b$, [independence](../../../random-variable.md#independent-random-variables) and the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) mean and [variance](../../../variance.md) give

$$
\mathbb E\!\left[\left(\sum_i\Theta_i'\right)^2\Bigm|b\right]
=\left(\sum_i\frac{A_i}{b+t_i}\right)^2+
\sum_i\frac{A_i}{(b+t_i)^2}
\leq\left(\sum_i\frac{A_i}{t_i}\right)^2+\sum_i\frac{A_i}{t_i^2}=:D.
$$

Averaging over the [full conditional distribution](../../../probability-theory.md#full-conditional-distribution) of $b$ preserves this bound, uniformly in the current state. Therefore $PV(\theta)\leq M:=1+D<\infty$. This is the mechanism in [bounded conditional moments imply a geometric drift](../../../statistical-inference.md#bounded-conditional-moments-imply-a-geometric-drift).

Choose $0<\rho<1$, $R>M/\rho$, and $C=\{\theta:V(\theta)\leq R\}$. Outside $C$, $PV\leq M<\rho V$; inside $C$, $PV\leq M\leq\rho V+M$. Hence

$$
\boxed{PV(\theta)\leq\rho V(\theta)+M\mathbf1_C(\theta),\qquad 0<\rho<1.}
$$

For completeness, $C$ is a [small set](../../../statistical-inference.md#small-set), even though it approaches the boundary of the positive orthant. Choose $\delta>0$ small enough that $B=[\delta,2\delta]^n\subset C$. On $C$, $s=\sum_i\theta_i\leq\sqrt{R-1}$. The conditional [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) of $b$ has fixed shape $na+c$ and rate $1+s$ in a compact positive interval. Its [probability density function](../../../continuous-probability-distribution.md#probability-density-function) therefore has a positive common lower bound on $b\in[1,2]$. For those $b$, the product [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of $\Theta'$ similarly has a positive common lower bound on $B$, since every shape is positive and every rate $b+t_i$ lies in a compact positive interval. Integrating over $b\in[1,2]$ gives $P(\theta,\cdot)\geq\varepsilon\eta(\cdot)$ on $C$, where $\eta$ is the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $B$ and $\varepsilon>0$.

The transition [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is positive throughout the positive orthant, giving an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain). Since $B\subset C$, the box minorization includes starts in the same box, which gives an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain). The proper [prior distributions](../../../statistical-inference.md#prior-probability) and bounded [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) likelihood have positive finite evidence, so the invariant [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is proper. Together with the [geometric drift condition](../../../statistical-inference.md#geometric-drift-condition), these hypotheses imply [geometric ergodicity](../../../statistical-inference.md#geometric-ergodicity). In particular, the argument proves the required drift rather than assuming that every [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) is geometrically ergodic.

The positive-period convention matters. If zero lengths are allowed, the printed assertion can fail: take $n=1$, $a=c=1$, $t_1=y_1=0$. Then $b\mid\theta\sim\operatorname{Gamma}(2,1+\theta)$ and $\Theta'\mid b\sim\operatorname{Gamma}(1,b)$, so

$$
\mathbb E[(\Theta')^2\mid\theta]=2\mathbb E[b^{-2}\mid\theta]=\infty.
$$

This example has a proper [posterior distribution](../../../statistical-inference.md#bayesian-posterior) but cannot satisfy a finite quadratic [geometric drift condition](../../../statistical-inference.md#geometric-drift-condition). Thus the proof establishes the intended claim for positive observation periods, not an unrestricted extension to zero exposure.

## 4

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $\pi(x)=\mu(x\mid y)$. [Mean-field variational inference](../../../statistical-inference.md#mean-field-variational-inference) minimizes the reverse [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence)

$$
\operatorname{KL}(q\Vert\pi)=\int q(x)\log\frac{q(x)}{\pi(x)}\,dx,
\qquad q(x)=\prod_{i=1}^pq_i(x_i),\quad \int q_i=1.
$$

Each $q_i$ is a [probability density function](../../../continuous-probability-distribution.md#probability-density-function); without further parametric restrictions, the optimization is over all such product [probability distributions](../../../probability-theory.md#probability-distribution). Equivalently it maximizes the [evidence lower bound](../../../statistical-inference.md#evidence-lower-bound) $\mathbb E_q[\log h(X)-\log q(X)]$ for any unnormalized [posterior density](../../../statistical-inference.md#posterior-density) $h$. Its difference from $\log\int h$ is exactly the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence).

Fix $q_2,\ldots,q_p$ and write

$$
F(x_1)=\mathbb E_{q_{-1}}[\log\pi(x_1,X_{-1})],\qquad
Z_1=\int e^{F(u)}\,du.
$$

Assume $0<Z_1<\infty$ and that the displayed [expected values](../../../probability-theory.md#expected-value) and objective decomposition are well defined. The optimal factor is

$$
\boxed{q_1^*(x_1)=\frac{\exp\{\mathbb E_{q_{-1}}[\log\pi(x_1,X_{-1})]\}}{Z_1}.}
$$

Indeed, the part of the objective depending on $q_1$ is

$$
\int q_1\log q_1-\int q_1F
=\operatorname{KL}(q_1\Vert q_1^*)-\log Z_1.
$$

The remaining term $\sum_{i=2}^p\int q_i\log q_i$ is fixed. [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) gives nonnegativity of the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence), with equality precisely at $q_1=q_1^*$ almost everywhere. This proves global optimality of that coordinate update; it does not assert global optimality of a sequence of coordinate updates for the full nonconvex product-family problem.

The printed upper index $k$ in the list of remaining coordinates is inconsistent with the dimension $p$; the natural interpretation is $k=p$. Also, if the exponential expression has zero or infinite [normalizing constant](../../../continuous-probability-distribution.md#normalizing-constant), or the [expected values](../../../probability-theory.md#expected-value) are undefined, the usual coordinate formula needs additional support or integrability hypotheses. A restricted parametric factor family need not contain this unrestricted optimal factor.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A counterexample can use an irreducible, aperiodic [reversible Markov chain](../../../markov-process.md#reversible-markov-chain), so failure is not caused by a pathological transition structure. Take two binary coordinates, enumerate the four states as $00,01,10,11$, and let $\pi$ be their [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution). Use the [Markov kernel](../../../markov-process.md#markov-kernel)

$$
K=\begin{pmatrix}
1/4&1/4&1/4&1/4\\
1/4&1/2&1/8&1/8\\
1/4&1/8&1/2&1/8\\
1/4&1/8&1/8&1/2
\end{pmatrix}.
$$

Its rows sum to one and it is symmetric, proving [detailed balance](../../../markov-process.md#detailed-balance) with $\pi$. Every entry is positive. Let the univariate parametric family be $\widetilde{\mathcal Q}=\{\operatorname{Bernoulli}(r):0\leq r\leq2/5\}$.

For a product initial [probability distribution](../../../probability-theory.md#probability-distribution) with parameters $r_1,r_2$, additivity of the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) gives

$$
\operatorname{KL}(\nu\Vert\pi)=\sum_{i=1}^2
\{r_i\log(2r_i)+(1-r_i)\log(2(1-r_i))\}.
$$

Each summand has [derivative](../../../calculus.md#derivative) $\log(r_i/(1-r_i))<0$ on $(0,2/5]$, so the unique optimum at $t=0$ has $r_1=r_2=2/5$. Thus

$$
q^{*0}=(9,6,6,4)/25,
\qquad Kq^{*0}=(25,26,26,23)/100.
$$

On the other hand the allowed initial [probability distribution](../../../probability-theory.md#probability-distribution) $\delta_{00}$, obtained with $r_1=r_2=0$, is sent by one step to $\pi$. Its [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) is zero, the smallest possible value. Consequently

$$
\boxed{q^{*1}=\pi\ne Kq^{*0}.}
$$

The transition reduces [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) for each input, but may reduce it by different amounts for different inputs. It therefore need not preserve the ordering of competing initial [probability distributions](../../../probability-theory.md#probability-distribution), which is exactly why [Markov chain variational inference](../../../statistical-inference.md#markov-chain-variational-inference) must optimize the initial parameters for its chosen number of steps.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Parameterize the initial product [normal distribution](../../../probability-theory.md#normal-distribution) by $\eta=(m,\rho)$, using

$$
X^{(0)}_\eta=m+\operatorname{diag}(e^{\rho_1},\ldots,e^{\rho_p})\varepsilon,
\qquad \varepsilon\sim N(0,I_p).
$$

Run the given recursion with independent [random variables](../../../random-variable.md) with [uniform distributions](../../../continuous-probability-distribution.md#continuous-uniform-distribution) to obtain $X_\eta=F_t(X^{(0)}_\eta,Z_{1:t})$. Because the noise laws do not depend on $\eta$, the [chain rule](../../../calculus.md#chain-rule) and [automatic differentiation](../../../calculus.md#automatic-differentiation) give [reparameterization gradients](../../../statistical-inference.md#reparameterization-gradient) through the entire simulated trajectory. The variational objective is $J(\eta)=\operatorname{KL}(q_\eta\Vert\pi)$, where $q_\eta=K^t\nu_\eta$ and $\pi=\mu(\cdot\mid y)$.

One must account for the output [differential entropy](../../../information-theory.md#differential-entropy), not just optimize $\mathbb E[\log\pi(X_\eta)]$. Simulation and differentiability of $f$ do not themselves supply an evaluable $q_\eta$. If $K$ retains the [reversible Markov chain](../../../markov-process.md#reversible-markov-chain) assumption from part (b), a concrete algorithm avoids a transition-density oracle using [reversible density-ratio propagation](../../../markov-process.md#reversible-density-ratio-propagation). Write $\pi=h/Z_\pi$, with $h$ an evaluable unnormalized [posterior density](../../../statistical-inference.md#posterior-density), and define

$$
A_\eta(x)=\mathbb E_{B\sim K^t(x,\cdot)}\left[\frac{\nu_\eta(B)}{h(B)}\right].
$$

[Detailed balance](../../../markov-process.md#detailed-balance) implies

$$
q_\eta(x)=h(x)A_\eta(x),\qquad
\boxed{J(\eta)=\log Z_\pi+\mathbb E[\log A_\eta(X_\eta)].}
$$

For example, integrate $\nu_\eta(b)K^t(b,dx)$ and replace $h(b)K^t(b,dx)$ by $h(x)K^t(x,db)$ to obtain the first identity. This also proves [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) of $K^t\nu_\eta$ with respect to $\pi$ when $\nu_\eta\ll\pi$. An everywhere finite differentiable [log-posterior](../../../statistical-inference.md#log-posterior) has positive density, so an ordinary product [normal distribution](../../../probability-theory.md#normal-distribution) has this domination.

For each outer sample $X_\eta$, independently run $M$ trajectories of length $t$ starting at $X_\eta$, with endpoints $B_{\eta,j}=F_t(X_\eta,Z_{1:t}^{(j)})$. These are reverse trajectories because of [detailed balance](../../../markov-process.md#detailed-balance); the same recursion simulates them. Estimate $A_\eta(X_\eta)$ by

$$
\widehat A_\eta(X_\eta)=\frac1M\sum_{j=1}^M
\frac{\nu_\eta(B_{\eta,j})}{h(B_{\eta,j})}.
$$

Average $\log\widehat A$ over an outer batch. Compute it stably by a logarithmic sum of exponentials. Differentiate through both outer and reverse trajectories and through the explicit product-normal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $\nu_\eta$. Only the given state [gradients](../../../calculus.md#gradient) of $f$ and $\log h$, together with elementary normal-density [derivatives](../../../calculus.md#derivative), are needed. Apply [stochastic gradient descent](../../../numerical-analysis.md#stochastic-gradient-descent) to $m$ and $\rho$, refreshing the independent noise batches. The logarithmic scale parameters keep all [variances](../../../variance.md) positive.

This is [nested Monte Carlo](../../../probability-and-statistics.md#nested-monte-carlo) optimization of the exact objective in the limit of adequately increasing inner and outer sample sizes. For fixed $M$, $\log\widehat A$ is generally biased, even though $\widehat A$ is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator). Finite logarithmic moments, suitable uniform integrability, and justified [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) are needed for consistency and [gradient](../../../calculus.md#gradient) interchange. Under those conditions increasing $M$ and controlling the optimization error yields a justified numerical approximation; nonconvexity prevents a generic guarantee of a global optimum.

There is a real assumption issue: part (c) redefines $K$ without explicitly restating reversibility. The algorithm above uses the reversible interpretation inherited from part (b). For an arbitrary differentiable recursion, one additionally needs access to output densities or a simulatable reverse kernel and regularity of the objective. Differentiability alone is insufficient: $f(x,z)=0$ is differentiable and, with a standard-normal target, makes $K^t\nu$ a point mass for $t\geq1$, so every candidate has infinite [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence). Thus a universal finite-objective algorithm cannot be justified solely from the literal differentiability assumptions. An invertible recursion with computable density transformations offers a different sufficient route, but invertibility is not stated here.

## 5

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The most plausible cause is **strong dependence between the [latent variables](../../../statistical-modelling.md#latent-variable) and [covariance](../../../variance.md#covariance) [hyperparameters](../../../statistical-inference.md#hyperparameter) in their joint [posterior distribution](../../../statistical-inference.md#bayesian-posterior)**. In the usual conditionally independent [Gaussian process classification](../../../stochastic-process.md#gaussian-process-classification) model, put $F=(f(x_1),\ldots,f(x_n))$, $w=\sigma^{-2}$, and $C=w^{-1}R_\tau$. The [probit regression](../../../statistical-modelling.md#probit-model) likelihood is $\ell(F)=\prod_i\Phi((2y_i-1)F_i)$, while $F\mid w,\tau$ has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) with [covariance matrix](../../../variance.md#covariance-matrix) $C$.

For distinct inputs and positive length scales, $R_\tau$ is positive definite. Its Gaussian [probability density function](../../../continuous-probability-distribution.md#probability-density-function) contributes

$$
p(F\mid w,\tau)\propto w^{n/2}|R_\tau|^{-1/2}
\exp\!\left(-\frac w2F^\top R_\tau^{-1}F\right).
$$

The unit-rate exponential [prior distribution](../../../statistical-inference.md#prior-probability) on $w$ therefore gives

$$
\boxed{w\mid F,\tau,y\sim\operatorname{Gamma}\!\left(1+\frac n2,\ 1+\frac12F^\top R_\tau^{-1}F\right).}
$$

Its scale is tightly tied to the current magnitude and shape of $F$. Changing $\tau$ changes the [eigenvectors](../../../linear-operator-theory.md#eigenvector) and [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of its [covariance matrix](../../../variance.md#covariance-matrix); a latent vector typical under the old [covariance](../../../variance.md#covariance) may be very atypical under a substantially different one. Holding $F$ fixed can thus restrict the range of a hyperparameter update, and holding the hyperparameters fixed restricts the next latent-[function](../../../function.md) update. Even exact sampling of each [full conditional distribution](../../../probability-theory.md#full-conditional-distribution) can move slowly along a narrow ridge of the joint [posterior distribution](../../../statistical-inference.md#bayesian-posterior).

Binary observations provide limited information about the absolute size of large correctly signed latent values. This can leave substantial scale uncertainty and strengthen the dependence. Long correlation lengths can also make the [covariance matrix](../../../variance.md#covariance-matrix) nearly singular and the latent coordinates highly dependent. These are plausible explanations for a large [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain), not proofs that every data set causes slow convergence. A [blocked Gibbs sampler](../../../statistical-inference.md#blocked-gibbs-sampler) removes dependence within its chosen blocks, but not dependence between them. Repeated identical inputs should be represented by one shared latent value; otherwise the nominal Gaussian [matrix](../../../vector-space.md#matrix) is singular and the displayed inverse formula must be replaced by a representation on its support.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $s=\sigma^2$ and $\vartheta=(s,\tau_1,\ldots,\tau_m)$. With [conditional independence](../../../random-variable.md#conditional-independence) of the binary observations given the latent [function](../../../function.md), define

$$
L(\vartheta)=\int\ell(F)\varphi_{C_\vartheta}(F)\,dF,
\qquad \ell(F)=\prod_{i=1}^n\Phi((2y_i-1)F_i).
$$

The [prior distribution](../../../statistical-inference.md#prior-probability) is specified on the precision $s^{-1}$, not on $s$. Its [Jacobian determinant](../../../calculus.md#jacobian-determinant) gives

$$
p(\vartheta)=s^{-2}e^{-1/s}\prod_{j=1}^m e^{-\tau_j},\qquad s>0,\ \tau_j>0,
$$

and the marginal [posterior density](../../../statistical-inference.md#posterior-density) is proportional to $p(\vartheta)L(\vartheta)$. Working instead with precision or logarithmic coordinates is possible, provided all corresponding [Jacobian determinants](../../../calculus.md#jacobian-determinant) are included.

Choose an [importance sampling](../../../probability-and-statistics.md#importance-sampling) density $g_\vartheta$ covering the support of $\ell(F)\varphi_{C_\vartheta}(F)$, draw $F_1,\ldots,F_M$ independently from it, and use the nonnegative [unbiased likelihood estimator](../../../statistical-inference.md#unbiased-likelihood-estimator)

$$
\widehat L(\vartheta)=\frac1M\sum_{j=1}^M
\frac{\ell(F_j)\varphi_{C_\vartheta}(F_j)}{g_\vartheta(F_j)}.
$$

Each summand integrates to $L(\vartheta)$, proving unbiasedness. A simple always-valid choice is the latent Gaussian [prior distribution](../../../statistical-inference.md#prior-probability), $g_\vartheta=\varphi_{C_\vartheta}$, when the [covariance matrix](../../../variance.md#covariance-matrix) is nonsingular. Then the estimator is just the average of the bounded values $\ell(F_j)\in(0,1)$. For duplicate inputs, sample only the distinct latent values and multiply all likelihood contributions at each common input. A Gaussian approximation to the latent [posterior distribution](../../../statistical-inference.md#bayesian-posterior), or its mixture with the Gaussian [prior distribution](../../../statistical-inference.md#prior-probability), can reduce relative [variance](../../../variance.md) while keeping complete support. Its approximation does not replace the exact weights.

The [pseudo-marginal Metropolis–Hastings algorithm](../../../statistical-inference.md#pseudo-marginal-metropolis-hastings-algorithm) stores both the current $\vartheta$ and its estimator randomness $u$; write their sampling law as $m_\vartheta(u)$. Propose $\vartheta'\sim q(\vartheta,\cdot)$, independently generate $u'\sim m_{\vartheta'}$, compute $\widehat L(\vartheta',u')$, and accept the pair with

$$
\boxed{\alpha=1\wedge
\frac{p(\vartheta')\widehat L(\vartheta',u')q(\vartheta',\vartheta)}
{p(\vartheta)\widehat L(\vartheta,u)q(\vartheta,\vartheta')}.}
$$

Here $q(\vartheta,\vartheta')$ denotes the proposal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) from $\vartheta$ to $\vartheta'$. On rejection retain both the old parameter and the old likelihood estimate. Initialize with a positive estimate. One must not independently refresh the denominator after rejection.

Correctness follows from the extended [posterior density](../../../statistical-inference.md#posterior-density)

$$
\widetilde\pi(\vartheta,u)\propto
p(\vartheta)\widehat L(\vartheta,u)m_\vartheta(u).
$$

The pair proposal is $q(\vartheta,\vartheta')m_{\vartheta'}(u')$. Its [Metropolis–Hastings acceptance probability](../../../statistical-inference.md#metropolis-hastings-acceptance-probability) simplifies to the displayed ratio, since the auxiliary densities cancel. Hence [detailed balance](../../../markov-process.md#detailed-balance) holds for $\widetilde\pi$. Integrating over $u$ gives $p(\vartheta)L(\vartheta)$ by unbiasedness, so the parameter [marginal distribution](../../../probability-theory.md#marginal-distribution) is exactly the intended [posterior distribution](../../../statistical-inference.md#bayesian-posterior) for any fixed positive $M$. This is exactness of the stationary target, not independent exact samples or a guarantee of rapid convergence. Large relative [variance](../../../variance.md) of the likelihood estimates can produce long holding times, so marginalizing $F$ does not by itself guarantee an improvement in [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain).

## 6

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use the extended target [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
\rho(x,p)=\mu(x)(2\pi)^{-d/2}e^{-\|p\|^2/2}.
$$

The desired [stationary distribution](../../../markov-process.md#stationary-distribution) for positions is $\mu$; the full position-momentum [joint probability distribution](../../../probability-theory.md#joint-probability-distribution) is $\rho$, not $\mu$ alone. Gaussian momentum refreshment preserves $\rho$, since it redraws its momentum [marginal distribution](../../../probability-theory.md#marginal-distribution) independently while keeping the position fixed.

Let $R(x,p)=(x,-p)$ and $T=T_{\varepsilon,L}$ be the surrogate [leapfrog integration](../../../classical-mechanics.md#leapfrog-integration) map. The proposal in the paper is $S=R\circ T$: its notation $(X',-P')=T(x,p)$ includes the final momentum flip. Reversibility gives $RTR=T^{-1}$, so $S^2=I$. Both $R$ and $T$ preserve volume. Thus $S$ is an [involutive Metropolis proposal](../../../statistical-inference.md#involutive-metropolis-proposal), and the required acceptance [probability](../../../probability-theory.md#probability) is

$$
\boxed{\alpha(x,p,x',p')=1\wedge
\frac{\mu(x')e^{-\|p'\|^2/2}}{\mu(x)e^{-\|p\|^2/2}}.}
$$

Equivalently, in terms of the surrogate [Hamiltonian](../../../classical-mechanics.md#hamiltonian) $H_\nu$,

$$
\alpha=1\wedge\left\{
 e^{H_\nu(x,p)-H_\nu(x',p')}
 \frac{\mu(x')\nu(x)}{\mu(x)\nu(x')}
\right\}.
$$

Only evaluations of the true target [probability density function](../../../continuous-probability-distribution.md#probability-density-function) are needed at endpoints; the trajectory uses the surrogate [gradient](../../../calculus.md#gradient). Target and surrogate [normalizing constants](../../../continuous-probability-distribution.md#normalizing-constant) cancel.

For $z=(x,p)$, the accepted flux satisfies

$$
\rho(z)\alpha(z)=\min\{\rho(z),\rho(Sz)\}=\rho(Sz)\alpha(Sz).
$$

Changing variables $z\mapsto Sz$ has unit absolute [Jacobian determinant](../../../calculus.md#jacobian-determinant), so this identity proves [detailed balance](../../../markov-process.md#detailed-balance) for accepted moves. The rejection mass stays at the same point and is also reversible. The accept/reject step therefore preserves $\rho$. Since momentum refreshment also preserves $\rho$, their composition and either phase of the alternating process preserve $\rho$. Projecting onto positions proves **the position [stationary distribution](../../../markov-process.md#stationary-distribution) is exactly the original target**. Stationarity alone does not establish uniqueness or convergence from every start; those require additional [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) and [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain) hypotheses.

There is a genuine defect in the printed smoothing claim. For the positive, nondifferentiable [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution) $\mu(y)=e^{-|y|}/2$ on the real line, direct minimization gives, for every $\lambda>0$,

$$
\min_y\{\log\mu(y)+\lambda(x-y)^2\}
=-\log2-|x|-\frac1{4\lambda}.
$$

For $x>0$ the minimizer is $y=x+1/(2\lambda)$; for $x<0$ it is $y=x-1/(2\lambda)$; at zero both signs minimize. Hence normalization leaves $\nu=\mu$, still nondifferentiable at zero. The displayed construction does not in general produce the asserted smooth surrogate. For example, the also nondifferentiable target $\mu(y)\propto e^{-y^4-|y|}$ makes that infimum $-\infty$ for every $x$, since the negative quartic term dominates the quadratic penalty. The invariance proof above is valid conditional on actually having a usable smooth surrogate, as the subsequent algorithm assumes.

A corrected sufficient construction is [Moreau smoothing of a negative log-density](../../../convex-optimization.md#moreau-smoothing-of-a-negative-log-density). For a [proper convex function](../../../real-analysis.md#proper-convex-function) with [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) $U=-\log\mu$, set

$$
U_\lambda(x)=\min_y\{U(y)+\lambda\|x-y\|^2\},\qquad
\log\nu(x)=C-U_\lambda(x).
$$

The [Moreau envelope](../../../convex-optimization.md#moreau-envelope) is differentiable, with $\nabla U_\lambda(x)=2\lambda(x-\operatorname{prox}_{U/(2\lambda)}(x))$; require $e^{-U_\lambda}$ to be integrable to normalize it. The signs differ from the printed formula. For the [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution), this gives

$$
U_\lambda(x)-\log2=
\begin{cases}
\lambda x^2,&|x|\leq1/(2\lambda),\\
|x|-1/(4\lambda),&|x|>1/(2\lambda),
\end{cases}
$$

a genuinely differentiable potential with integrable exponential tails. Using that surrogate with the boxed acceptance [probability](../../../probability-theory.md#probability) still targets the original [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
