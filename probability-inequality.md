# Probability inequality

↑ **Parent:** [Probability theory](probability-theory.md)

Probability inequalities bound event probabilities using moments or other tractable quantities.

**Table of contents**

- [Lyapunov moment inequality](#lyapunov-moment-inequality)
- [Chebyshev inequality](#chebyshev-inequality)
  - [Cantelli inequality](#cantelli-inequality)
- [First moment method](#first-moment-method)
- [Second moment method](#second-moment-method)
- [Markov inequality](#markov-inequality)
  - [Exponential Markov bound](#exponential-markov-bound)
- [Concentration inequality](#concentration-inequality)
  - [Concentration of Lipschitz functions on the symmetric group](#concentration-of-lipschitz-functions-on-the-symmetric-group)
  - [Talagrand convex distance](#talagrand-convex-distance)
    - [Talagrand's convex distance inequality](#talagrand-s-convex-distance-inequality)
      - [Section induction for the Talagrand exponential moment](#section-induction-for-the-talagrand-exponential-moment)
      - [Scalar estimate for Talagrand product induction](#scalar-estimate-for-talagrand-product-induction)
  - [Entropy functional](#entropy-functional)
    - [Logarithmic Sobolev inequality](#logarithmic-sobolev-inequality)
      - [Logarithmic Sobolev inequality implies hypercontractivity](#logarithmic-sobolev-inequality-implies-hypercontractivity)
  - [Hoeffding inequality](#hoeffding-inequality)
    - [Hoeffding lemma](#hoeffding-lemma)
  - [Bennett inequality](#bennett-inequality)
    - [Bennett bounds for sparse binomial fluctuations](#bennett-bounds-for-sparse-binomial-fluctuations)
    - [Bennett rate function](#bennett-rate-function)
  - [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)
    - [Gaussian Poincaré inequality](#gaussian-poincare-inequality)
    - [Tensorization of a Poincaré inequality](#tensorization-of-a-poincare-inequality)
    - [Pushforward of a Poincaré inequality by a Lipschitz function](#pushforward-of-a-poincare-inequality-by-a-lipschitz-function)
    - [Poincaré inequality for the uniform distribution on an interval](#poincare-inequality-for-the-uniform-distribution-on-an-interval)
    - [Gaussian logarithmic Sobolev inequality](#gaussian-logarithmic-sobolev-inequality)
      - [Sharpness of the Gaussian logarithmic Sobolev constant](#sharpness-of-the-gaussian-logarithmic-sobolev-constant)
      - [Ornstein-Uhlenbeck entropy dissipation identity](#ornstein-uhlenbeck-entropy-dissipation-identity)
    - [Convex Poincaré inequality](#convex-poincare-inequality)
  - [Chernoff bound](#chernoff-bound)
    - [Entrywise concentration of a Gaussian Gram matrix](#entrywise-concentration-of-a-gaussian-gram-matrix)
  - [Bounded differences property](#bounded-differences-property)
    - [McDiarmid's inequality](#mcdiarmid-s-inequality)
      - [Boolean cube expansion from bounded differences](#boolean-cube-expansion-from-bounded-differences)
    - [Talagrand's one-sided bounded differences inequality](#talagrand-s-one-sided-bounded-differences-inequality)
  - [Certifiable function](#certifiable-function)
    - [Entropy method for certifiable functions](#entropy-method-for-certifiable-functions)
  - [Self-bounding function](#self-bounding-function)
    - [Weakly self-bounding function](#weakly-self-bounding-function)
      - [Variance bound for a weakly self-bounding function](#variance-bound-for-a-weakly-self-bounding-function)
      - [Lower-tail concentration for a weakly self-bounding function](#lower-tail-concentration-for-a-weakly-self-bounding-function)
  - [Tensorization of entropy](#tensorization-of-entropy)
  - [Efron–Stein inequality](#efron-stein-inequality)
    - [Variance tensorization](#variance-tensorization)
  - [Modified logarithmic Sobolev inequality](#modified-logarithmic-sobolev-inequality)
    - [Herbst argument](#herbst-argument)
  - [Transport-entropy inequality](#transport-entropy-inequality)
    - [Tensorization of a transport-entropy inequality](#tensorization-of-a-transport-entropy-inequality)
  - [Sub-Poisson random variable in the right tail](#sub-poisson-random-variable-in-the-right-tail)
  - [Sub-Gamma random variable in the right tail](#sub-gamma-random-variable-in-the-right-tail)
    - [Bernstein inequalities (probability theory)](#bernstein-inequalities-probability-theory)
      - [Bernstein bound for independent sub-exponential variables](#bernstein-bound-for-independent-sub-exponential-variables)
  - [Rosenthal inequality](#rosenthal-inequality)
  - [Talagrand's concentration inequality](#talagrand-s-concentration-inequality)
    - [Talagrand concentration inequality for certifiable functions](#talagrand-concentration-inequality-for-certifiable-functions)
      - [Two-threshold concentration for certifiable functions](#two-threshold-concentration-for-certifiable-functions)
      - [Increasing-subsequence certificate concentration](#increasing-subsequence-certificate-concentration)
- [Boole's inequality](#boole-s-inequality)
  - [Positive common intersection from pair-intersection probabilities](#positive-common-intersection-from-pair-intersection-probabilities)
- [FKG inequality](#fkg-inequality)
  - [FKG lattice condition](#fkg-lattice-condition)
    - [Exponential-tilt proof of positive association](#exponential-tilt-proof-of-positive-association)
  - [Harris-FKG inequality](#harris-fkg-inequality)
    - [Square-root bound for increasing events](#square-root-bound-for-increasing-events)
    - [Square-root trick for positively associated events](#square-root-trick-for-positively-associated-events)
    - [Harris' inequality](#harris-inequality)
      - [Negative correlation of increasing and decreasing events](#negative-correlation-of-increasing-and-decreasing-events)
      - [Increasing event](#increasing-event)
        - [Sharp threshold](#sharp-threshold)
        - [Transitive increasing event](#transitive-increasing-event)
        - [Decreasing event](#decreasing-event)
- [Janson inequality](#janson-inequality)
  - [Janson lower-tail bound by independent thinning](#janson-lower-tail-bound-by-independent-thinning)
  - [Janson dependency sum](#janson-dependency-sum)
  - [Janson sequential product lemma](#janson-sequential-product-lemma)
- [Lévy maximal inequality](#levy-maximal-inequality)

## Lyapunov moment inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)

For a [random variable](random-variable.md) $Z$ and exponents $0<r<s$, the absolute [moment](probability-theory.md#moment) norms satisfy $(\mathbb E|Z|^r)^{1/r}\leq(\mathbb E|Z|^s)^{1/s}$, allowing infinity. For a finite $s$th [moment](probability-theory.md#moment), apply the [Jensen inequality](real-analysis.md#jensen-s-inequality) to the [concave function](real-analysis.md#concave-function) $t^{r/s}$ and $|Z|^s$. The formula is for positive exponents; $r=0$ requires a separately defined limiting quantity.

## Chebyshev inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_inequality)

For a random variable $X$ of finite variance and $a>0$,

$$
\mathbb P(|X-\mathbb EX|\geq a)
\leq\frac{\operatorname{var}(X)}{a^2}.
$$

### Cantelli inequality

↑ **Parent:** [Chebyshev inequality](#chebyshev-inequality)

For a finite-variance [random variable](random-variable.md), shift its centred version by $b>0$ and apply [Markov inequality](#markov-inequality) to the square. Minimizing $(\sigma^2+b^2)/(a+b)^2$ at $b=\sigma^2/a$ proves the bound. A two-point distribution attains equality. If the [variance](variance.md) is zero, the centred variable vanishes almost surely.

## First moment method

↑ **Parent:** [Probability inequality](probability-inequality.md)

This is a [Markov inequality](#markov-inequality) argument, complementary to the [second moment method](#second-moment-method). For a nonnegative integer-valued random variable $N$, [Markov inequality](#markov-inequality) gives

$$
\mathbb P(N\geq1)\leq\mathbb EN.
$$

Consequently, $\mathbb EN<1$ proves that some outcome has $N=0$, while $\mathbb EN\to0$ shows that $N=0$ with probability tending to one.

## Second moment method

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_moment_method)

For a nonnegative random variable $N$, Chebyshev's inequality gives

$$
\mathbb P(N=0)
\leq\frac{\operatorname{var}(N)}{(\mathbb EN)^2}.
$$

Hence $\operatorname{var}(N)/(\mathbb EN)^2\to0$ implies that $N>0$ with probability tending to one.

## Markov inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Markov_inequality)

For a nonnegative random variable $Y$ and $a>0$,

$$
\Pr(Y\geq a)\leq\frac{\mathbb EY}{a}.
$$

### Exponential Markov bound

↑ **Parent:** [Markov inequality](#markov-inequality)

Applying Markov's inequality to $e^{tX}$ gives

$$
\Pr(X\geq x)\leq e^{-tx}M_X(t),
\qquad t>0.
$$

Optimizing this expression is the basic Chernoff-bound method.

## Concentration inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Concentration_inequality)

A concentration inequality bounds the probability that a [random variable](random-variable.md) differs substantially from a typical value such as its [expected value](probability-theory.md#expected-value) or [median](probability-theory.md#median).

### Concentration of Lipschitz functions on the symmetric group

↑ **Parent:** [Concentration inequality](#concentration-inequality)

Equip the [symmetric group](finite-group-theory.md#symmetric-group) $S_n$ with its uniform [probability measure](probability-theory.md#probability-measure) and unnormalized [Hamming distance](coding-theory.md#hamming-distance). If $f$ has [Lipschitz constant](real-analysis.md#lipschitz-constant) $K$, it obeys the displayed two-sided bound, and each one-sided tail has the same exponential without the factor two. Reveal a uniform [permutation](combinatorics.md#permutation) one image at a time. Two possible next images have completion sets paired by swapping those two values, changing exactly two coordinates. Thus the corresponding conditional means differ by at most $2K$. Each increment of the [Doob exposure martingale](martingale.md#doob-exposure-martingale) has conditional range length at most $2K$. Applying the conditional [Hoeffding lemma](#hoeffding-lemma) gives $\mathbb E e^{\lambda(f-\mathbb Ef)}\leq e^{n\lambda^2K^2/2}$; optimizing the [exponential Markov bound](#exponential-markov-bound) proves the bound. A mere absolute-increment bound of $2K$ gives a weaker constant, so using the range length matters.

### Talagrand convex distance

↑ **Parent:** [Concentration inequality](#concentration-inequality)

For an event $A$ in a product of finitely many [probability spaces](probability-theory.md#probability-space) with its [product measure](probability-theory.md#product-measure), take the closed [convex hull](mathematical-optimization.md#convex-hull) of the mismatch vectors $(\mathbf1_{x_i\ne y_i})_i$, $y\in A$. The distance of this hull from zero is $d_T(x,A)$. Equivalently it is the supremum, over nonnegative coordinate weights of squared sum at most one, of their minimum mismatch sum. Averaging mismatch patterns is the feature that distinguishes this quantity from ordinary Hamming distance.

<h4 id="talagrand-s-convex-distance-inequality">Talagrand's convex distance inequality</h4>

↑ **Parent:** [Talagrand convex distance](#talagrand-convex-distance)

On a finite product of standard [probability spaces](probability-theory.md#probability-space), for any measurable event $A$ of positive probability,

$$
\mathbb E\exp(d_T(X,A)^2/4)\leq1/\mathbb P(A).
$$

Consequently $\mathbb P(A)\mathbb P(d_T(X,A)\geq s)\leq e^{-s^2/4}$. Here $d_T$ is the [Talagrand convex distance](#talagrand-convex-distance). The distance-event conclusion can be read with outer probability when necessary.

##### Section induction for the Talagrand exponential moment

↑ **Parent:** [Talagrand's convex distance inequality](#talagrand-s-convex-distance-inequality)

Let the largest last-coordinate section have probability $a$, and another section probability $ar$. Mix mismatch vectors from these two sections with weights $\lambda,1-\lambda$. Their squared norm is at most $\lambda d_1^2+(1-\lambda)d_2^2+(1-\lambda)^2$. [Hölder's inequality](real-analysis.md#holder-s-inequality) and induction bound that section's exponential integral by $a^{-1}\inf_\lambda r^{-\lambda}e^{(1-\lambda)^2/4}$. The [scalar estimate for Talagrand product induction](#scalar-estimate-for-talagrand-product-induction) makes it at most $(2-r)/a$. Average over sections and use $m(2-m)\le1$ with $m=\Pr(A)/a$ to close the induction.

##### Scalar estimate for Talagrand product induction

↑ **Parent:** [Talagrand's convex distance inequality](#talagrand-s-convex-distance-inequality)

For $a\in[0,1]$,

$$
\inf_{0\leq t\leq1}e^{t^2/4}a^{-(1-t)}\leq2-a,
$$

where the endpoint $t=1$ is used directly if $a=0$. Put $L=-\log a$. For $L\leq1/2$, choose $t=2L$ and [set](set.md) $h(L)=\log(2-e^{-L})-L+L^2$. Then $h(0)=h'(0)=0$ and $h''(L)=2-2e^L/(2e^L-1)^2\geq0$, proving the bound. For $L\geq1/2$, take $t=1$; the result follows from the already proved boundary case and monotonicity of $2-a$. This estimate closes the section-by-section induction for the exponential [Talagrand convex distance](#talagrand-convex-distance) moment.

### Entropy functional

↑ **Parent:** [Concentration inequality](#concentration-inequality)

For a nonnegative integrable random variable $Z$, the entropy functional is

$$
\operatorname{Ent}(Z)
=\mathbb E[Z\log Z]-\mathbb EZ\log\mathbb EZ.
$$

It is the unnormalized [relative entropy](probability-and-statistics.md#kullback-leibler-divergence) of the measure with density proportional to $Z$ relative to the original probability measure.

#### Logarithmic Sobolev inequality

↑ **Parent:** [Entropy functional](#entropy-functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_Sobolev_inequality)

Here $\operatorname{Ent}_\mu(h)=\int h\log h\,d\mu-(\int h\,d\mu)\log\int h\,d\mu$ for a probability measure. The coefficient depends on the normalization of the energy. With the joint energy $-\langle Lg,g\rangle$ for $L=D^2-xD$, standard Gaussian measure has optimal constant two.

// Target: analysis.bigb

##### Logarithmic Sobolev inequality implies hypercontractivity

↑ **Parent:** [Logarithmic Sobolev inequality](#logarithmic-sobolev-inequality)

Differentiate $\log\|u\|_q$ with $u=P_tf$ and a changing exponent. The derivative is $q'\operatorname{Ent}(u^q)/(q^2\int u^q)-\mathcal E(u^{q-1},u)/\int u^q$. Apply the logarithmic Sobolev inequality to $u^{q/2}$ and the [power inequality for symmetric Markov energies](functional-analysis.md#power-inequality-for-symmetric-markov-energies). Choosing $q'=4(q-1)/c_{\mathrm{LS}}$ makes the upper bound zero.

// Target: probability-and-statistics.bigb

### Hoeffding inequality

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hoeffding_inequality)

If independent random variables satisfy $a_i\leq X_i\leq b_i$, then

$$
\mathbb P\left(\sum_i(X_i-\mathbb EX_i)\geq t\right)
\leq\exp\left(-\frac{2t^2}{\sum_i(b_i-a_i)^2}\right),
$$

with the same bound for the lower tail.

#### Hoeffding lemma

↑ **Parent:** [Hoeffding inequality](#hoeffding-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hoeffding_lemma)

If $a\leq X\leq b$ almost surely, then

$$
\log\mathbb E e^{\lambda(X-\mathbb EX)}
\leq\frac{\lambda^2(b-a)^2}{8}.
$$

### Bennett inequality

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bennett_inequality)

If independent centered random variables satisfy $X_i\leq b$ and $\sum_i\mathbb EX_i^2\leq v$, then

$$
\mathbb P\left(\sum_iX_i\geq t\right)
\leq\exp\left[-\frac v{b^2}h\left(\frac{bt}{v}\right)\right],
\qquad h(u)=(1+u)\log(1+u)-u.
$$

#### Bennett bounds for sparse binomial fluctuations

↑ **Parent:** [Bennett inequality](#bennett-inequality)

For a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with $p_n\to0$ and $np_n\to\infty$, the [Bennett inequality](#bennett-inequality) at $C$ standard deviations tends to $2e^{-C^2/2}$, whereas the [Hoeffding inequality](#hoeffding-inequality) tends to two. The raw [Bennett inequality](#bennett-inequality) bound is eventually smaller for any fixed $C>0$; after clipping at one it is nontrivial in the limit only when $C>\sqrt{2\log2}$.

#### Bennett rate function

↑ **Parent:** [Bennett inequality](#bennett-inequality)

The [Bennett rate function](#bennett-rate-function) has [Taylor expansion](calculus.md#taylor-expansion) $\phi(u)=u^2/2-u^3/6+O(u^4)$ near zero. It is the optimized exponent in the [Chernoff bound](#chernoff-bound) based on the [moment-generating function](probability-theory.md#moment-generating-function) estimate for the [Bennett inequality](#bennett-inequality).

<h3 id="poincare-inequality-in-probability-theory">Poincaré inequality in probability theory</h3>

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A probability distribution $\mu$ has Poincaré constant $C_P$ when every sufficiently regular $f$ satisfies

$$
\operatorname{Var}_\mu f\leq C_P\int\lVert\nabla f\rVert^2d\mu.
$$

<h4 id="gaussian-poincare-inequality">Gaussian Poincaré inequality</h4>

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_Poincaré_inequality)

For standard Gaussian measure $\gamma$, the sharp Poincaré constant is one:

$$
\operatorname{Var}_\gamma f\leq\int\lVert\nabla f\rVert^2d\gamma.
$$

<h4 id="tensorization-of-a-poincare-inequality">Tensorization of a Poincaré inequality</h4>

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)

If each probability measure $\mu_i$ has Poincaré constant $C_i$, then the product measure $\bigotimes_i\mu_i$ has Poincaré constant at most $\max_iC_i$. This follows by iterating the [law of total variance](probability-theory.md#law-of-total-variance) and applying [Jensen inequality](real-analysis.md#jensen-s-inequality) to derivatives of conditional expectations.

<h4 id="pushforward-of-a-poincare-inequality-by-a-lipschitz-function">Pushforward of a Poincaré inequality by a Lipschitz function</h4>

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)

If $\mu$ has Poincaré constant $C$ and $\phi$ is $L$-Lipschitz, then the [pushforward measure](measure-theory.md#pushforward-measure) $\phi_*\mu$ has Poincaré constant at most $CL^2$. Apply the original inequality to $g\circ\phi$ and use the [chain rule](calculus.md#chain-rule).

<h4 id="poincare-inequality-for-the-uniform-distribution-on-an-interval">Poincaré inequality for the uniform distribution on an interval</h4>

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)

For the uniform distribution on $[0,1]$,

$$
\operatorname{Var}(f(U))\leq\frac1{\pi^2}\mathbb E[f'(U)^2].
$$

The constant $1/\pi^2$ is sharp and is the mean-zero [Poincare-Wirtinger inequality](sobolev-space.md#poincare-wirtinger-inequality) on the interval.

#### Gaussian logarithmic Sobolev inequality

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_logarithmic_Sobolev_inequality)

For standard Gaussian measure $\gamma$,

$$
\operatorname{Ent}_\gamma(f^2)
\leq2\int\lVert\nabla f\rVert^2d\gamma.
$$

##### Sharpness of the Gaussian logarithmic Sobolev constant

↑ **Parent:** [Gaussian logarithmic Sobolev inequality](#gaussian-logarithmic-sobolev-inequality)

For standard one-dimensional [Gaussian measure](stochastic-process.md#gaussian-measure), $\int e^{sx}\,d\gamma=e^{s^2/2}$. Thus $\operatorname{Ent}_\gamma(e^{sx})=(s^2/2)e^{s^2/2}$, while $\int|(e^{sx/2})'|^2d\gamma=(s^2/4)e^{s^2/2}$. Every nonzero $s$ therefore attains ratio two, proving optimality of the Gaussian constant.

##### Ornstein-Uhlenbeck entropy dissipation identity

↑ **Parent:** [Gaussian logarithmic Sobolev inequality](#gaussian-logarithmic-sobolev-inequality)

For bounded smooth positive $h$ bounded away from zero, differentiation and [Gaussian integration by parts](probability-theory.md#stein-s-lemma-probability) give the displayed identity. The [Ornstein-Uhlenbeck gradient commutation identity](functional-analysis.md#ornstein-uhlenbeck-gradient-commutation-identity) and weighted [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound its right side by $e^{-2t}\int|h'|^2/h\,d\gamma$. Integrating and setting $h=f^2$ proves the [Gaussian logarithmic Sobolev inequality](#gaussian-logarithmic-sobolev-inequality). Positive clipped approximation extends it to functions of finite [Gaussian Dirichlet energy](functional-analysis.md#gaussian-dirichlet-energy).

<h4 id="convex-poincare-inequality">Convex Poincaré inequality</h4>

↑ **Parent:** [Poincaré inequality in probability theory](#poincare-inequality-in-probability-theory)

For independent random variables supported on $[0,1]$ and a differentiable convex function $f$,

$$
\operatorname{Var}(f(X))\leq\mathbb E\lVert\nabla f(X)\rVert^2.
$$

### Chernoff bound

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chernoff_bound)

For every $\lambda>0$, [Markov inequality](#markov-inequality) applied to $e^{\lambda X}$ gives

$$
\mathbb P(X\geq t)\leq e^{-\lambda t}\mathbb E[e^{\lambda X}].
$$

Optimizing over $\lambda$ gives the Chernoff bound in terms of the [moment-generating function](probability-theory.md#moment-generating-function) of $X$.

#### Entrywise concentration of a Gaussian Gram matrix

↑ **Parent:** [Chernoff bound](#chernoff-bound)

For a $d\times p$ matrix of independent standard normal entries and $0<t<1$, diagonal entries of $A^TA/d-I$ have two-sided tails bounded by $2e^{-dt^2/8}$, while off-diagonal entries have tails bounded by $2e^{-dt^2/4}$. A [union bound](#boole-s-inequality) over $p$ diagonal entries and $p(p-1)/2$ distinct off-diagonal entries controls their common [entrywise maximum norm](vector-space.md#entrywise-maximum-norm).

### Bounded differences property

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A [function](function.md) $f(x_1,\ldots,x_n)$ has bounded differences with constants $c_i$ when changing only $x_i$ changes its value by at most $c_i$.

<h4 id="mcdiarmid-s-inequality">McDiarmid's inequality</h4>

↑ **Parent:** [Bounded differences property](#bounded-differences-property)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/McDiarmid's_inequality)

If $X_1,\ldots,X_n$ are [independent random variables](random-variable.md#independent-random-variables) and $f$ has [bounded differences](#bounded-differences-property) constants $c_i$, then

$$
\mathbb P\bigl(f(X)-\mathbb Ef(X)\geq t\bigr)
\leq\exp\left(-\frac{2t^2}{\sum_i c_i^2}\right),
$$

and the same bound holds for the lower tail.

##### Boolean cube expansion from bounded differences

↑ **Parent:** [McDiarmid's inequality](#mcdiarmid-s-inequality)

For a nonempty $A\subseteq\{0,1\}^n$ of relative size at least $\varepsilon\in(0,1]$, its [Hamming distance](coding-theory.md#hamming-distance) [function](function.md) $F(x)=d(x,A)$ has the [bounded differences property](#bounded-differences-property) with all constants one. If $\mu=\mathbb EF$, the concentration bound at $F=0$ gives $\varepsilon\leq2e^{-2\mu^2/n}$, so $\mu\leq t/2$ for $t=\sqrt{2n\log(2/\varepsilon)}$. Then $\Pr(F>t)\leq2e^{-2(t-\mu)^2/n}\leq\varepsilon$, proving that the radius-$t$ neighbourhood contains at least $(1-\varepsilon)2^n$ cube points.

<h4 id="talagrand-s-one-sided-bounded-differences-inequality">Talagrand's one-sided bounded differences inequality</h4>

↑ **Parent:** [Bounded differences property](#bounded-differences-property)

If a function of independent coordinates has one-sided squared-difference proxy at most $v$, Talagrand's one-sided inequality gives a Gaussian lower-tail bound $\mathbb P(Z-\mathbb EZ\leq-t)\leq e^{-t^2/(2v)}$. Applied to the negative of a concave function, it gives the corresponding upper-tail bound.

### Certifiable function

↑ **Parent:** [Concentration inequality](#concentration-inequality)

An integer-valued [function](function.md) $f$ is $g$-certifiable when every input $x$ with $f(x)=k$ has a set of at most $g(k)$ coordinates whose values alone guarantee that $f\geq k$.

#### Entropy method for certifiable functions

↑ **Parent:** [Certifiable function](#certifiable-function)

The entropy method combines a coordinatewise certificate with [tensorization of entropy](#tensorization-of-entropy) to bound the [moment-generating function](probability-theory.md#moment-generating-function) of a certifiable random quantity and hence its tails.

### Self-bounding function

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A nonnegative [function](function.md) $f$ of independent coordinates is self-bounding when there are coordinate-deleted versions $f_i$ such that $0\leq f-f_i\leq1$ and

$$
\sum_i(f-f_i)\leq f.
$$

These inequalities make the natural variance proxy no larger than the function itself.

#### Weakly self-bounding function

↑ **Parent:** [Self-bounding function](#self-bounding-function)

A nonnegative function $f$ is weakly self-bounding when coordinate-deleted functions $f_i$ satisfy $f_i\leq f$ and

$$
\sum_i(f-f_i)^2\leq f.
$$

The squared coordinate sensitivity is then controlled by the observed value of the function itself.

##### Variance bound for a weakly self-bounding function

↑ **Parent:** [Weakly self-bounding function](#weakly-self-bounding-function)

For a weakly self-bounding function $Z=f(X_1,\ldots,X_n)$ of [independent random variables](random-variable.md#independent-random-variables), the coordinatewise variance inequality gives

$$
\operatorname{Var}(Z)\leq\mathbb E\sum_i(Z-Z_i)^2\leq\mathbb EZ,
$$

where $Z_i=f_i(X^{(i)})$.

##### Lower-tail concentration for a weakly self-bounding function

↑ **Parent:** [Weakly self-bounding function](#weakly-self-bounding-function)

The entropy method gives

$$
\log\mathbb E e^{-\lambda(Z-\mathbb EZ)}
\leq\frac{\lambda^2\mathbb EZ}{2}
$$

for $\lambda\geq0$. Consequently the [Chernoff bound](#chernoff-bound) yields $\mathbb P(Z-\mathbb EZ\leq-t)\leq\exp[-t^2/(2\mathbb EZ)]$.

### Tensorization of entropy

↑ **Parent:** [Concentration inequality](#concentration-inequality)

For a nonnegative [function](function.md) $Z$ of [independent random variables](random-variable.md#independent-random-variables), entropy is at most the sum of its conditional coordinate entropies. This tensorization is a basic step of the [entropy method](#entropy-method-for-certifiable-functions).

<h3 id="efron-stein-inequality">Efron–Stein inequality</h3>

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Efron–Stein_inequality)

If $Z=f(X_1,\ldots,X_n)$ for independent coordinates and $Z_i'$ replaces $X_i$ by an independent copy, then

$$
\operatorname{Var}(Z)\leq\frac12\sum_i\mathbb E(Z-Z_i')^2.
$$

#### Variance tensorization

↑ **Parent:** [Efron–Stein inequality](#efron-stein-inequality)

For independent coordinates $X_1,\ldots,X_n$ and square-integrable $f$,

$$
\operatorname{Var}f(X)
\leq\sum_i\mathbb E\!\left[\operatorname{Var}(f(X)\mid X_j,\ j\ne i)\right].
$$

For Bernoulli coordinates, each conditional variance is an explicit squared coordinate difference.

### Modified logarithmic Sobolev inequality

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A modified logarithmic Sobolev inequality bounds the entropy of $e^{\lambda Z}$ by a one-sided coordinate-difference energy. For independent coordinates and arbitrary coordinate-deleted functions $f_i$, tensorization gives

$$
\operatorname{Ent}(e^{\lambda f})
\leq\mathbb E\left[e^{\lambda f}\sum_i
\phi\bigl(-\lambda(f-f_i)\bigr)\right],
\qquad \phi(u)=e^u-u-1.
$$

If that energy is at most $v$, one common normalization is

$$
\operatorname{Ent}(e^{\lambda Z})\leq\frac{\lambda^2v}{2}\mathbb Ee^{\lambda Z}.
$$

#### Herbst argument

↑ **Parent:** [Modified logarithmic Sobolev inequality](#modified-logarithmic-sobolev-inequality)

The Herbst argument integrates a logarithmic Sobolev bound on $\lambda H'(\lambda)-H(\lambda)$ to control the centered cumulant-generating function $H$, then applies a [Chernoff bound](#chernoff-bound) to obtain concentration.

### Transport-entropy inequality

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A transport-entropy inequality controls an optimal expected transportation cost between [probability distributions](probability-theory.md#probability-distribution) by their [Kullback-Leibler divergence](probability-and-statistics.md#kullback-leibler-divergence).

#### Tensorization of a transport-entropy inequality

↑ **Parent:** [Transport-entropy inequality](#transport-entropy-inequality)

If each coordinate law satisfies the same convex [transport-entropy inequality](#transport-entropy-inequality), then the product law satisfies the sum-cost version. Sequentially couple conditional coordinates, apply [Jensen inequality](real-analysis.md#jensen-s-inequality), and use the [chain rule for relative entropy](probability-and-statistics.md#chain-rule-for-relative-entropy).

### Sub-Poisson random variable in the right tail

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A centered [random variable](random-variable.md) $X$ is sub-Poisson in the right tail with variance parameter $\sigma^2$ when

$$
\log\mathbb E e^{\lambda X}\leq\sigma^2(e^\lambda-\lambda-1)
$$

for every $\lambda\geq0$.

### Sub-Gamma random variable in the right tail

↑ **Parent:** [Concentration inequality](#concentration-inequality)

A centered [random variable](random-variable.md) $X$ is sub-Gamma in the right tail with variance parameter $v$ and scale parameter $c$ when

$$
\log\mathbb E e^{\lambda X}\leq\frac{v\lambda^2}{2(1-c\lambda)}
$$

for $0\leq\lambda<c^{-1}$.

#### Bernstein inequalities (probability theory)

↑ **Parent:** [Sub-Gamma random variable in the right tail](#sub-gamma-random-variable-in-the-right-tail)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernstein_inequalities_(probability_theory))

For independent centered variables $X_i\leq b$ and $v=\sum_i\mathbb EX_i^2$,

$$
\mathbb P\left(\sum_iX_i\geq t\right)
\leq\exp\left(-\frac{t^2}{2(v+bt/3)}\right).
$$

##### Bernstein bound for independent sub-exponential variables

↑ **Parent:** [Bernstein inequalities (probability theory)](#bernstein-inequalities-probability-theory)

Suppose independent centered [sub-exponential random variables](probability-and-statistics.md#subexponential-distribution-light-tailed) satisfy $\log\mathbb E e^{\lambda X_i}\leq v_i\lambda^2/(2(1-b|\lambda|))$ for $|\lambda|<1/b$, and put $v=\sum_iv_i$. Independence adds the log [moment-generating functions](probability-theory.md#moment-generating-function). The [Chernoff bound](#chernoff-bound) with $\lambda=t/(v+bt)$ gives the displayed two-sided tail. If each variable has common scale $K$, one may take $v_i\leq CK^2$ and $b\leq CK$, giving $\mathbb P(|n^{-1}\sum_iX_i|>t)\leq2e^{-c n\min\{t^2/K^2,t/K\}}$. This form of [Bernstein's inequality](#bernstein-inequalities-probability-theory) allows unbounded variables with factorial moment control, including the [centered square of a sub-Gaussian random variable](probability-and-statistics.md#centered-square-of-a-sub-gaussian-random-variable).

### Rosenthal inequality

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rosenthal_inequality)

For independent centered variables and $p\geq2$, the $p$th moment of their sum is bounded, up to a constant depending only on $p$, by the sum of their $p$th moments plus the $p/2$ power of their total variance.

<h3 id="talagrand-s-concentration-inequality">Talagrand's concentration inequality</h3>

↑ **Parent:** [Concentration inequality](#concentration-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Talagrand's_concentration_inequality)

[Talagrand's concentration inequality](#talagrand-s-concentration-inequality) gives strong concentration in product spaces using convex distance. If $A$ has positive product probability, its convex-distance enlargement has Gaussian tails. A [Talagrand concentration inequality for certifiable functions](#talagrand-concentration-inequality-for-certifiable-functions) follows by bounding this distance using bounded differences and small certificates.

#### Talagrand concentration inequality for certifiable functions

↑ **Parent:** [Talagrand's concentration inequality](#talagrand-s-concentration-inequality)

This is an application of [Talagrand's concentration inequality](#talagrand-s-concentration-inequality) to [certifiable functions](#certifiable-function). Talagrand's product-space inequality gives sub-Gaussian-type concentration for a [bounded-differences](#bounded-differences-property), [certifiable function](#certifiable-function), with a variance scale controlled by the certificate size.

##### Two-threshold concentration for certifiable functions

↑ **Parent:** [Talagrand concentration inequality for certifiable functions](#talagrand-concentration-inequality-for-certifiable-functions)

Suppose an integer-valued [certifiable function](#certifiable-function) is $L$-Lipschitz under one-coordinate changes and a value at least $b$ has a certificate of at most $rb$ coordinates. Any input with value at most $a<b$ must differ on at least $(b-a)/L$ certificate positions. Equal weights on those positions bound its [Talagrand convex distance](#talagrand-convex-distance) from the low-value event. Applying [Talagrand's convex distance inequality](#talagrand-s-convex-distance-inequality) gives the displayed product bound. For $0\le Z\le D$, median tails integrate to $|\mathbb EZ-\operatorname{med}Z|=O(L\sqrt{rD})$, and deviations of order $D$ have exponentially small probability.

##### Increasing-subsequence certificate concentration

↑ **Parent:** [Talagrand concentration inequality for certifiable functions](#talagrand-concentration-inequality-for-certifiable-functions)

For the [longest increasing subsequence](combinatorics.md#longest-increasing-subsequence) length $L$ on a product space of independent coordinates, a witness of length $\ell$ uses only $\ell$ coordinates. Any point with subsequence length at most $a$ must differ on at least $\ell-a$ witness positions. Weights $1/\sqrt\ell$ on those positions show $d_T(x,\{L\leq a\})\geq(\ell-a)/\sqrt\ell$. Thus for $0\leq a<b$,

$$
\Pr(L\leq a)\Pr(L\geq b)\leq e^{-(b-a)^2/(4b)}.
$$

At a [median](probability-theory.md#median) $m$, this gives upper tail $2e^{-t^2/[4(m+t)]}$ and lower tail $2e^{-t^2/(4m)}$. Integrating the tails places the mean within $O(\sqrt m+1)$ of the [median](probability-theory.md#median), so the natural concentration scale near the mean is $\sqrt{\mathbb EL}$. A random permutation is represented by the ranks of independent continuous variables; arbitrary dependent sequences need not obey this conclusion.

<h2 id="boole-s-inequality">Boole's inequality</h2>

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boole's_inequality)

The union bound says $P(\bigcup_i A_i)\le\sum_iP(A_i)$.

### Positive common intersection from pair-intersection probabilities

↑ **Parent:** [Boole's inequality](#boole-s-inequality)

For $n\geq2$, the intersection of all pairwise intersections $A_i\cap A_j$ is $\bigcap_iA_i$. Apply the [union bound](#boole-s-inequality) to the complements of the pairwise intersections and then take the complement to obtain the displayed lower bound. A sum exceeding $\binom n2-1$ therefore forces positive common probability without any [independence](random-variable.md#independent-random-variables) assumption.

## FKG inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/FKG_inequality)

The FKG inequality gives positive association under a log-supermodular probability measure on a finite distributive lattice.

### FKG lattice condition

↑ **Parent:** [FKG inequality](#fkg-inequality)

This lattice condition on configuration masses is the hypothesis of the [FKG inequality](#fkg-inequality). A [product measure](probability-theory.md#product-measure) on a finite Boolean lattice satisfies it with equality, since in each coordinate the minimum and maximum retain the original two coordinate values. It implies [positive association of random variables](probability-theory.md#positive-association-of-random-variables) for increasing functions.

#### Exponential-tilt proof of positive association

↑ **Parent:** [FKG lattice condition](#fkg-lattice-condition)

For a strictly positive law $\mu$ satisfying the [FKG lattice condition](#fkg-lattice-condition) on a finite Boolean lattice, and an increasing function $g$, tilt to $\mu_t(\omega)\propto e^{tg(\omega)}\mu(\omega)$. For $t\ge0$, the lattice inequality and $g(\omega\vee\eta)\ge g(\omega)$ give the [Holley condition](probability-and-statistics.md#holley-condition) for $\mu_t\ge_{\mathrm{st}}\mu$. For any increasing $f$, differentiate $\mathbb E_{\mu_t}f\ge\mathbb E_\mu f$ at $t=0$ from the right. The derivative is $\operatorname{Cov}_\mu(f,g)$, proving [positive association of random variables](probability-theory.md#positive-association-of-random-variables).

### Harris-FKG inequality

↑ **Parent:** [FKG inequality](#fkg-inequality)

Increasing events under a product probability measure are positively associated: $\mathbb P(A\cap B)\geq\mathbb P(A)\mathbb P(B)$.

#### Square-root bound for increasing events

↑ **Parent:** [Harris-FKG inequality](#harris-fkg-inequality)

For two [increasing events](#increasing-event) of equal [probability](probability-theory.md#probability) $a$ under a [product measure](probability-theory.md#product-measure), positive association of their complements gives $1-P(A\cup B)\ge(1-a)^2$. Hence $a\ge1-\sqrt{1-P(A\cup B)}$. For $r$ equal-probability [increasing events](#increasing-event), the same reasoning gives $a\ge1-(1-P(\bigcup_jA_j))^{1/r}$.

#### Square-root trick for positively associated events

↑ **Parent:** [Harris-FKG inequality](#harris-fkg-inequality)

If [increasing events](#increasing-event) $A_1,\ldots,A_k$ have a common probability, applying the [Harris-FKG inequality](#harris-fkg-inequality) to their decreasing complements gives $\mathbb P(A_1)\geq1-(1-\mathbb P(\bigcup_iA_i))^{1/k}$.

#### Harris' inequality

↑ **Parent:** [Harris-FKG inequality](#harris-fkg-inequality)

Harris' inequality states that two increasing events under an independent Bernoulli product measure are positively correlated.

##### Negative correlation of increasing and decreasing events

↑ **Parent:** [Harris' inequality](#harris-inequality)

Under a [product measure](probability-theory.md#product-measure) on a finite [Boolean lattice](extremal-set-theory.md#boolean-lattice), an [increasing event](#increasing-event) $E$ and a [decreasing event](#decreasing-event) $G$ obey the displayed inequality. The complement $G^c$ is an [increasing event](#increasing-event), so [Harris' inequality](#harris-inequality) gives $\mathbb P(E\cap G^c)\geq\mathbb P(E)\mathbb P(G^c)$. Subtract from $\mathbb P(E)$ to obtain the result. This implication includes degenerate [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) parameters $0$ and $1$.

##### Increasing event

↑ **Parent:** [Harris' inequality](#harris-inequality)

An event in a partially ordered configuration space is increasing when changing coordinates upward cannot make a configuration leave the event.

###### Sharp threshold

↑ **Parent:** [Increasing event](#increasing-event)

For a sequence of nontrivial [increasing events](#increasing-event) on finite [product measures](probability-theory.md#product-measure), write $p_x$ for the parameter at which the success probability is $x$. An additive sharp threshold means that $p_{1-\varepsilon}-p_\varepsilon\to0$ for every fixed $0<\varepsilon<1/2$. When the threshold parameter itself tends to zero, relative sharpness instead compares this window with $p_{1/2}$; additive sharpness alone is then a weaker assertion. The [Friedgut-Kalai sharp threshold theorem](combinatorics.md#friedgut-kalai-sharp-threshold-theorem) provides an explicit additive bound for [transitive increasing events](#transitive-increasing-event).

###### Transitive increasing event

↑ **Parent:** [Increasing event](#increasing-event)

An [increasing event](#increasing-event) on a finite product of identically distributed coordinates is transitive if a [group action](group-theory.md#group-action) preserving the event is transitive on the coordinate set. Its [influences](combinatorics.md#influence-of-a-variable) are all equal. Transitivity concerns coordinates, and does not assert transitivity on successful configurations.

###### Decreasing event

↑ **Parent:** [Increasing event](#increasing-event)

An event is decreasing when closing additional edges cannot destroy it. Its complement is an [increasing event](#increasing-event).

## Janson inequality

↑ **Parent:** [Probability inequality](probability-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Janson_inequality)

For increasing containment events $A_i$ in a Bernoulli product space, let $X=\sum_i\mathbf1_{A_i}$, $\mu=\mathbb EX$, and

$$
\Delta=\sum_{i\ne j:\,A_i\sim A_j}\mathbb P(A_i\cap A_j),
$$

where the sum is ordered and dependency means overlapping coordinate supports. Then

$$
\mathbb P(X=0)\leq e^{-\mu+\Delta/2}.
$$

In particular it is at most $e^{-\mu/2}$ when $\Delta\leq\mu$, and at most $e^{-\mu^2/(2\Delta)}$ when $\Delta\geq\mu$.

### Janson lower-tail bound by independent thinning

↑ **Parent:** [Janson inequality](#janson-inequality)

For increasing containment indicators, attach independent Bernoulli selectors of parameter $t$. [Janson inequality](#janson-inequality) applied to the selected events gives $\mathbb E(1-t)^X\le\exp(-t\mu+t^2\Delta/2)$. Set $t=1-e^{-s}$ and apply the [exponential Markov bound](#exponential-markov-bound). The estimates $s-s^2/2\le1-e^{-s}\le s$ give exponent at most $-sa+s^2(\mu+\Delta)/2$. Optimizing at $s=a/(\mu+\Delta)$ proves the displayed lower-tail bound, with the dependency sum ordered and excluding the diagonal.

### Janson dependency sum

↑ **Parent:** [Janson inequality](#janson-inequality)

The Janson dependency sum adds $\mathbb P(A_i\cap A_j)$ over ordered pairs of distinct containment events whose coordinate supports overlap.

### Janson sequential product lemma

↑ **Parent:** [Janson inequality](#janson-inequality)

For containment-event indicators $I_1,\ldots,I_m$ in a Bernoulli product space,

$$
\mathbb P(I_1=\cdots=I_m=0)
\leq
\prod_i\left(1-\mathbb EI_i+\sum_{j<i:j\sim i}\mathbb E(I_iI_j)\right).
$$

It follows by exposing the avoidance events in sequence, separating disjoint coordinate supports, and applying [Harris' inequality](#harris-inequality) to the remaining decreasing events.

<h2 id="levy-maximal-inequality">Lévy maximal inequality</h2>

↑ **Parent:** [Probability inequality](probability-inequality.md)

For independent symmetric random variables in a normed vector space and partial sums $S_k$,

$$
\mathbb P\left(\max_{k\leq n}\lVert S_k\rVert>t\right)
\leq2\mathbb P(\lVert S_n\rVert>t).
$$

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
