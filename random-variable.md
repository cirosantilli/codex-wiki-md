# Random variable

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_variable)

A random variable is a measurable [function](function.md) from a probability space to a measurable space.

**Table of contents**

- [Random element](#random-element)
- [Statistical dependence](#statistical-dependence)
- [Random sum](#random-sum)
  - [Transform composition for an independent random sum](#transform-composition-for-an-independent-random-sum)
- [Discrete random variable](#discrete-random-variable)
- [Random vector](#random-vector)
- [Hilbert-space-valued random variable](#hilbert-space-valued-random-variable)
  - [Covariance operator](#covariance-operator)
    - [Covariance kernel](#covariance-kernel)
      - [Brownian covariance kernel](#brownian-covariance-kernel)
        - [Brownian covariance from an integrated orthonormal basis](#brownian-covariance-from-an-integrated-orthonormal-basis)
      - [Brownian bridge covariance kernel](#brownian-bridge-covariance-kernel)
    - [Empirical covariance operator](#empirical-covariance-operator)
      - [Pooled covariance operator](#pooled-covariance-operator)
  - [Gaussian random element](#gaussian-random-element)
- [Independent random variables](#independent-random-variables)
  - [Pairwise independent random variables](#pairwise-independent-random-variables)
  - [Conditional independence](#conditional-independence)
    - [Covariance induced by a shared latent variable](#covariance-induced-by-a-shared-latent-variable)
    - [Conditional independence graph](#conditional-independence-graph)
      - [Nodewise regression](#nodewise-regression)
        - [Profiling intercepts in nodewise regression](#profiling-intercepts-in-nodewise-regression)
        - [AND rule for nodewise graph selection](#and-rule-for-nodewise-graph-selection)
        - [OR rule for nodewise graph selection](#or-rule-for-nodewise-graph-selection)
      - [Gaussian graphical model](#gaussian-graphical-model)
      - [Neighbourhood selection](#neighbourhood-selection)
      - [Moral graph equals the conditional independence graph under faithfulness](#moral-graph-equals-the-conditional-independence-graph-under-faithfulness)
    - [Contraction axiom for conditional independence](#contraction-axiom-for-conditional-independence)
    - [Decomposition axiom for conditional independence](#decomposition-axiom-for-conditional-independence)
    - [Generalized covariance measure statistic](#generalized-covariance-measure-statistic)
      - [Studentization of the generalized covariance measure statistic](#studentization-of-the-generalized-covariance-measure-statistic)
  - [Orthogonality of independent centered Hilbert-space random variables](#orthogonality-of-independent-centered-hilbert-space-random-variables)
  - [Independent and identically distributed random variables](#independent-and-identically-distributed-random-variables)

## Random element

↑ **Parent:** [Random variable](random-variable.md)

A random element is a [measurable function](measure-theory.md#measurable-function) from a [probability space](probability-theory.md#probability-space) $(\Omega,\mathcal F,\mathbb P)$ to a [measurable space](measure-theory.md#measurable-space) $(E,\mathcal E)$. Its law is the [pushforward measure](measure-theory.md#pushforward-measure) $\mathbb P_X(A)=\mathbb P(X^{-1}(A))$ for $A\in\mathcal E$. Real-valued [random variables](random-variable.md) and vector-valued random variables are examples; a stochastic sample path can also be a random element when its path-space sigma-algebra is specified. For a [Polish space](topological-analysis.md#polish-space) $E$, the usual choice is its [Borel sigma-algebra](measure-theory.md#borel-sigma-algebra). A [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) concerns the laws of a family of such random elements.

## Statistical dependence

↑ **Parent:** [Random variable](random-variable.md)

Two [random variables](random-variable.md) are statistically dependent when their joint [probability distribution](probability-theory.md#probability-distribution) differs from the product of their marginal [probability distributions](probability-theory.md#probability-distribution). Equivalently, some events determined by the two variables violate the product rule that defines [independence](#independent-random-variables). Nonzero [covariance](variance.md#covariance) implies statistical dependence when the moments exist, but zero [covariance](variance.md#covariance) does not in general imply [independence](#independent-random-variables).

## Random sum

↑ **Parent:** [Random variable](random-variable.md)

A [random sum](#random-sum) has a random number $N$ of summands, usually with $N$ a nonnegative integer-valued [random variable](random-variable.md). The empty sum is zero. The dependence between $N$ and the summands must be stated; independent summands do not by themselves imply independence from $N$.

### Transform composition for an independent random sum

↑ **Parent:** [Random sum](#random-sum)

For independent identically distributed summands, independent also of the count $N$, conditioning on $N=n$ gives $\mathbb E[e^{tZ}\mid N=n]=M_Y(t)^n$. The [law of total expectation](measure-theory.md#law-of-total-expectation) gives the composition of the count's [probability generating function](probability-theory.md#probability-generating-function) with the summand's [moment-generating function](probability-theory.md#moment-generating-function). This identity is valid as an extended nonnegative expectation; finiteness near zero requires additional exponential-integrability assumptions.

## Discrete random variable

↑ **Parent:** [Random variable](random-variable.md)

A [random variable](random-variable.md) supported on a finite or countable subset of the real line. Its law is specified by a [probability mass function](probability-theory.md#probability-mass-function). Countable support need not consist of integers: a variable constantly equal to $3/2$ is discrete. Integer-indexed [tail-sum formulas](probability-theory.md#tail-sum-formula) therefore require a separate integer-valued hypothesis.

## Random vector

↑ **Parent:** [Random variable](random-variable.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_vector)

A random vector is a [random variable](random-variable.md) whose values are vectors or, equivalently, an ordered tuple of scalar random variables on one probability space.

## Hilbert-space-valued random variable

↑ **Parent:** [Random variable](random-variable.md)

A Hilbert-space-valued random variable is a measurable map into a [Hilbert space](hilbert-space.md). It is square-integrable when $\mathbb E\lVert X\rVert^2<\infty$, in which case its mean is defined by the [Bochner integral](measure-theory.md#bochner-integral).

### Covariance operator

↑ **Parent:** [Hilbert-space-valued random variable](#hilbert-space-valued-random-variable)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covariance_operator)

For a square-integrable centered [Hilbert-space-valued random variable](#hilbert-space-valued-random-variable) $X$, its covariance operator is

$$
C_Xh=\mathbb E[\langle X,h\rangle X]=\mathbb E[X\otimes X]h.
$$

It is a positive self-adjoint [trace-class operator](compact-operator.md#trace-class-operator), and $\operatorname{tr}C_X=\mathbb E\lVert X\rVert^2$.

#### Covariance kernel

↑ **Parent:** [Covariance operator](#covariance-operator)

When a [covariance operator](#covariance-operator) on a function space is an [integral operator](functional-analysis.md#integral-operator), its covariance kernel satisfies $(C_Xf)(s)=\int c_X(s,t)f(t)dt$. For a centered process, $c_X(s,t)=\mathbb E[X(s)X(t)]$ whenever point evaluation is meaningful.

##### Brownian covariance kernel

↑ **Parent:** [Covariance kernel](#covariance-kernel)

The covariance kernel of standard [Brownian motion](brownian-motion.md) on $[0,1]$ is $c(s,t)=\min(s,t)$. Its integral operator has eigenfunctions $\sqrt2\sin((k-\tfrac12)\pi t)$ and eigenvalues $((k-\tfrac12)\pi)^{-2}$.

###### Brownian covariance from an integrated orthonormal basis

↑ **Parent:** [Brownian covariance kernel](#brownian-covariance-kernel)

For a complete [orthonormal basis](linear-algebra.md#orthonormal-basis) of $L^2(\mathbb R_+)$, the [Parseval identity for a Hilbertian basis](hilbert-space.md#parseval-identity-for-a-hilbertian-basis) identifies the sum of the feature products with $\langle1_{[0,s]},1_{[0,t]}\rangle=\min(s,t)$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives absolute convergence.

##### Brownian bridge covariance kernel

↑ **Parent:** [Covariance kernel](#covariance-kernel)

The covariance kernel of a standard [Brownian bridge](brownian-motion.md#brownian-bridge) on $[0,1]$ is $c(s,t)=\min(s,t)-st$. Its integral operator has eigenfunctions $\sqrt2\sin(k\pi t)$ and eigenvalues $(k\pi)^{-2}$ for $k\geq1$.

#### Empirical covariance operator

↑ **Parent:** [Covariance operator](#covariance-operator)

For observations $X_1,\ldots,X_n$ and a chosen center $m$, the empirical covariance operator is $\widehat C_m=n^{-1}\sum_i(X_i-m)\otimes(X_i-m)$. Its expectation equals the population covariance plus the rank-one operator formed from the centering error.

##### Pooled covariance operator

↑ **Parent:** [Empirical covariance operator](#empirical-covariance-operator)

A pooled covariance operator averages the within-group empirical covariance operators from several samples that are assumed to share one population covariance. Centering within each group prevents differences between group means from contaminating the covariance estimate.

### Gaussian random element

↑ **Parent:** [Hilbert-space-valued random variable](#hilbert-space-valued-random-variable)

A random element $G$ of a [Hilbert space](hilbert-space.md) is Gaussian when every continuous linear functional of $G$ has a [normal distribution](probability-theory.md#normal-distribution). Its mean and [covariance operator](#covariance-operator) determine its distribution.

## Independent random variables

↑ **Parent:** [Random variable](random-variable.md)

Random variables $X_1,\ldots,X_n$ are independent when their generated sigma-algebras are [independent sigma-algebras](probability-theory.md#independent-sigma-algebras). Equivalently, their joint distribution is the product of their marginal distributions.

### Pairwise independent random variables

↑ **Parent:** [Independent random variables](#independent-random-variables)

Random variables are pairwise independent when every two distinct members are independent. This is weaker than joint independence, but it is enough to make all off-diagonal covariances vanish for square-integrable variables.

### Conditional independence

↑ **Parent:** [Independent random variables](#independent-random-variables)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_independence)

Random variables $X$ and $Y$ are conditionally independent given $Z$ when their conditional joint distribution factorizes into their two conditional marginal distributions almost surely.

#### Covariance induced by a shared latent variable

↑ **Parent:** [Conditional independence](#conditional-independence)

Let $A,B$ be [indicator random variables](probability-theory.md#indicator-random-variable) with [conditional independence](#conditional-independence) given a [random variable](random-variable.md) $T$, and suppose $\mathbb E[A\mid T]=\mathbb E[B\mid T]=g(T)$. Then the [law of total expectation](measure-theory.md#law-of-total-expectation) gives $\mathbb E[AB]=\mathbb E[g(T)^2]$ and $\mathbb E[A]=\mathbb E[B]=\mathbb E[g(T)]$. Thus their [covariance](variance.md#covariance) is the [variance](variance.md) of $g(T)$ and is nonnegative. The result explains correlated component evolutionary states in a [coeval binary population](stellar-astrophysics.md#coeval-binary-population) without correlation between initial masses.

#### Conditional independence graph

↑ **Parent:** [Conditional independence](#conditional-independence)

For a random vector indexed by vertices $V$, its conditional independence graph is the undirected graph with $u-v$ absent exactly when $Z_u\perp Z_v\mid Z_{V\setminus\{u,v\}}$. In a nonsingular [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), its edges are the nonzero off-diagonal entries of the [precision matrix](variance.md#precision-matrix).

##### Nodewise regression

↑ **Parent:** [Conditional independence graph](#conditional-independence-graph)

Fit the conditional law of each variable given all others and use its predictor support to estimate its neighbours. In a [Gaussian graphical model](#gaussian-graphical-model), this is linear regression with coefficients given by [conditional regression coefficients from a Gaussian precision matrix](variance.md#conditional-regression-coefficients-from-a-gaussian-precision-matrix). The [Nodewise Lasso](probability-and-statistics.md#nodewise-lasso) supplies sparse fits; the [OR rule for nodewise graph selection](#or-rule-for-nodewise-graph-selection) and [AND rule for nodewise graph selection](#and-rule-for-nodewise-graph-selection) combine possibly disagreeing directional supports into an undirected graph.

###### Profiling intercepts in nodewise regression

↑ **Parent:** [Nodewise regression](#nodewise-regression)

Minimizing the squared error over each free regression intercept gives the displayed formula. Substitution replaces all data columns by centred columns. The regression intercept is generally not the marginal mean of the response when predictor means are nonzero; the distinction matters in [conditional regression coefficients from a Gaussian precision matrix](variance.md#conditional-regression-coefficients-from-a-gaussian-precision-matrix).

###### AND rule for nodewise graph selection

↑ **Parent:** [Nodewise regression](#nodewise-regression)

The intersection rule retains an edge only when both directions of [nodewise regression](#nodewise-regression) select it. It is more conservative than the [OR rule for nodewise graph selection](#or-rule-for-nodewise-graph-selection); the distinction matters because separate finite-sample fits can disagree.

###### OR rule for nodewise graph selection

↑ **Parent:** [Nodewise regression](#nodewise-regression)

The union rule retains an edge whenever either of the two [nodewise regression](#nodewise-regression) fits selects the other variable. It is more inclusive than the [AND rule for nodewise graph selection](#and-rule-for-nodewise-graph-selection) and makes an undirected edge decision from potentially asymmetric estimated neighbourhoods.

##### Gaussian graphical model

↑ **Parent:** [Conditional independence graph](#conditional-independence-graph)

For a nondegenerate [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), the [conditional independence graph](#conditional-independence-graph) is read from zeros in its [precision matrix](variance.md#precision-matrix). Conditional independence of two components given all others is equivalent to a zero cross term in their conditional Gaussian quadratic density, hence to $\Omega_{jk}=0$. It does not generally correspond to a zero in the [covariance matrix](variance.md#covariance-matrix).

##### Neighbourhood selection

↑ **Parent:** [Conditional independence graph](#conditional-independence-graph)

For Gaussian data, regress each variable on all remaining variables using [Lasso](probability-and-statistics.md#lasso). Nonzero coefficients estimate its neighbours in the [conditional independence graph](#conditional-independence-graph). Symmetrize the separate regressions using either the union or the intersection of their selected directed neighbourhoods.

##### Moral graph equals the conditional independence graph under faithfulness

↑ **Parent:** [Conditional independence graph](#conditional-independence-graph)

If [D-separation](combinatorics.md#d-separation) and [conditional independence](#conditional-independence) are equivalent for a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph), its [moral graph](combinatorics.md#moral-graph) is its [conditional independence graph](#conditional-independence-graph). After conditioning on all other vertices, an active path can only be a direct edge or a two-edge collider through a common child: two adjacent interior vertices cannot both be colliders. These are exactly the moral edges.

#### Contraction axiom for conditional independence

↑ **Parent:** [Conditional independence](#conditional-independence)

The contraction axiom says that

$$
X\perp Y\mid Z
\quad\text{and}\quad
X\perp W\mid(Y,Z)
\quad\Longrightarrow\quad
X\perp(Y,W)\mid Z.
$$

It follows directly by multiplying the corresponding conditional-density factorizations.

#### Decomposition axiom for conditional independence

↑ **Parent:** [Conditional independence](#conditional-independence)

The decomposition axiom says that $X\perp(Y,W)\mid Z$ implies both $X\perp Y\mid Z$ and $X\perp W\mid Z$. It follows by marginalizing the joint conditional distribution over the discarded variable.

#### Generalized covariance measure statistic

↑ **Parent:** [Conditional independence](#conditional-independence)

To test $X\mathrel{\perp\!\!\!\perp}Y\mid Z$, regress $X$ and $Y$ on $Z$ and average the products of their residuals. Dividing the scaled average by its empirical second moment produces the generalized covariance measure statistic. Small mean-square nuisance-regression errors and a product-rate condition make it asymptotically pivotal.

##### Studentization of the generalized covariance measure statistic

↑ **Parent:** [Generalized covariance measure statistic](#generalized-covariance-measure-statistic)

If the numerator of the [generalized covariance measure statistic](#generalized-covariance-measure-statistic) obeys a [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) with variance $\mathbb E(\varepsilon^2\xi^2)$ and its empirical residual-product second moment converges in probability to the same positive quantity, the [Slutsky theorem](statistical-inference.md#slutsky-theorem) makes the studentized statistic converge in distribution to $N(0,1)$.

### Orthogonality of independent centered Hilbert-space random variables

↑ **Parent:** [Independent random variables](#independent-random-variables)

If $X_i$ are independent centered square-integrable random variables in a Hilbert space, then $\mathbb E\langle X_i,X_j\rangle=0$ for $i\ne j$, and hence

$$
\mathbb E\left\lVert\sum_iX_i\right\rVert^2
=\sum_i\mathbb E\lVert X_i\rVert^2.
$$

### Independent and identically distributed random variables

↑ **Parent:** [Independent random variables](#independent-random-variables)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables)

A family of [independent random variables](#independent-random-variables) is independent and identically distributed when every variable has the same [probability distribution](probability-theory.md#probability-distribution).

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (210)

- [Absolute moment](probability-theory.md#absolute-moment)
- [Bayesian network](statistical-model.md#bayesian-network)
- [Bernoulli coupling by a shared uniform random variable](probability-and-statistics.md#bernoulli-coupling-by-a-shared-uniform-random-variable)
- [Bernstein moment condition](probability-and-statistics.md#bernstein-moment-condition)
- [Boundedness in probability](convergence-of-random-variables.md#boundedness-in-probability)
- [Canonical pseudometric of a Gaussian process](stochastic-process.md#canonical-pseudometric-of-a-gaussian-process)
- [Cantelli inequality](probability-inequality.md#cantelli-inequality)
- [Cauchy random variable](probability-theory.md#cauchy-random-variable)
- [Characteristic function](probability-theory.md#characteristic-function)
- [Complex covariance](variance.md#complex-covariance)
- [Composition of absolutely summable time-series filters](time-series.md#composition-of-absolutely-summable-time-series-filters)
- [Concentration inequality](probability-inequality.md#concentration-inequality)
- [Conditional characteristic function](probability-theory.md#conditional-characteristic-function)
- [Conditional expectation preserving a distribution](measure-theory.md#conditional-expectation-preserving-a-distribution)
- [Conditional Jensen inequality](measure-theory.md#conditional-jensen-inequality)
- [Contingent claim payoff](mathematical-finance.md#contingent-claim-payoff)
- [Control variates](probability-and-statistics.md#control-variates)
- [Covariance criterion for diversification of factor residuals](mathematical-finance.md#covariance-criterion-for-diversification-of-factor-residuals)
- [Covariance induced by a shared latent variable](#covariance-induced-by-a-shared-latent-variable)
- [Cumulative distribution function](probability-theory.md#cumulative-distribution-function)
- [Cylindrical Brownian motion](brownian-motion.md#cylindrical-brownian-motion)
- [Dirichlet probability generating function](probability-theory.md#dirichlet-probability-generating-function)
- [Discrete Gaussian white noise](time-series.md#discrete-gaussian-white-noise)
- [Discrete random variable](#discrete-random-variable)
- [Entropy submodularity](information-theory.md#entropy-submodularity)
- [Epsilon-sufficient set](information-theory.md#epsilon-sufficient-set)
- [Equality case for conditional second moments](measure-theory.md#equality-case-for-conditional-second-moments)
- [Exchangeable random variables](probability-theory.md#exchangeable-random-variables)
- [Factorial-moment criterion for Poisson convergence](markov-process.md#factorial-moment-criterion-for-poisson-convergence)
- [Factorial-moment inversion](markov-process.md#factorial-moment-inversion)
- [Financial asset](mathematical-finance.md#financial-asset)
- [Gaussian scale mixture](statistical-modelling.md#gaussian-scale-mixture)
- [Infinite divisibility (probability)](probability-theory.md#infinite-divisibility-probability)
- [Integrability](measure-theory.md#integrability)
- [Integrable random variable](probability-theory.md#integrable-random-variable)
- [Jensen's inequality](real-analysis.md#jensen-s-inequality)
- [Joint probability distribution](probability-theory.md#joint-probability-distribution)
- [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable)
- [Lindeberg-Feller central limit theorem](convergence-of-random-variables.md#lindeberg-feller-central-limit-theorem)
- [Littlewood interpolation inequality](functional-analysis.md#littlewood-interpolation-inequality)
- [Lyapunov condition](convergence-of-random-variables.md#lyapunov-condition)
- [Lyapunov moment inequality](probability-inequality.md#lyapunov-moment-inequality)
- [Mean residual life](survival-analysis.md#mean-residual-life)
- [Mean-square integral](measure-theory.md#mean-square-integral)
- [Method of moments (probability theory)](convergence-of-random-variables.md#method-of-moments-probability-theory)
- [Minimal martingale measure in a one-period market](mathematical-finance.md#minimal-martingale-measure-in-a-one-period-market)
- [Monotonicity of normalized subset entropies](probability-and-statistics.md#monotonicity-of-normalized-subset-entropies)
- [Multiplicative entropy power inequality](information-theory.md#multiplicative-entropy-power-inequality)
- [One-sided maximal inequality for a centered square-integrable martingale](martingale.md#one-sided-maximal-inequality-for-a-centered-square-integrable-martingale)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#10f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#3f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#9f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#25j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#25j/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#12g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#10f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#4f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#4f/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#29i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2.md#10f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2.md#12f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2.md#9f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-30.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#22j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33.md#5/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#11f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#12f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#12f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#12f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2.md#10f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2.md#4f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2.md#9f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#11g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#27j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#3g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#26k/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#27h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-320.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#26k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#26g/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-2.md#11f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-2.md#4f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-210.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-210.md#1/d/solution)
- [Pedigree graphical model](biology.md#pedigree-graphical-model)
- [Poisson characterization by independent binomial splitting](probability-theory.md#poisson-characterization-by-independent-binomial-splitting)
- [Popoviciu's inequality on variances](variance.md#popoviciu-s-inequality-on-variances)
- [Portfolio diversification](mathematical-finance.md#portfolio-diversification)
- [Probability generating function](probability-theory.md#probability-generating-function)
- [Probability mass function](probability-theory.md#probability-mass-function)
- [Pseudo-covariance](variance.md#pseudo-covariance)
- [Random element](#random-element)
- [Random field](stochastic-process.md#random-field)
- [Random matrix](probability-theory.md#random-matrix)
- [Random measure](measure-theory.md#random-measure)
- [Random sum](#random-sum)
- [Random vector](#random-vector)
- [Recycling a uniform random variable after discrete sampling](probability-theory.md#recycling-a-uniform-random-variable-after-discrete-sampling)
- [Regular conditional distribution](probability-theory.md#regular-conditional-distribution)
- [Reparameterization gradient](statistical-inference.md#reparameterization-gradient)
- [Second moment](probability-theory.md#second-moment)
- [Shape parameter](statistical-modelling.md#shape-parameter)
- [Statistical dependence](#statistical-dependence)
- [Sub-Gamma random variable in the right tail](probability-inequality.md#sub-gamma-random-variable-in-the-right-tail)
- [Sub-Poisson random variable in the right tail](probability-inequality.md#sub-poisson-random-variable-in-the-right-tail)
- [Symmetrization as conditional expectation](measure-theory.md#symmetrization-as-conditional-expectation)
- [Tail integral formula for expectation](probability-theory.md#tail-integral-formula-for-expectation)
- [Tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments)
- [Tail measurability of limits of sample averages](probability-theory.md#tail-measurability-of-limits-of-sample-averages)
- [Tail probability](probability-theory.md#tail-probability)
- [Tail-sum formula for expectation](probability-theory.md#tail-sum-formula-for-expectation)
- [Terminal wealth floor](utility-function.md#terminal-wealth-floor)
- [Truncated first moment bound](probability-and-statistics.md#truncated-first-moment-bound)
- [Wigner matrix](probability-theory.md#wigner-matrix)
- [Zero-probability event](probability-theory.md#zero-probability-event)
