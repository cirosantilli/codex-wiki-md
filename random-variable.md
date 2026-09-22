# Random variable

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_variable)

A real-valued random variable is a [measurable function](measure-theory.md#measurable-function) $X$ from a [probability space](probability-theory.md#probability-space) $(\Omega,\mathcal F,\mathbb P)$ to the [real numbers](arithmetic.md#real-number) with their [Borel sigma-algebra](measure-theory.md#borel-sigma-algebra). More general targets give [random elements](#random-element). For every [Borel set](measure-theory.md#borel-set) $A$, measurability ensures that $\{\omega:X(\omega)\in A\}$ is an [event](probability-theory.md#event), so the question "does the observed value lie in $A$?" has a defined [probability](probability-theory.md#probability).

The [function](function.md) $X$ is fixed; its input outcome is uncertain. This separates what we measure from how the uncertainty is modeled. A [probability distribution](probability-theory.md#probability-distribution) is the resulting [pushforward measure](measure-theory.md#pushforward-measure), $\mathbb P_X(A)=\mathbb P(X\in A)$. A [cumulative distribution function](probability-theory.md#cumulative-distribution-function), [probability mass function](probability-theory.md#probability-mass-function), or [probability density function](continuous-probability-distribution.md#probability-density-function) describes that [measure](measure-theory.md#measure) in an appropriate setting. The random variable and its [probability distribution](probability-theory.md#probability-distribution) are different objects: the former also retains its relationship to other measurements on the same [sample space](probability-theory.md#sample-space).

For two independent uniform dice, let $U,V$ record their results and define $S=U+V$ and $M=\max(U,V)$. The 36 ordered pairs are equally likely, but the resulting [probability mass functions](probability-theory.md#probability-mass-function) differ:

$$
\mathbb P(S=s)=\frac{6-|s-7|}{36}\quad(2\leq s\leq12),\qquad
\mathbb P(M=m)=\frac{2m-1}{36}\quad(1\leq m\leq6).
$$

For the sum, count the diagonal of the outcome grid having total $s$. For the maximum, subtract the $(m-1)^2$ pairs with both results below $m$ from the $m^2$ pairs with both results at most $m$. These examples show how a deterministic [function](function.md) transforms a simple input [probability distribution](probability-theory.md#probability-distribution) into a nonuniform output one.

<a id="image-different-random-variables-on-the-same-equally-likely-dice-outcome-space"></a>
![](random-variable-dice-distributions.png)

**[Figure 1](#image-different-random-variables-on-the-same-equally-likely-dice-outcome-space). Different random variables on the same equally likely dice outcome space**.

The corresponding [expected values](probability-theory.md#expected-value) are $\mathbb E S=7$ and $\mathbb E M=161/36$. The first follows immediately from [linearity of expectation](probability-theory.md#linearity-of-expectation); the second follows from $\sum_{m=1}^6m(2m-1)/36$. Neither number must be an attainable result. An [expected value](probability-theory.md#expected-value) describes an average under the [probability measure](probability-theory.md#probability-measure), not a prediction that the next observation will equal it.

The distinction between a random variable and its [probability distribution](probability-theory.md#probability-distribution) matters for dependence. $U$ and $V$ have the same [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution) and are [independent random variables](#independent-random-variables). $U$ and a second copy of $U$ also have that same marginal [probability distribution](probability-theory.md#probability-distribution), but they always agree. Their joint [probability distribution](probability-theory.md#probability-distribution) is concentrated on the diagonal; the marginals alone cannot say which relationship holds. This is why a model for several measurements must specify their joint law or an appropriate [independence](#independent-random-variables) assumption.

[Indicator random variables](probability-theory.md#indicator-random-variable) turn [events](probability-theory.md#event) into numbers: $\mathbf1_A$ equals one on $A$ and zero elsewhere, and $\mathbb E\mathbf1_A=\mathbb P(A)$. This connects event counting with [expected value](probability-theory.md#expected-value) and [variance](variance.md), and lets tools for [random variables](random-variable.md) answer questions about [probabilities](probability-theory.md#probability). More complicated [functions](function.md) of observations can describe totals, waiting times, or estimation errors using the same framework.

**Table of contents**

- [Random element](#random-element)
- [Statistical dependence](#statistical-dependence)
- [Random sum](#random-sum)
  - [Transform composition for an independent random sum](#transform-composition-for-an-independent-random-sum)
- [Discrete random variable](#discrete-random-variable)
- [Random vector](#random-vector)
  - [Joint probability mass function](#joint-probability-mass-function)
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
    - [Pairwise independence does not imply joint independence](#pairwise-independence-does-not-imply-joint-independence)
  - [Conditional independence](#conditional-independence)
    - [Conditioning can destroy independence](#conditioning-can-destroy-independence)
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

A [random variable](random-variable.md) is discrete when some finite or [countable set](set-theory.md#countable-set) $D\subseteq\mathbb R$ has $\mathbb P(X\in D)=1$. Its [probability mass function](probability-theory.md#probability-mass-function) is $p_X(x)=\mathbb P(X=x)$; these nonnegative masses sum to one. An [event](probability-theory.md#event) determined by the value has [probability](probability-theory.md#probability) $\mathbb P(X\in A)=\sum_{x\in A\cap D}p_X(x)$. Values outside $D$ may still occur on a [zero-probability event](probability-theory.md#zero-probability-event) without changing this definition.

Countable support need not consist of [integers](number-theory.md#integer): a random variable constantly equal to $3/2$ is discrete. Integer-indexed [tail-sum formulas](probability-theory.md#tail-sum-formula) therefore require a separate integer-valued hypothesis. For the dice sum in [random variable](random-variable.md), the [expected value](probability-theory.md#expected-value) is $\sum_{s=2}^{12}s\,p_S(s)=7$ and the [variance](variance.md) is $\sum_{s=2}^{12}(s-7)^2p_S(s)=35/6$; the same answer follows by adding the [variances](variance.md) of its [independent](#independent-random-variables) summands.

## Random vector

↑ **Parent:** [Random variable](random-variable.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_vector)

A random vector is a [random variable](random-variable.md) whose values are vectors or, equivalently, an ordered tuple of scalar random variables on one probability space.

### Joint probability mass function

↑ **Parent:** [Random vector](#random-vector)

For [discrete random variables](#discrete-random-variable) $X,Y$, their joint probability mass function assigns a [probability](probability-theory.md#probability) to each possible ordered pair. Its entries are nonnegative and sum to one. [Marginalization](probability-theory.md#marginalization) gives the [probability mass functions](probability-theory.md#probability-mass-function) $p_X(x)=\sum_y p_{X,Y}(x,y)$ and $p_Y(y)=\sum_x p_{X,Y}(x,y)$. In a table with rows indexed by $x$ and columns by $y$, these are the row and column totals. The [joint probability distribution](probability-theory.md#joint-probability-distribution) records how the coordinates occur together, while the [marginal distributions](probability-theory.md#marginal-distribution) describe each separately.

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

[Random variables](random-variable.md) $X_1,\ldots,X_n$ are independent when, for every choice of [Borel sets](measure-theory.md#borel-set) $A_1,\ldots,A_n$,

$$
\mathbb P\!\left(\bigcap_{i=1}^n\{X_i\in A_i\}\right)
=\prod_{i=1}^n\mathbb P(X_i\in A_i).
$$

The requirement covers all these [events](probability-theory.md#event), not only one selected combination of values. Equivalently, the generated [sigma-algebras](measure-theory.md#sigma-algebra) are [independent sigma-algebras](probability-theory.md#independent-sigma-algebras), or the [joint probability distribution](probability-theory.md#joint-probability-distribution) is the [product measure](probability-theory.md#product-measure) of the [marginal distributions](probability-theory.md#marginal-distribution). For an infinite family, the same condition must hold for every finite subfamily. For [random elements](#random-element), replace [Borel sets](measure-theory.md#borel-set) by [measurable sets](measure-theory.md#measurable-set) in their specified target spaces.

For [discrete random variables](#discrete-random-variable), checking every entry of the [joint probability mass function](#joint-probability-mass-function) is enough:

$$
p_{X_1,\ldots,X_n}(x_1,\ldots,x_n)=\prod_{i=1}^n p_{X_i}(x_i).
$$

Summing this identity over the desired sets proves the event formulation. For general real-valued [random variables](random-variable.md), checking point [probabilities](probability-theory.md#probability) alone can say nothing: a pair with no point masses has $\mathbb P(X=x,Y=y)=\mathbb P(X=x)\mathbb P(Y=y)=0$ even when $Y=X$. The all-set definition avoids that trap. See [Gautam Iyer, Conditional Probability and Independence, definitions 12, 16 and 18 and proposition 19](https://www.math.cmu.edu/~gautam/c/2026-425/notes/independence.html), with the continuous case treated in his [Continuous Random Variables notes](https://www.math.cmu.edu/~gautam/c/2026-425/notes/cts-rvs.html).

For a concrete comparison, let $X,Y$ be [independent](#independent-random-variables) fair [bits](information-theory.md#bit): each has a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with parameter $1/2$. Their [joint probability mass function](#joint-probability-mass-function), with rows $X=0,1$ and columns $Y=0,1$, is

$$
J_{\mathrm{ind}}=\begin{pmatrix}1/4&1/4\\1/4&1/4\end{pmatrix}.
$$

All four entries equal the product of the corresponding row and column totals, $(1/2)(1/2)$. For example, $\mathbb P(Y=1\mid X=0)=1/2$: learning one [bit](information-theory.md#bit) leaves the other one's [probability distribution](probability-theory.md#probability-distribution) unchanged.

Now keep a fair $X$ but set $Y=X$. The same [marginal distributions](probability-theory.md#marginal-distribution) give the same product table, yet the actual [joint probability mass function](#joint-probability-mass-function) is

$$
J_{\mathrm{same}}=\begin{pmatrix}1/2&0\\0&1/2\end{pmatrix}.
$$

Here $\mathbb P(X=0,Y=1)=0$ differs from $(1/2)(1/2)=1/4$, and $\mathbb P(Y=1\mid X=1)=1$. Thus matching [marginal distributions](probability-theory.md#marginal-distribution) does not establish [independence](#independent-random-variables). Grinstead and Snell formulate the discrete product criterion in [Introduction to Probability, section 4.1, definition 4.4, printed page 143](https://chance.dartmouth.edu/teaching_aids/books_articles/probability_book/Chapter4.pdf).

<a id="image-independence-compares-every-joint-probability-with-the-product-of-the-marginals"></a>
![](independent-and-dependent-probability-tables.png)

**[Figure 2](#image-independence-compares-every-joint-probability-with-the-product-of-the-marginals). Independence compares every joint probability with the product of the marginals**. Each row compares an actual [joint probability mass function](#joint-probability-mass-function) with its product of [marginal distributions](probability-theory.md#marginal-distribution). Marginal totals are shown at the right and bottom of every table; each whole table sums to one. The last example has zero [covariance](variance.md#covariance) but a visibly different joint table.

[Independence](#independent-random-variables) is stronger than zero [covariance](variance.md#covariance). For [square-integrable](measure-theory.md#square-integrable-function) [independent random variables](#independent-random-variables), $\mathbb E[XY]=\mathbb E[X]\mathbb E[Y]$, so they are [uncorrelated random variables](variance.md#uncorrelated-random-variables). The converse fails: take $X$ with a [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution) on $\{-1,0,1\}$ and $Y=X^2$. Direct calculation gives

$$
\mathbb E[X]=0,\qquad \mathbb E[Y]=2/3,\qquad
\mathbb E[XY]=\mathbb E[X^3]=0,\qquad
\operatorname{Cov}(X,Y)=0.
$$

Nevertheless, $Y$ is a nonconstant [function](function.md) determined by $X$. The [event](probability-theory.md#event) $X=0$ is exactly the [event](probability-theory.md#event) $Y=0$, so $\mathbb P(X=0,Y=0)=1/3$, whereas $\mathbb P(X=0)\mathbb P(Y=0)=1/9$. The positive and negative contributions to the [covariance](variance.md#covariance) cancel without erasing the [statistical dependence](#statistical-dependence).

The usefulness of [independence](#independent-random-variables) is that a large [joint probability distribution](probability-theory.md#joint-probability-distribution) can be assembled from small pieces. For $n$ fair [independent](#independent-random-variables) [bits](information-theory.md#bit), each of the $2^n$ patterns has [probability](probability-theory.md#probability) $2^{-n}$. Products also simplify [expected values](probability-theory.md#expected-value), and vanishing cross [covariances](variance.md#covariance) simplify the [variance of a sum](variance.md#variance-of-a-sum). Separate [measurable functions](measure-theory.md#measurable-function) of [independent random variables](#independent-random-variables) remain [independent](#independent-random-variables): each output [event](probability-theory.md#event) is already an input [event](probability-theory.md#event), so the defining product rule still applies. These are consequences of a model's [independence](#independent-random-variables) assumption; whether the assumption describes actual observations is a question for [statistical inference](statistical-inference.md).

### Pairwise independent random variables

↑ **Parent:** [Independent random variables](#independent-random-variables)

[Random variables](random-variable.md) are pairwise independent when every two distinct members are [independent random variables](#independent-random-variables). Each pair's [joint probability distribution](probability-theory.md#joint-probability-distribution) must factor for all its [events](probability-theory.md#event); examining only a pair's [covariance](variance.md#covariance) is insufficient. Full [independence](#independent-random-variables) implies pairwise independence by taking the other sets in the definition to be the whole target spaces. The reverse implication fails once there are three or more variables.

Pairwise independence is enough to add [variances](variance.md): for a finite family of [square-integrable](measure-theory.md#square-integrable-function) pairwise independent [random variables](random-variable.md),

$$
\operatorname{Var}\!\left(\sum_{i=1}^n X_i\right)=\sum_{i=1}^n\operatorname{Var}(X_i),
$$

because all cross [covariances](variance.md#covariance) vanish in the [variance of a sum](variance.md#variance-of-a-sum). Thus pairwise independence can support calculations about the size of fluctuations while failing to determine the full [joint probability distribution](probability-theory.md#joint-probability-distribution). The following example makes that distinction visible.

#### Pairwise independence does not imply joint independence

↑ **Parent:** [Pairwise independent random variables](#pairwise-independent-random-variables)

Let $X,Y$ be [independent](#independent-random-variables) fair [bits](information-theory.md#bit), and let $Z=X\mathbin\oplus Y$ be their [exclusive or](computer-science.md#exclusive-or): $Z=1$ precisely when $X\ne Y$. The four possible triples are $000,011,101,110$, each with [probability](probability-theory.md#probability) $1/4$. Each coordinate is a fair [bit](information-theory.md#bit). Writing out all eight patterns gives

$$
\begin{array}{c|cccccccc}
(x,y,z)&000&001&010&011&100&101&110&111\\\hline
p_{X,Y,Z}(x,y,z)&1/4&0&0&1/4&0&1/4&1/4&0\\
p_X(x)p_Y(y)p_Z(z)&1/8&1/8&1/8&1/8&1/8&1/8&1/8&1/8
\end{array}
$$

Every pair has all four cells $00,01,10,11$ with [probability](probability-theory.md#probability) $1/4$:

$$
J_{X,Y}=J_{X,Z}=J_{Y,Z}
=\begin{pmatrix}1/4&1/4\\1/4&1/4\end{pmatrix}.
$$

For $(X,Z)$, the four allowed triples project to $00,01,11,10$; for $(Y,Z)$ they project to $00,11,01,10$. Each projection lists each pair exactly once, proving pairwise independence. But $\mathbb P(X=0,Y=0,Z=0)=1/4$ differs from the product $1/8$, so the three are not [independent random variables](#independent-random-variables). Indeed, any two determine the third. A single coordinate reveals nothing about another, while two coordinates together reveal it completely.

<a id="image-the-xor-example-hides-joint-dependence-from-every-pairwise-probability-table"></a>
![](pairwise-versus-joint-independence.png)

**[Figure 3](#image-the-xor-example-hides-joint-dependence-from-every-pairwise-probability-table). The XOR example hides joint dependence from every pairwise probability table**. The bars show all eight triple patterns against the $1/8$ reference for three [independent](#independent-random-variables) fair [bits](information-theory.md#bit). Below, all three pairwise [joint probability mass functions](#joint-probability-mass-function) have four equal cells of $1/4$.

The [exclusive or](computer-science.md#exclusive-or) example is the complementary-bit version of the two-toss exercise in [Grinstead and Snell, Introduction to Probability, section 4.1, exercise 7, printed page 151](https://chance.dartmouth.edu/teaching_aids/books_articles/probability_book/Chapter4.pdf). It is a compact reason to check the full product rule whenever a calculation uses three-way or higher [events](probability-theory.md#event).

### Conditional independence

↑ **Parent:** [Independent random variables](#independent-random-variables)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_independence)

[Random variables](random-variable.md) $X$ and $Y$ are conditionally independent given $Z$ when, for every pair of [Borel sets](measure-theory.md#borel-set) $A,B$, the following identity holds [almost surely](convergence-of-random-variables.md#almost-sure-convergence):

$$
\mathbb P(X\in A,Y\in B\mid Z)
=\mathbb P(X\in A\mid Z)\mathbb P(Y\in B\mid Z).
$$

Here [conditional probabilities](probability-theory.md#conditional-probability) are [conditional expectations](measure-theory.md#conditional-expectation) of the corresponding [indicator random variables](probability-theory.md#indicator-random-variable) given the [sigma-algebra](measure-theory.md#sigma-algebra) generated by $Z$. This defines the condition even when $\mathbb P(Z=z)=0$. In terms of [regular conditional distributions](probability-theory.md#regular-conditional-distribution), the conditional joint law is the product of the conditional [marginal distributions](probability-theory.md#marginal-distribution) for almost every conditioning value.

For [discrete random variables](#discrete-random-variable), at every $z$ with $\mathbb P(Z=z)>0$, the condition becomes

$$
p_{X,Y\mid Z=z}(x,y)=p_{X\mid Z=z}(x)p_{Y\mid Z=z}(y).
$$

Where $\mathbb P(X=x,Z=z)>0$, this is equivalent to $\mathbb P(Y=y\mid X=x,Z=z)=\mathbb P(Y=y\mid Z=z)$. Once $Z$ is known, observing $X$ provides no further information about $Y$. See [Cosma Shalizi, Information Theory I, section Conditional independence and conditional mutual information](https://www.stat.cmu.edu/~cshalizi/dm/20/lectures/09/lecture-09.html) for this predictive interpretation.

For a worked example, suppose a [latent variable](statistical-modelling.md#latent-variable) $T$ chooses between two environments with $\mathbb P(T=0)=\mathbb P(T=1)=1/2$. Given $T=t$, take $X,Y$ to be [independent and identically distributed](#independent-and-identically-distributed-random-variables) with a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) of parameter $p_t$, where $p_0=0.1$ and $p_1=0.9$. Think of two separate trials run under the same quiet or active environment. Their conditional [joint probability mass functions](#joint-probability-mass-function), with rows $X=0,1$ and columns $Y=0,1$, are

$$
J_0=\begin{pmatrix}0.81&0.09\\0.09&0.01\end{pmatrix},\qquad
J_1=\begin{pmatrix}0.01&0.09\\0.09&0.81\end{pmatrix}.
$$

Each is exactly the product of its own conditional [marginal distributions](probability-theory.md#marginal-distribution): $(0.9,0.1)$ for $T=0$, and $(0.1,0.9)$ for $T=1$. Thus $X,Y$ are [conditionally independent](#conditional-independence) given $T$.

If the environment is unobserved, the [law of total probability](probability-theory.md#law-of-total-probability) averages the two tables:

$$
J=\tfrac12J_0+\tfrac12J_1
=\begin{pmatrix}0.41&0.09\\0.09&0.41\end{pmatrix}.
$$

Both unconditional [marginal distributions](probability-theory.md#marginal-distribution) are fair, but $0.41\ne0.5\times0.5$. The [law of total expectation](measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[X]=\mathbb E[Y]=0.5,\qquad
\mathbb E[XY]=\tfrac12(0.1^2+0.9^2)=0.41,\qquad
\operatorname{Cov}(X,Y)=0.41-0.25=0.16.
$$

Observing $X=1$ makes the active environment more plausible, so it raises $\mathbb P(Y=1\mid X=1)$ to $0.41/0.5=0.82$. Knowing the actual environment removes this source of [statistical dependence](#statistical-dependence). The [covariance induced by a shared latent variable](#covariance-induced-by-a-shared-latent-variable) lemma explains the calculation without listing all the outcomes.

This is why [conditional independence](#conditional-independence) is useful in [statistical modelling](statistical-modelling.md): a model can multiply simple conditional laws and then average over a shared [latent variable](statistical-modelling.md#latent-variable). The resulting observations can remain statistically dependent. [Conditional independence graphs](#conditional-independence-graph) organize such information relations; their interpretation as causes requires additional assumptions from [causal inference](causal-inference.md). Conditioning describes the information available to an observer. It does not, by itself, describe what would happen if an experimenter changed a variable.

#### Conditioning can destroy independence

↑ **Parent:** [Conditional independence](#conditional-independence)

Return to [pairwise independence does not imply joint independence](#pairwise-independence-does-not-imply-joint-independence), where $X,Y$ are [independent](#independent-random-variables) fair [bits](information-theory.md#bit) and $Z=X\mathbin\oplus Y$ is their [exclusive or](computer-science.md#exclusive-or). Given $Z=0$, only $000$ and $110$ remain, each with conditional [probability](probability-theory.md#probability) $1/2$. Given $Z=1$, only $011$ and $101$ remain, again each with conditional [probability](probability-theory.md#probability) $1/2$. Consequently,

$$
J_{X,Y\mid Z=0}=\begin{pmatrix}1/2&0\\0&1/2\end{pmatrix},\qquad
J_{X,Y\mid Z=1}=\begin{pmatrix}0&1/2\\1/2&0\end{pmatrix}.
$$

The conditional [marginal distributions](probability-theory.md#marginal-distribution) are still fair, so their product has four entries $1/4$ in either case. The actual tables differ: $Y=X$ given $Z=0$, and $Y=1-X$ given $Z=1$. Thus unconditional [independence](#independent-random-variables) need not survive conditioning. Observing whether two [bits](information-theory.md#bit) agree restricts their possible combinations; no physical interaction between the original trials is required to produce that information constraint.

#### Covariance induced by a shared latent variable

↑ **Parent:** [Conditional independence](#conditional-independence)

Let $A,B$ be [indicator random variables](probability-theory.md#indicator-random-variable) with [conditional independence](#conditional-independence) given a [latent variable](statistical-modelling.md#latent-variable) $T$, and suppose $\mathbb E[A\mid T]=\mathbb E[B\mid T]=g(T)$. Then

$$
\operatorname{Cov}(A,B)=\operatorname{Var}(g(T))\geq0.
$$

For a short proof, [conditional independence](#conditional-independence) gives $\mathbb E[AB\mid T]=g(T)^2$. The [law of total expectation](measure-theory.md#law-of-total-expectation) gives $\mathbb E[AB]=\mathbb E[g(T)^2]$ and $\mathbb E[A]=\mathbb E[B]=\mathbb E[g(T)]$. Subtract their product to obtain the claimed [variance](variance.md). Since $0\leq g(T)\leq1$, all the required [expected values](probability-theory.md#expected-value) exist.

In the two-environment example of [conditional independence](#conditional-independence), $g(T)$ is $0.1$ or $0.9$ with equal [probabilities](probability-theory.md#probability). Hence $\mathbb E[g(T)]=0.5$ and $\operatorname{Var}(g(T))=((0.1-0.5)^2+(0.9-0.5)^2)/2=0.16$. The two trials have zero [conditional covariance](variance.md#conditional-covariance) in either environment, yet their unconditional [covariance](variance.md#covariance) is positive because their success [probabilities](probability-theory.md#probability) rise and fall together.

More generally, [square-integrable](measure-theory.md#square-integrable-function) [conditionally independent](#conditional-independence) [random variables](random-variable.md) satisfy

$$
\operatorname{Cov}(A,B)
=\operatorname{Cov}\bigl(\mathbb E[A\mid T],\mathbb E[B\mid T]\bigr)
$$

by the [law of total covariance](variance.md#law-of-total-covariance). Equal conditional means reduce this to the displayed [variance](variance.md); unequal conditional means need not give a nonnegative [covariance](variance.md#covariance). The equal-mean result explains correlated component evolutionary states in a [coeval binary population](stellar-astrophysics.md#coeval-binary-population) without correlation between initial masses: variation in a shared environment can supply the entire [covariance](variance.md#covariance).

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

## ← Incoming links (288)

- [Absolute moment](probability-theory.md#absolute-moment)
- [Bayesian network](statistical-model.md#bayesian-network)
- [Benford law](discrete-probability-distribution.md#benford-law)
- [Benford law from logarithmic uniformity](discrete-probability-distribution.md#benford-law-from-logarithmic-uniformity)
- [Bernoulli coupling by a shared uniform random variable](probability-and-statistics.md#bernoulli-coupling-by-a-shared-uniform-random-variable)
- [Bernstein moment condition](probability-and-statistics.md#bernstein-moment-condition)
- [Beta distribution](probability-theory.md#beta-distribution)
- [Birthday probability for hash outputs](computer-science.md#birthday-probability-for-hash-outputs)
- [Boundedness in probability](convergence-of-random-variables.md#boundedness-in-probability)
- [Canonical pseudometric of a Gaussian process](stochastic-process.md#canonical-pseudometric-of-a-gaussian-process)
- [Cantelli inequality](probability-inequality.md#cantelli-inequality)
- [Cauchy random variable](probability-theory.md#cauchy-random-variable)
- [Characteristic function](probability-theory.md#characteristic-function)
- [Chebyshev's inequality](probability-inequality.md#chebyshev-s-inequality)
- [Chordal graph](graph-theory.md#chordal-graph)
- [Complement rule of probability](probability-theory.md#complement-rule-of-probability)
- [Complex covariance](variance.md#complex-covariance)
- [Composition of absolutely summable time-series filters](time-series.md#composition-of-absolutely-summable-time-series-filters)
- [Concentration inequality](probability-inequality.md#concentration-inequality)
- [Conditional characteristic function](probability-theory.md#conditional-characteristic-function)
- [Conditional expectation](measure-theory.md#conditional-expectation)
- [Conditional expectation preserving a distribution](measure-theory.md#conditional-expectation-preserving-a-distribution)
- [Conditional independence](#conditional-independence)
- [Conditional Jensen inequality](measure-theory.md#conditional-jensen-inequality)
- [Conditional probability](probability-theory.md#conditional-probability)
- [Conditional variance](variance.md#conditional-variance)
- [Contingent claim payoff](mathematical-finance.md#contingent-claim-payoff)
- [Continuity of probability](probability-theory.md#continuity-of-probability)
- [Control variates](probability-and-statistics.md#control-variates)
- [Coupling](probability-and-statistics.md#coupling)
- [Coupling characterization of total variation distance](probability-and-statistics.md#coupling-characterization-of-total-variation-distance)
- [Coupling inequality for total variation](probability-and-statistics.md#coupling-inequality-for-total-variation)
- [Covariance](variance.md#covariance)
- [Covariance criterion for diversification of factor residuals](mathematical-finance.md#covariance-criterion-for-diversification-of-factor-residuals)
- [Covariance induced by a shared latent variable](#covariance-induced-by-a-shared-latent-variable)
- [Cumulative distribution function](probability-theory.md#cumulative-distribution-function)
- [Cylindrical Brownian motion](brownian-motion.md#cylindrical-brownian-motion)
- [Differential entropy](information-theory.md#differential-entropy)
- [Dirichlet probability generating function](probability-theory.md#dirichlet-probability-generating-function)
- [Discrete Gaussian white noise](time-series.md#discrete-gaussian-white-noise)
- [Discrete probability distribution](discrete-probability-distribution.md)
- [Discrete random variable](#discrete-random-variable)
- [Discrete-time Markov chain](markov-process.md#discrete-time-markov-chain)
- [Disjoint observation windows](probability-theory.md#disjoint-observation-windows)
- [Entropy submodularity](information-theory.md#entropy-submodularity)
- [Epsilon-sufficient set](information-theory.md#epsilon-sufficient-set)
- [Equality case for conditional second moments](measure-theory.md#equality-case-for-conditional-second-moments)
- [Equality in Markov's inequality](probability-inequality.md#equality-in-markov-s-inequality)
- [Exchangeable random variables](probability-theory.md#exchangeable-random-variables)
- [Expectation value](quantum-mechanics.md#expectation-value)
- [Expected value](probability-theory.md#expected-value)
- [Expected value premium principle](actuarial-statistics.md#expected-value-premium-principle)
- [Exponential Markov bound](probability-inequality.md#exponential-markov-bound)
- [Extreme value theory](probability-theory.md#extreme-value-theory)
- [Factorial-moment criterion for Poisson convergence](markov-process.md#factorial-moment-criterion-for-poisson-convergence)
- [Factorial-moment inversion](markov-process.md#factorial-moment-inversion)
- [Financial asset](mathematical-finance.md#financial-asset)
- [First moment method](probability-inequality.md#first-moment-method)
- [Gaussian random variable](probability-theory.md#gaussian-random-variable)
- [Gaussian scale mixture](statistical-modelling.md#gaussian-scale-mixture)
- [Gumbel distribution](probability-theory.md#gumbel-distribution)
- [Hoeffding inequality](probability-inequality.md#hoeffding-inequality)
- [Hoeffding lemma](probability-inequality.md#hoeffding-lemma)
- [Independent increments](stochastic-process.md#independent-increments)
- [Independent random variables](#independent-random-variables)
- [Indicator random variable](probability-theory.md#indicator-random-variable)
- [Infinite divisibility (probability)](probability-theory.md#infinite-divisibility-probability)
- [Integrability](measure-theory.md#integrability)
- [Integrable random variable](probability-theory.md#integrable-random-variable)
- [Jensen's inequality](real-analysis.md#jensen-s-inequality)
- [Joint entropy](information-theory.md#joint-entropy)
- [Joint probability distribution](probability-theory.md#joint-probability-distribution)
- [Kolmogorov extension theorem](stochastic-process.md#kolmogorov-extension-theorem)
- [Kullback-Leibler divergence](probability-and-statistics.md#kullback-leibler-divergence)
- [Kurtosis](probability-theory.md#kurtosis)
- [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable)
- [Law of the unconscious statistician](probability-theory.md#law-of-the-unconscious-statistician)
- [Law of total variance](probability-theory.md#law-of-total-variance)
- [Lebesgue integral](measure-theory.md#lebesgue-integral)
- [Limsup of events](probability-theory.md#limsup-of-events)
- [Lindeberg-Feller central limit theorem](convergence-of-random-variables.md#lindeberg-feller-central-limit-theorem)
- [Linearity of expectation](probability-theory.md#linearity-of-expectation)
- [Littlewood interpolation inequality](functional-analysis.md#littlewood-interpolation-inequality)
- [Lyapunov condition](convergence-of-random-variables.md#lyapunov-condition)
- [Lyapunov moment inequality](probability-inequality.md#lyapunov-moment-inequality)
- [Markov's inequality](probability-inequality.md#markov-s-inequality)
- [Maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator)
- [Mean residual life](survival-analysis.md#mean-residual-life)
- [Mean-square integral](measure-theory.md#mean-square-integral)
- [Method of moments (probability theory)](convergence-of-random-variables.md#method-of-moments-probability-theory)
- [Minimal martingale measure in a one-period market](mathematical-finance.md#minimal-martingale-measure-in-a-one-period-market)
- [Moment matching for a beta prior](probability-theory.md#moment-matching-for-a-beta-prior)
- [Monotonicity of normalized subset entropies](probability-and-statistics.md#monotonicity-of-normalized-subset-entropies)
- [Multiplicative entropy power inequality](information-theory.md#multiplicative-entropy-power-inequality)
- [Negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution)
- [Nondecreasing function](calculus.md#nondecreasing-function)
- [Normal distribution](probability-theory.md#normal-distribution)
- [One-sided maximal inequality for a centered square-integrable martingale](martingale.md#one-sided-maximal-inequality-for-a-centered-square-integrable-martingale)
- [Order statistic](probability-theory.md#order-statistic)
- [Overlap in the union bound](probability-inequality.md#overlap-in-the-union-bound)
- [Pairwise independent random variables](#pairwise-independent-random-variables)
- [Parity construction of pairwise independent bits](probability-theory.md#parity-construction-of-pairwise-independent-bits)
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
- [Pearson correlation coefficient](variance.md#pearson-correlation-coefficient)
- [Pedigree graphical model](biology.md#pedigree-graphical-model)
- [Point process](probability-theory.md#point-process)
- [Poisson characterization by independent binomial splitting](probability-theory.md#poisson-characterization-by-independent-binomial-splitting)
- [Popoviciu's inequality on variances](variance.md#popoviciu-s-inequality-on-variances)
- [Portfolio diversification](mathematical-finance.md#portfolio-diversification)
- [Probability density function](continuous-probability-distribution.md#probability-density-function)
- [Probability distribution](probability-theory.md#probability-distribution)
- [Probability generating function](probability-theory.md#probability-generating-function)
- [Probability inequality](probability-inequality.md)
- [Probability mass function](probability-theory.md#probability-mass-function)
- [Probability space](probability-theory.md#probability-space)
- [Probability theory](probability-theory.md)
- [Pseudo-covariance](variance.md#pseudo-covariance)
- [Q-Q plot](probability-and-statistics.md#q-q-plot)
- [Random element](#random-element)
- [Random field](stochastic-process.md#random-field)
- [Random matrix](probability-theory.md#random-matrix)
- [Random measure](measure-theory.md#random-measure)
- [Random sum](#random-sum)
- [Random variable](random-variable.md)
- [Random vector](#random-vector)
- [Recycling a uniform random variable after discrete sampling](probability-theory.md#recycling-a-uniform-random-variable-after-discrete-sampling)
- [Regular conditional distribution](probability-theory.md#regular-conditional-distribution)
- [Reparameterization gradient](statistical-inference.md#reparameterization-gradient)
- [Sample path](stochastic-process.md#sample-path)
- [Scope and scale of total correlation](information-theory.md#scope-and-scale-of-total-correlation)
- [Scoring rule](statistical-inference.md#scoring-rule)
- [Second moment](probability-theory.md#second-moment)
- [Second-moment bound for positivity](probability-inequality.md#second-moment-bound-for-positivity)
- [Second moment method](probability-inequality.md#second-moment-method)
- [Separate chaining](computer-science.md#separate-chaining)
- [Shape parameter](statistical-modelling.md#shape-parameter)
- [Shared random rate gives dependent point counts](probability-theory.md#shared-random-rate-gives-dependent-point-counts)
- [Shared-uniform counterexample to the second Borel-Cantelli lemma](probability-theory.md#shared-uniform-counterexample-to-the-second-borel-cantelli-lemma)
- [Simple random walk on the integer line](markov-process.md#simple-random-walk-on-the-integer-line)
- [Standard score](probability-theory.md#standard-score)
- [Statistical dependence](#statistical-dependence)
- [Stochastic process](stochastic-process.md)
- [Sub-Gamma random variable in the right tail](probability-inequality.md#sub-gamma-random-variable-in-the-right-tail)
- [Sub-Poisson random variable in the right tail](probability-inequality.md#sub-poisson-random-variable-in-the-right-tail)
- [Symmetrization as conditional expectation](measure-theory.md#symmetrization-as-conditional-expectation)
- [Tail integral formula for expectation](probability-theory.md#tail-integral-formula-for-expectation)
- [Tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments)
- [Tail measurability of limits of sample averages](probability-theory.md#tail-measurability-of-limits-of-sample-averages)
- [Tail probability](probability-theory.md#tail-probability)
- [Tail-sum formula for expectation](probability-theory.md#tail-sum-formula-for-expectation)
- [Terminal wealth floor](utility-function.md#terminal-wealth-floor)
- [Total correlation](information-theory.md#total-correlation)
- [Total variation distance and hypothesis testing](probability-and-statistics.md#total-variation-distance-and-hypothesis-testing)
- [Truncated first moment bound](probability-and-statistics.md#truncated-first-moment-bound)
- [Uncorrelated random variables](variance.md#uncorrelated-random-variables)
- [Variance](variance.md)
- [Wigner matrix](probability-theory.md#wigner-matrix)
- [Window count of a point process](probability-theory.md#window-count-of-a-point-process)
- [Zero-probability event](probability-theory.md#zero-probability-event)
