# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper29.pdf)

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
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $Y=\mathbb E[X\mid\mathcal G]$. The [conditional expectation](../../../measure-theory.md#conditional-expectation) is an $L^2$ contraction by the [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality), so $X,Y$ are square-integrable. The defining integral identity for [conditional expectation](../../../measure-theory.md#conditional-expectation), first with bounded [measurable](../../../measure-theory.md#measurability) truncations of $Y$ and then with their $L^2$ limit, gives

$$
\mathbb E[XY]=\mathbb E[Y\mathbb E[X\mid\mathcal G]]=\mathbb E[Y^2].
$$

For clarity, if $Y^{(K)}=\max(-K,\min(Y,K))$, then $\mathbb E[XY^{(K)}]=\mathbb E[YY^{(K)}]$, and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) permits the limit $K\to\infty$. Expanding the square now proves the [equality case for conditional second moments](../../../measure-theory.md#equality-case-for-conditional-second-moments):

$$
\mathbb E[(X-Y)^2]=\mathbb E[X^2]-\mathbb E[Y^2]=0.
$$

A nonnegative [random variable](../../../random-variable.md) of zero [expected value](../../../probability-theory.md#expected-value) vanishes [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Therefore $\boxed{X=Y\text{ almost surely}.}$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Equality of the [probability distributions](../../../probability-theory.md#probability-distribution) implies equality of all integrals for which they are finite, in particular $\mathbb E[(\mathbb E[X\mid\mathcal G])^2]=\mathbb E[X^2]<\infty$. Part (a), applied to this [conditional expectation](../../../measure-theory.md#conditional-expectation), therefore gives $\boxed{X=\mathbb E[X\mid\mathcal G]\text{ almost surely}.}$ The second-moment assumption justifies the squared-norm argument; the next part removes it.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Again put $Y=\mathbb E[X\mid\mathcal G]$. For any fixed real $c$, the [random variable](../../../random-variable.md)

$$
D_c=|X-c|-\operatorname{sign}(Y-c)(X-c)
$$

is nonnegative and [integrable](../../../measure-theory.md#integrability). The [sign function](../../../foundations-of-mathematics.md#sign-function) of $Y-c$ is bounded and $\mathcal G$-[measurable](../../../measure-theory.md#measurability), so conditioning and equality of the [probability distributions](../../../probability-theory.md#probability-distribution) give

$$
\mathbb E D_c=\mathbb E|X-c|-\mathbb E[\operatorname{sign}(Y-c)(Y-c)]=\mathbb E|X-c|-\mathbb E|Y-c|=0.
$$

Thus $D_c=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). On $\{Y>c\}$ this forces $X\geq c$; on $\{Y<c\}$ it forces $X\leq c$; on $\{Y=c\}$ it forces $X=c$. In particular $\{Y=c\}\subseteq\{X=c\}$ up to a null set. These two [events](../../../probability-theory.md#event) have equal [probability](../../../probability-theory.md#probability), again by equality of the [probability distributions](../../../probability-theory.md#probability-distribution), so they agree up to a null set. Consequently

$$
\operatorname{sign}(X-c)=\operatorname{sign}(Y-c)\quad\text{almost surely}.
$$

Taking $c=0$ establishes the suggested sign assertion, but this alone would not exclude unequal positive values. Apply the same argument simultaneously to the [countable](../../../set-theory.md#countable-set) set of rational $c$. Outside the union of their null sets, unequal $X$ and $Y$ would have a rational strictly between them, giving opposite signs. This proves the [conditional expectation preserving a distribution](../../../measure-theory.md#conditional-expectation-preserving-a-distribution) result:

$$
\boxed{X=\mathbb E[X\mid\mathcal G]\quad\text{almost surely}.}
$$

Only [integrability](../../../measure-theory.md#integrability) was used; no finite second moment or hidden square-integrability assumption is needed.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A convenient precise version is the [almost sure submartingale convergence theorem](../../../martingale.md#almost-sure-submartingale-convergence-theorem): if $(S_n)$ is a real [submartingale](../../../martingale.md#submartingale) and $\sup_n\mathbb E S_n^+<\infty$, then $S_n$ converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) to a finite [integrable random variable](../../../probability-theory.md#integrable-random-variable). In particular the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) applies to any [martingale](../../../martingale.md) with $\sup_n\mathbb E|S_n|<\infty$. It asserts neither [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) nor preservation of the initial [expected value](../../../probability-theory.md#expected-value) without additional [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability).

Here is a proof including the crossing estimate. Fix real $a<b$, and let $U_n[a,b]$ count completed [upcrossings](../../../martingale.md#upcrossing) by time $n$. Use a predictable indicator $H_k$ which holds one unit during each crossing attempt: enter when $S_k\leq a$, exit when $S_k\geq b$. With

$$
G_n=\sum_{k=0}^{n-1}H_k(S_{k+1}-S_k),
$$

each completed trade gains at least $b-a$, while the possible unfinished trade loses no more than $(S_n-a)^-$. Hence $G_n\geq(b-a)U_n[a,b]-(S_n-a)^-$. The [submartingale](../../../martingale.md#submartingale) property and $0\leq H_k\leq1$ give $\mathbb E G_n\leq\mathbb E(S_n-S_0)$: the complementary predictable gains have nonnegative [expected value](../../../probability-theory.md#expected-value). Therefore

$$
(b-a)\mathbb E U_n[a,b]\leq\mathbb E(S_n-S_0)+\mathbb E(S_n-a)^-=\mathbb E(S_n-a)^++a-\mathbb E S_0.
$$

The right side is uniformly bounded, since $(S_n-a)^+\leq S_n^++|a|$. By the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem), every rational interval has finitely many [upcrossings](../../../martingale.md#upcrossing) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). A real sequence whose lower and upper limits differ crosses some rational interval infinitely often, so the [countable](../../../set-theory.md#countable-set) intersection of these events gives an extended-real limit. Furthermore

$$
\mathbb E S_n^- =\mathbb E S_n^+-\mathbb E S_n\leq\sup_m\mathbb E S_m^+-\mathbb E S_0,
$$

so $\sup_n\mathbb E|S_n|<\infty$. The [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) makes the limit finite and [integrable](../../../measure-theory.md#integrability), completing the proof. Applying this theorem to $-Z_n$ gives the [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) for nonnegative [supermartingales](../../../martingale.md#supermartingale).

For the given adapted multiplicative drift, put

$$
P_0=1,\qquad P_n=\prod_{k=0}^{n-1}(1+Y_k),\qquad Z_n=\frac{X_n}{P_n}.
$$

The next denominator $P_{n+1}$ is $\mathcal F_n$-[measurable](../../../measure-theory.md#measurability), and $P_n\geq1$ makes $Z_n$ [integrable](../../../measure-theory.md#integrability). Thus

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]=\frac{\mathbb E[X_{n+1}\mid\mathcal F_n]}{P_{n+1}}\leq\frac{(1+Y_n)X_n}{P_{n+1}}=Z_n.
$$

The nonnegative [supermartingale](../../../martingale.md#supermartingale) $Z_n$ has a finite [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence) limit $Z_\infty$. On the probability-one event where the specified series is finite,

$$
0\leq\log P_n=\sum_{k<n}\log(1+Y_k)\leq\sum_{k\geq0}Y_k<\infty.
$$

Consequently $P_n\uparrow P_\infty\in[1,\infty)$ and the [multiplicative correction for summable adapted drift](../../../martingale.md#multiplicative-correction-for-summable-adapted-drift) gives

$$
\boxed{X_n\longrightarrow P_\infty Z_\infty<\infty\quad\text{almost surely}.}
$$

The argument does not require a finite [expected value](../../../probability-theory.md#expected-value) for the infinite product or for the total drift.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) $T_a$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Indeed the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives $\mathbb P(T_a\leq t)=2\mathbb P(B_t\geq a)\to1$ as $t\to\infty$. Continuity of the paths means the first passage to $x+y$ occurs after the first passage to $x$. By the [Strong Markov property](../../../markov-process.md#strong-markov-property), the process $B_{T_x+s}-x$ is an independent fresh [Brownian motion](../../../brownian-motion.md). Thus $T_{x+y}-T_x$ has the same [probability distribution](../../../probability-theory.md#probability-distribution) as $T_y$ and is independent of $T_x$. Taking the [Laplace transforms of nonnegative random variables](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) gives

$$
\boxed{\varphi_{x+y}(\lambda)=\varphi_x(\lambda)\varphi_y(\lambda).}
$$

For fixed $\lambda\geq0$, these transforms lie in $(0,1]$. Put $g(a)=-\log\varphi_a(\lambda)$. It is additive on positive arguments and nondecreasing, because the hitting times increase with the level. Writing $c(\lambda)=g(1)$, additivity gives $g(r)=rc(\lambda)$ for positive rational $r$, and rational upper and lower approximations then give $g(a)=ac(\lambda)$ for every $a>0$. Hence $\varphi_a(\lambda)=e^{-ac(\lambda)}$, with $c(\lambda)\geq0$.

The [Brownian scaling](../../../brownian-motion.md#brownian-scaling) identity $T_a\overset d=a^2T_1$ gives

$$
e^{-ac(\lambda)}=\varphi_1(a^2\lambda)=e^{-c(a^2\lambda)}.
$$

For $\lambda>0$, take $a=\sqrt\lambda$ in this relation with the transform parameter one. It follows that $c(\lambda)=C\sqrt\lambda$, where $C=c(1)\geq0$. At zero, finiteness of the hitting time gives $c(0)=0$. Thus $\boxed{\varphi_a(\lambda)=e^{-aC\sqrt\lambda}}$, with the constant determined in part (b).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix $\lambda>0$ and choose the positive root

$$
\theta=b+\sqrt{b^2+2\lambda}>0,\qquad \frac{\theta^2}{2}-b\theta=\lambda.
$$

Use the [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion) $M_t=\exp(\theta B_t-\theta^2t/2)$. Before the linear-boundary [stopping time](../../../martingale.md#stopping-time) $\tau$, path continuity gives $B_s<a+bs$. At the boundary there is equality. Consequently

$$
0\leq M_{t\wedge\tau}\leq e^{\theta a}e^{-\lambda(t\wedge\tau)}\leq e^{\theta a}.
$$

The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the bounded [stopping time](../../../martingale.md#stopping-time) $t\wedge\tau$ yields $\mathbb E M_{t\wedge\tau}=1$. Separate the two events:

$$
1=e^{\theta a}\mathbb E[e^{-\lambda\tau}\mathbf1_{\{\tau\leq t\}}]+\mathbb E[M_t\mathbf1_{\{\tau>t\}}].
$$

The last term is at most $e^{\theta a-\lambda t}$ and tends to zero. The first term converges by the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem). Taking $e^{-\lambda\infty}=0$ therefore proves

$$
\boxed{\mathbb E e^{-\lambda\tau}=\exp\!\left[-a\left(b+\sqrt{b^2+2\lambda}\right)\right].}
$$

This bounded-stopping argument does not assume in advance that $\tau$ is finite. For $b\leq0$, letting $\lambda\downarrow0$ makes the right side tend to one, so it also proves $\mathbb P(\tau<\infty)=1$. Setting $b=0$ gives the [Brownian first-passage Laplace transform](../../../markov-process.md#brownian-first-passage-laplace-transform)

$$
\boxed{\varphi_a(\lambda)=e^{-a\sqrt{2\lambda}},\qquad\lambda\geq0,\qquad C=\sqrt2.}
$$

The zero-parameter value follows from the just-proved almost-sure finiteness.

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For [probability measures](../../../probability-theory.md#probability-measure) on a metric space, [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) $\mu_n\Rightarrow\mu$ means $\int f\,d\mu_n\to\int f\,d\mu$ for every bounded continuous real function $f$. On the real line it is equivalently convergence of the [cumulative distribution functions](../../../probability-theory.md#cumulative-distribution-function) at every continuity point of the limiting [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function). Bounded continuous upper and lower approximations to interval indicators give one direction; a partition at continuity points, uniform approximation on a compact interval, and control of the tails give the reverse direction.

For a [probability measure](../../../probability-theory.md#probability-measure) $\mu$ on $\mathbb R$, its [characteristic function](../../../probability-theory.md#characteristic-function) is $\varphi_\mu(t)=\int e^{itx}\mu(dx)$. The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) states: $\mu_n\Rightarrow\mu$ implies $\varphi_{\mu_n}(t)\to\varphi_\mu(t)$ for every real $t$; conversely, if these [characteristic functions](../../../probability-theory.md#characteristic-function) have a pointwise limit $\varphi$ which is continuous at zero, there is a unique [probability measure](../../../probability-theory.md#probability-measure) $\mu$ with [characteristic function](../../../probability-theory.md#characteristic-function) $\varphi$, and $\mu_n\Rightarrow\mu$. In particular, for a specified limiting [probability measure](../../../probability-theory.md#probability-measure), weak convergence is equivalent to pointwise convergence of its [characteristic functions](../../../probability-theory.md#characteristic-function).

The forward implication follows by testing cosine and sine. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) shows that every [characteristic function](../../../probability-theory.md#characteristic-function) is continuous at zero and has value one there. For the converse, first establish [tightness of probability measures](../../../probability-theory.md#uniform-tightness). By [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem), for $h>0$,

$$
\frac1{2h}\int_{-h}^h(1-\operatorname{Re}\varphi_{\mu_n}(t))\,dt
=\int\left(1-\frac{\sin(hx)}{hx}\right)\mu_n(dx).
$$

The integrand on the right is at least $1/2$ when $|x|\geq2/h$. This proves the [characteristic-function tightness bound](../../../probability-theory.md#characteristic-function-tightness-bound)

$$
\mu_n(|x|\geq2/h)\leq\frac1h\int_{-h}^h(1-\operatorname{Re}\varphi_{\mu_n}(t))\,dt.
$$

The integrals converge for each $h$ by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem), and continuity of $\varphi$ at zero makes the limit as small as desired by choosing $h$ small. Thus all sufficiently late measures have a common tail bound; the finitely many earlier measures also have small tails once the radius is increased. This is uniform [tightness of probability measures](../../../probability-theory.md#uniform-tightness).

We give the required compactness argument explicitly. For any subsequence, choose a further diagonal subsequence whose [cumulative distribution functions](../../../probability-theory.md#cumulative-distribution-function) $F_n$ converge at every rational $q$, to $f(q)$. Define

$$
F(x)=\inf_{\substack{q>x\\q\in\mathbb Q}}f(q).
$$

This function is nondecreasing and right-continuous: given a rational $q>x$ with $f(q)$ close to $F(x)$, the same bound holds for $F(y)$ when $x<y<q$. Tightness gives $F(-\infty)=0$ and $F(+\infty)=1$, so $F$ is a [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) of a [probability measure](../../../probability-theory.md#probability-measure) $\nu$. For rationals $r<x<s$, $F_n(r)\leq F_n(x)\leq F_n(s)$. The limits bracket $F(x-)$ and $F(x)$; at a continuity point of $F$ they coincide. Thus $F_n(x)\to F(x)$ at all such points. To obtain weak convergence, choose a compact interval with small tails and partition it using continuity points of $F$. A bounded continuous function is uniformly continuous there, so step-function approximations and convergence of interval probabilities prove convergence of its integral. This proves [Helly selection for distribution functions](../../../probability-theory.md#helly-selection-for-distribution-functions) and supplies a weak subsequential limit $\nu$.

Its [characteristic function](../../../probability-theory.md#characteristic-function) is $\varphi$ by the already proved forward implication. We also prove uniqueness rather than assume it. If two [probability measures](../../../probability-theory.md#probability-measure) $\nu,\rho$ have the same [characteristic function](../../../probability-theory.md#characteristic-function), convolve each with a centered [normal distribution](../../../probability-theory.md#normal-distribution) of variance $\varepsilon^2>0$. Their densities are, by the [Gaussian integral](../../../calculus.md#gaussian-integral) and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem),

$$
p_{\nu,\varepsilon}(x)=\frac1{2\pi}\int_{\mathbb R}e^{-itx}\varphi_\nu(t)e^{-\varepsilon^2t^2/2}\,dt,
$$

and likewise for $\rho$. The integrable Gaussian factor justifies exchanging the integrals, so these densities agree. For every bounded continuous $f$, letting $\varepsilon\downarrow0$ in $\int\mathbb E[f(x+\varepsilon Z)]\nu(dx)$, with $Z$ a standard [normal random variable](../../../probability-theory.md#gaussian-random-variable), gives $\int f\,d\nu$ by [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem). Hence the two measures have equal integrals against all these test functions, and approximating interval indicators shows $\nu=\rho$. This proves the [uniqueness theorem for characteristic functions](../../../probability-theory.md#uniqueness-theorem-for-characteristic-functions).

Every subsequence therefore has a further subsequence weakly converging to the same unique $\mu$. If the original sequence failed weak convergence, some bounded continuous test function would have a subsequence of integrals staying a fixed distance from its integral under $\mu$, contradicting that further convergence. This completes both directions of the theorem. Continuity at zero is essential: the laws $N(0,n)$ have pointwise limiting [characteristic function](../../../probability-theory.md#characteristic-function) zero away from zero and one at zero, and are not tight.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For the finite [probability distribution](../../../probability-theory.md#probability-distribution), put $\xi_j=(X_j+1)/2$. These are [independent](../../../random-variable.md#independent-random-variables) fair zero-one variables, and

$$
Y_n=2\sum_{j=1}^n2^{-j}\xi_j-(1-2^{-n}).
$$

The binary integer $\sum_{j=1}^n2^{n-j}\xi_j$ is uniform on $\{0,\ldots,2^n-1\}$. Hence

$$
\boxed{\mathbb P\!\left(Y_n=-1+\frac{2k+1}{2^n}\right)=2^{-n},\qquad 0\leq k<2^n.}
$$

These are the midpoints of $2^n$ equal subintervals of $[-1,1]$. For every bounded continuous $f$, the [Riemann sums](../../../real-analysis.md#riemann-sum) give

$$
\mathbb E f(Y_n)=2^{-n}\sum_{k=0}^{2^n-1}f\!\left(-1+\frac{2k+1}{2^n}\right)\longrightarrow\frac12\int_{-1}^1f(x)\,dx.
$$

Thus $\boxed{Y_n\Rightarrow\operatorname{Unif}[-1,1]}$ in the sense of [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures).

For the almost-sure and $L^2$ assertions, the [Dyadic Rademacher series](../../../probability-theory.md#dyadic-rademacher-series) $Y=\sum_{j\geq1}2^{-j}X_j$ converges absolutely on every sign sequence, since $|X_j|=1$. Its tail satisfies $|Y-Y_n|\leq2^{-n}$, proving [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence) and [convergence in L2](../../../convergence-of-random-variables.md#convergence-in-l2). More precisely, zero means and [independence](../../../random-variable.md#independent-random-variables) eliminate the cross terms:

$$
\boxed{\mathbb E[(Y-Y_n)^2]=\sum_{j>n}4^{-j}=\frac{4^{-n}}3.}
$$

This identity follows first for finite tails and then by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem). Bounded continuous test functions and [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) identify the [probability distribution](../../../probability-theory.md#probability-distribution) of $Y$ with the weak limit above, namely the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[-1,1]$.

For the requested product identity, each [Rademacher random variable](../../../probability-theory.md#rademacher-distribution) has [characteristic function](../../../probability-theory.md#characteristic-function) $\mathbb E e^{itX_j}=\cos t$. The [characteristic function of a sum of independent variables](../../../probability-theory.md#characteristic-function-of-a-sum-of-independent-variables) therefore yields

$$
\varphi_{Y_n}(t)=\prod_{j=1}^n\cos(t/2^j).
$$

By part (a), or directly by [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem), this converges to the [characteristic function of a uniform distribution](../../../probability-theory.md#characteristic-function-of-a-uniform-distribution), $\tfrac12\int_{-1}^1e^{itx}\,dx=\sin t/t$. Consequently the [dyadic cosine product](../../../probability-theory.md#dyadic-cosine-product) is

$$
\boxed{\prod_{j=1}^{\infty}\cos(t/2^j)=\frac{\sin t}{t},\qquad t\in\mathbb R.}
$$

Both sides are one at zero. At zeros of the [sinc function](../../../analysis.md#sinc-function) the identity is understood as the limit of the finite products, so no logarithm or division by a vanishing factor is needed.

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $B$ be a standard [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $z$. Neighbourhood recurrence means that, with [probability](../../../probability-theory.md#probability) one, every nonempty open subset of $\mathbb R^2$ is visited at arbitrarily large times. Not hitting points means that for each fixed $w\ne z$, $\mathbb P_z(\exists t\geq0:B_t=w)=0$. If $w=z$, time zero must be excluded, and there is still no return at any positive time. This assertion concerns each prescribed point; it does not say that the path contains no points.

We prove both claims from the [planar Brownian annulus hitting probability](../../../brownian-motion.md#planar-brownian-annulus-hitting-probability). Fix a center $w$ and radii $0<r<\rho=|z-w|<R$, and define the [stopping times](../../../martingale.md#stopping-time) $\tau_r=\inf\{t:|B_t-w|=r\}$ and $\tau_R=\inf\{t:|B_t-w|=R\}$. Their minimum $\sigma$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence): a coordinate of [Brownian motion](../../../brownian-motion.md) cannot stay forever in a bounded interval, by the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process), so exit from the outer disk is finite. On the annulus,

$$
\Delta\log|x-w|=0.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore makes $\log|B_{t\wedge\sigma}-w|$ a [local martingale](../../../martingale.md#local-martingale). It is bounded between $\log r$ and $\log R$, hence is a genuine [martingale](../../../martingale.md). The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $t\wedge\sigma$, followed by the [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem), gives

$$
\log\rho=\mathbb P_z(\tau_r<\tau_R)\log r+\mathbb P_z(\tau_R<\tau_r)\log R.
$$

Thus

$$
\boxed{\mathbb P_z(\tau_r<\tau_R)=\frac{\log(R/\rho)}{\log(R/r)}.}
$$

The exit can only be at one of the two distinct boundaries by path continuity.

For a fixed $r$, let $R\to\infty$. These events increase to $\{\tau_r<\infty\}$: any path up to a finite hitting time is bounded and so avoids some sufficiently large outer circle. The ratio tends to one, proving that any closed disk of positive radius is hit [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) from any starting point outside it. An initial point inside it already counts as a hit.

To prove the stronger recurrence statement, take a closed disk contained in any prescribed nonempty open set. At each integer time $n$, the [Markov property](../../../markov-process.md#markov-property) and the preceding disk-hitting result imply that some time $t\geq n$ visits this disk with [probability](../../../probability-theory.md#probability) one. Intersecting these events over all $n$ proves visits at arbitrarily large times. A [countable](../../../set-theory.md#countable-set) basis of disks with rational centers and rational radii makes this simultaneous for all nonempty open sets. This is [recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion), or equivalently neighbourhood recurrence.

For point avoidance, keep $R>\rho$ fixed and let $r\downarrow0$. Hitting $w$ before $\tau_R$ requires hitting every inner circle first. The displayed ratio tends to zero, so this point-hitting event has [probability](../../../probability-theory.md#probability) zero. Any finite hit of $w$ would occur before exit from some outer circle with integer radius, again because the preceding path is bounded. A [countable union](../../../set.md#countable-union) now gives $\boxed{\mathbb P_z(T_w<\infty)=0\ (z\ne w)}$, the [polar point for planar Brownian motion](../../../brownian-motion.md#polar-point-for-planar-brownian-motion) assertion.

Finally, even if the process starts at $w$, for each deterministic $s>0$ its [normal distribution](../../../probability-theory.md#normal-distribution) has a density, so $\mathbb P(B_s=w)=0$. The [Markov property](../../../markov-process.md#markov-property) at $s$ and the result from other starting points exclude any visit to $w$ at or after $s$. Taking $s=1/n$ excludes all positive-time returns. Thus **planar Brownian motion repeatedly approaches every point, while almost surely never hitting any prescribed point at positive time**.

## 6

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Interpret the comparison at $N$ on $\{N<\infty\}$; values at an infinite [stopping time](../../../martingale.md#stopping-time) are not required. The [stopping time](../../../martingale.md#stopping-time) events make $Y_n$ adapted, and $|Y_n|\leq|X_n^1|+|X_n^2|$ gives [integrability](../../../measure-theory.md#integrability). On $\{N\leq n\}$ the next value is $X_{n+1}^2$. On $\{N>n\}$ it is $X_{n+1}^1$ unless $N=n+1$, and on that latter event switching only decreases the value. Consequently the pointwise inequality

$$
Y_{n+1}\leq\mathbf1_{\{N>n\}}X_{n+1}^1+\mathbf1_{\{N\leq n\}}X_{n+1}^2
$$

holds even though $\{N=n+1\}$ need not be known at time $n$. Both indicators displayed here are $\mathcal F_n$-[measurable](../../../measure-theory.md#measurability). Taking [conditional expectations](../../../measure-theory.md#conditional-expectation) and using the two [supermartingale](../../../martingale.md#supermartingale) inequalities therefore gives

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]\leq\mathbf1_{\{N>n\}}X_n^1+\mathbf1_{\{N\leq n\}}X_n^2=Y_n.
$$

Thus $\boxed{Y\text{ is a supermartingale}.}$ This proves [pasting supermartingales with downward jumps](../../../martingale.md#pasting-supermartingales-with-downward-jumps) without incorrectly treating the future switching event as predictable.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Put $q=b/a>1$. Each successive crossing time $N_j$, $j\geq1$, is a [stopping time](../../../martingale.md#stopping-time), since in discrete time the event that a threshold is first met after the previous [stopping time](../../../martingale.md#stopping-time) can be written as a finite union of events known at the candidate time. Use $\inf\varnothing=\infty$, with all later crossing times then infinite as well.

For the supermartingale assertion, build a process by finitely many switches. Begin with the constant [supermartingale](../../../martingale.md#supermartingale) one. At $N_1$ switch to $X_n/a$; the new value at that time is at most one. At $N_2$ switch to the constant $q$; the old value there is $X_{N_2}/a\geq q$. At $N_3$ switch to $qX_n/a$, whose value is at most $q$, and at $N_4$ switch to the constant $q^2$, whose value is at most the previous process. More generally, the switches at $N_{2\ell-1}$ and $N_{2\ell}$ are respectively from cash $q^{\ell-1}$ to $q^{\ell-1}X_n/a$ and from that stock value to cash $q^\ell$. Every switch is downward, including possible overshoots of either threshold.

Each candidate continuation is a [supermartingale](../../../martingale.md#supermartingale), being either constant or a fixed positive multiple of $X$. Part (a) therefore proves by induction that the process $M^{(j)}$ obtained after the first $j$ switches is a [supermartingale](../../../martingale.md#supermartingale). It agrees with $Y$ through $N_j$. For fixed $j,n$, its values are bounded in absolute value by a deterministic constant depending on $j$ times $1+X_n$, which also verifies the required [integrability](../../../measure-theory.md#integrability) rather than assuming it for an infinite sequence of pastings.

Stopping a discrete [supermartingale](../../../martingale.md#supermartingale) preserves the property. Indeed its stopped increment is $\mathbf1_{\{N_j>n\}}(M^{(j)}_{n+1}-M^{(j)}_n)$, with an $\mathcal F_n$-[measurable](../../../measure-theory.md#measurability) indicator; integrability at any fixed time follows from a finite sum of the absolute values at earlier times. Hence

$$
\boxed{Y_{n\wedge N_j}=M^{(j)}_{n\wedge N_j}\text{ is a nonnegative supermartingale for }j\geq1.}
$$

This is the [multiplicative upcrossing supermartingale](../../../martingale.md#multiplicative-upcrossing-supermartingale) construction. The printed $j=0$ case uses $N_0=-1$, while $Y$ was only defined from time zero. With the natural pre-start convention $Y_{-1}=1$, it is the constant process one and the assertion also holds for $j=0$. Without such an extension, that single displayed stopped process is undefined.

For the probability bound, the actual initial value is

$$
Y_0=\min(X_0/a,1),
$$

because $N_1=0$ exactly when $X_0\leq a$. For an integer $k\geq1$, stop after the $k$th completed [upcrossing](../../../martingale.md#upcrossing), at $N_{2k}$. The nonnegative stopped [supermartingale](../../../martingale.md#supermartingale) satisfies

$$
q^k\mathbb P(N_{2k}\leq n)\leq\mathbb E Y_{n\wedge N_{2k}}\leq\mathbb E Y_0,
$$

since $Y_{N_{2k}}=q^k$ on the event in the left side. Letting $n\to\infty$, and identifying $\{U\geq k\}=\{N_{2k}<\infty\}$, proves the [Dubins upcrossing inequality](../../../martingale.md#dubins-upcrossing-inequality):

$$
\boxed{\mathbb P(U\geq k)\leq\left(\frac ab\right)^k\mathbb E\min(X_0/a,1),\qquad k=1,2,\ldots.}
$$

Neither finiteness of $N_{2k}$ nor [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) is needed. The bound is for positive integers $k$; extending it to $k=0$ would generally be false, because its left side would be one while $\mathbb E\min(X_0/a,1)$ can be less than one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
