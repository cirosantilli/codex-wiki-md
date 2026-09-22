# Variance

↑ **Parent:** [Expected value](expected-value.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variance)

The [variance](variance.md) measures the mean squared distance of a [random variable](random-variable.md) from its [expected value](expected-value.md). For a real [square-integrable](measure-theory.md#square-integrable-function) [random variable](random-variable.md) $X$,

$$
\operatorname{var}(X)=\mathbb E[(X-\mathbb EX)^2]
=\mathbb E[X^2]-(\mathbb EX)^2.
$$

The square prevents positive and negative deviations from cancelling. It also gives the [variance](variance.md) squared units: if $X$ measures a [length](physics.md#length) in metres, its [variance](variance.md) has units of square metres. Its nonnegative square root is the [standard deviation](#standard-deviation), which has the same units as $X$.

For example, let $X$ take $-1$, $0$ and $1$ with equal [probabilities](probability-theory.md#probability). Its [expected value](expected-value.md) is zero, but its [variance](variance.md) is $[(-1)^2+0^2+1^2]/3=2/3$, and its [standard deviation](#standard-deviation) is $\sqrt{2/3}$. The constant [random variable](random-variable.md) zero has the same [expected value](expected-value.md) and zero [variance](variance.md): a [mean](expected-value.md) alone does not describe the spread. The [variance](variance.md) is zero exactly when $X=\mathbb E X$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence).

The [variance](variance.md) is useful because squared deviations interact neatly with [linear combinations](vector-space.md#linear-combination). The [covariance](#covariance) supplies the cross terms when combining different [random variables](random-variable.md), and a [covariance matrix](#covariance-matrix) organizes those terms for many variables. The characterization of [variance as the minimum mean squared error of a constant](#variance-as-the-minimum-mean-squared-error-of-a-constant) also explains why the [expected value](expected-value.md) is the best constant prediction under squared error.

**Table of contents**

- [Population variance](#population-variance)
- [Fano factor](#fano-factor)
- [Coefficient of variation](#coefficient-of-variation)
- [Variance as the minimum mean squared error of a constant](#variance-as-the-minimum-mean-squared-error-of-a-constant)
- [Conditional variance](#conditional-variance)
  - [Average conditional variance decreases with more information](#average-conditional-variance-decreases-with-more-information)
- [Variance additivity for independent random variables](#variance-additivity-for-independent-random-variables)
  - [L2 convergence of averages of independent variables with bounded second moments](#l2-convergence-of-averages-of-independent-variables-with-bounded-second-moments)
- [Variance of a sum](#variance-of-a-sum)
- [Dependent uniform sampling variance lower bound](#dependent-uniform-sampling-variance-lower-bound)
- [Standard deviation](#standard-deviation)
- [Covariance](#covariance)
  - [Law of total covariance](#law-of-total-covariance)
  - [Strict positive covariance with an increasing payoff](#strict-positive-covariance-with-an-increasing-payoff)
  - [Conditional covariance](#conditional-covariance)
  - [Sample correlation coefficient](#sample-correlation-coefficient)
    - [Sample correlation matrix](#sample-correlation-matrix)
  - [Complex covariance](#complex-covariance)
    - [Pseudo-covariance](#pseudo-covariance)
  - [Linearity of covariance](#linearity-of-covariance)
  - [Uncorrelated random variables](#uncorrelated-random-variables)
    - [Bernoulli independence from zero covariance](#bernoulli-independence-from-zero-covariance)
  - [Covariance matrix](#covariance-matrix)
    - [Covariance ellipse](#covariance-ellipse)
    - [Correlation matrix](#correlation-matrix)
    - [Equicorrelation covariance matrix](#equicorrelation-covariance-matrix)
    - [Mahalanobis distance](#mahalanobis-distance)
    - [Compound-symmetry covariance](#compound-symmetry-covariance)
    - [Rank-one covariance spike](#rank-one-covariance-spike)
    - [Sample mean and covariance](#sample-mean-and-covariance)
      - [Uncentered empirical second-moment matrix](#uncentered-empirical-second-moment-matrix)
      - [Sample mean](#sample-mean)
      - [Sample covariance matrix](#sample-covariance-matrix)
        - [Rank of a centered sample covariance matrix](#rank-of-a-centered-sample-covariance-matrix)
        - [Sample covariance](#sample-covariance)
        - [Effective rank of a covariance matrix](#effective-rank-of-a-covariance-matrix)
          - [Gaussian sample-covariance operator-norm bound](#gaussian-sample-covariance-operator-norm-bound)
    - [Precision matrix](#precision-matrix)
      - [Gaussian conditional variance from precision](#gaussian-conditional-variance-from-precision)
      - [Conditional regression coefficients from a Gaussian precision matrix](#conditional-regression-coefficients-from-a-gaussian-precision-matrix)
      - [Profile likelihood for a Gaussian precision matrix](#profile-likelihood-for-a-gaussian-precision-matrix)
      - [Gaussian sampling from a precision Cholesky factor](#gaussian-sampling-from-a-precision-cholesky-factor)
      - [CLIME precision-matrix estimator](#clime-precision-matrix-estimator)
      - [Graphical Lasso](#graphical-lasso)
        - [Graphical Lasso column regression](#graphical-lasso-column-regression)
        - [Graphical-Lasso Karush-Kuhn-Tucker conditions](#graphical-lasso-karush-kuhn-tucker-conditions)
    - [Pearson correlation coefficient](#pearson-correlation-coefficient)
      - [Conditional correlation](#conditional-correlation)
      - [Partial correlation](#partial-correlation)
      - [Perfect positive correlation](#perfect-positive-correlation)
        - [Terminal proportionality identifies bounded stock volatility](#terminal-proportionality-identifies-bounded-stock-volatility)
        - [Terminal correlation does not identify adapted stock volatility](#terminal-correlation-does-not-identify-adapted-stock-volatility)
      - [Serial correlation](#serial-correlation)
      - [Intraclass correlation coefficient](#intraclass-correlation-coefficient)
- [Popoviciu's inequality on variances](#popoviciu-s-inequality-on-variances)

## Population variance

↑ **Parent:** [Variance](variance.md)

For a finite population $x_1,\ldots,x_n$ with [arithmetic mean](arithmetic.md#arithmetic-mean) $\bar x$, its variance is $\frac1n\sum_{i=1}^n(x_i-\bar x)^2$. It averages squared deviations over the whole population.

## Fano factor

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fano_factor)

For a nonnegative count with positive mean, the Fano factor compares its [variance](variance.md) to its mean. A [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) has factor one. Correlated production bursts or weak restoring feedback can give factors larger than one even at large molecular copy number.

// Target: mathematical-biology.bigb

## Coefficient of variation

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coefficient_of_variation)

For a random variable with nonzero mean, the coefficient of variation is the dimensionless ratio

$$
\operatorname{CV}(X)=\frac{\sqrt{\operatorname{Var}(X)}}{|\mathbb E X|}.
$$

## Variance as the minimum mean squared error of a constant

↑ **Parent:** [Variance](variance.md)

For a square-integrable real random variable $X$,

$$
\mathbb E[(X-a)^2]
=\operatorname{Var}(X)+(\mathbb EX-a)^2.
$$

Thus the unique best constant predictor is $a=\mathbb EX$, and the minimum mean squared error is $\operatorname{Var}(X)$.

## Conditional variance

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_variance)

The conditional variance measures the remaining squared uncertainty after specified information has been used to form a [conditional mean](measure-theory.md#conditional-expectation). For a real [square-integrable](measure-theory.md#square-integrable-function) [random variable](random-variable.md) $X$ and a sub-[sigma-algebra](measure-theory.md#sigma-algebra) $\mathcal G$, let $m=\mathbb E[X\mid\mathcal G]$. Then

$$
\operatorname{Var}(X\mid\mathcal G)
=\mathbb E[(X-m)^2\mid\mathcal G]
=\mathbb E[X^2\mid\mathcal G]-m^2.
$$

It is a $\mathcal G$-measurable [random variable](random-variable.md), nonnegative [almost surely](convergence-of-random-variables.md#almost-sure-convergence), rather than necessarily a single number. With the information $\mathcal G=\sigma(Y)$, its value is the [variance](variance.md) in the group identified by $Y$. Its [expected value](expected-value.md) is the [mean squared error](statistical-modelling.md#mean-squared-error) of predicting $X$ by its [conditional mean](measure-theory.md#conditional-expectation).[Theorem 4.1.15, p. 213](mathematics-bibliography.md#probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation)

In the exact [mixture distribution](probability-distribution.md#mixture-distribution) in [law of total expectation](measure-theory.md#law-of-total-expectation), group $A$ contains $0,4$ around mean two, and group $B$ contains $6,10$ around mean eight. Both groups have [conditional variance](#conditional-variance) four because their deviations from their own means are $-2,2$ with equal probabilities. Therefore $\mathbb E[\operatorname{Var}(X\mid Y)]=4$. Meanwhile, the two group means have [variance](variance.md) $\frac14(2-13/2)^2+\frac34(8-13/2)^2=27/4$. The [law of total variance](probability-theory.md#law-of-total-variance) gives

$$
\boxed{\operatorname{Var}(X)=4+\frac{27}{4}=\frac{43}{4}.}
$$

Direct calculation gives $\mathbb E[X^2]=53$ and $\operatorname{Var}(X)=53-(13/2)^2=43/4$, checking the decomposition.

<a id="image-total-variance-separates-remaining-within-group-error-from-variation-of-group-means"></a>
![](conditional-variance-within-between-groups.png)

**[Figure 1](#image-total-variance-separates-remaining-within-group-error-from-variation-of-group-means). Total variance separates remaining within-group error from variation of group means**. Left: in the stipulated finite [mixture distribution](probability-distribution.md#mixture-distribution), each group's values deviate by $\pm2$ from its [conditional mean](measure-theory.md#conditional-expectation). Right: the total [variance](variance.md) $43/4$ separates into expected [conditional variance](#conditional-variance) four and [variance](variance.md) of the [conditional mean](measure-theory.md#conditional-expectation) $27/4$. Knowing the group removes the latter part from the average squared prediction error. Values and weights are exact model choices, not measured data.

For any square-integrable $\mathcal G$-measurable predictor $Z$, the error identity is

$$
\mathbb E[(X-Z)^2]=\mathbb E[\operatorname{Var}(X\mid\mathcal G)]+\mathbb E[(m-Z)^2].
$$

The cross term vanishes because $\mathbb E[X-m\mid\mathcal G]=0$. Thus using the [conditional mean](measure-theory.md#conditional-expectation) minimizes [mean squared error](statistical-modelling.md#mean-squared-error), while [conditional variance](#conditional-variance) quantifies what this information still cannot predict. This is the [orthogonal projection](hilbert-space.md#orthogonal-projection) interpretation in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space).[4.1 Conditional Expectation](mathematics-bibliography.md#probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation)

### Average conditional variance decreases with more information

↑ **Parent:** [Conditional variance](#conditional-variance)

For [square-integrable](measure-theory.md#square-integrable-function) $X$ and nested information $\mathcal H\subseteq\mathcal G$, let $m_{\mathcal H}=\mathbb E[X\mid\mathcal H]$ and $m_{\mathcal G}=\mathbb E[X\mid\mathcal G]$. The predictor $m_{\mathcal H}$ is also $\mathcal G$-measurable, so the [conditional variance](#conditional-variance) error identity gives

$$
\mathbb E[\operatorname{Var}(X\mid\mathcal H)]-\mathbb E[\operatorname{Var}(X\mid\mathcal G)]=\mathbb E[(m_{\mathcal G}-m_{\mathcal H})^2]\geq0.
$$

More information cannot increase the average best squared prediction error. Equality holds exactly when the two [conditional means](measure-theory.md#conditional-expectation) agree [almost surely](convergence-of-random-variables.md#almost-sure-convergence); additional information can change the [conditional distribution](probability-theory.md#conditional-distribution) without changing its mean.

This is an averaged statement. Take $X=-4,0,4$ with equal probabilities, and learn only whether $X$ is zero. The unconditional [variance](variance.md) is $32/3$. In the nonzero group, the [conditional variance](#conditional-variance) is $16$, which is larger; in the zero group it is zero. Their weighted average remains $(2/3)16+(1/3)0=32/3$. Both groups have [conditional mean](measure-theory.md#conditional-expectation) zero, so the extra information has not improved squared-error prediction, even though it has revealed whether the outcome is extreme or central. An individual group's [conditional variance](#conditional-variance) need not decrease.

## Variance additivity for independent random variables

↑ **Parent:** [Variance](variance.md)

For independent square-integrable random variables,

$$
\operatorname{Var}\left(\sum_iX_i\right)
=\sum_i\operatorname{Var}(X_i).
$$

### L2 convergence of averages of independent variables with bounded second moments

↑ **Parent:** [Variance additivity for independent random variables](#variance-additivity-for-independent-random-variables)

For independent random variables with $\sup_n\mathbb E|X_n|^2<\infty$, write

$$
Y_N=\frac1N\sum_{k=1}^NX_k,
\qquad
m_N=\frac1N\sum_{k=1}^N\mathbb EX_k.
$$

Then $\lVert Y_N-m_N\rVert_2^2=N^{-2}\sum_{k\leq N}\operatorname{Var}(X_k)=O(N^{-1})$. Hence $Y_N$ converges in $L^2$ exactly when the scalar [Cesàro means](sequence-and-series.md#cesaro-mean) $m_N$ converge.

## Variance of a sum

↑ **Parent:** [Variance](variance.md)

For square-integrable random variables,

$$
\operatorname{Var}\left(\sum_iX_i\right)
=\sum_i\sum_j\operatorname{Cov}(X_i,X_j).
$$

## Dependent uniform sampling variance lower bound

↑ **Parent:** [Variance](variance.md)

Let $Z_1,\ldots,Z_n$ each be uniform on $[0,1]$, with arbitrary dependence. For centered unit-norm $f\in L^2[0,1]$, put

$$
D(f)=\operatorname{Var}\left(\frac1n\sum_{i=1}^nf(Z_i)\right).
$$

Then

$$
\sup_fD(f)\ge\frac1n.
$$

Partition $[0,1]$ into $k$ equal intervals and test normalized differences of two interval indicators. Averaging over the two intervals reduces the claim to $\sum_pN_p^2\ge\sum_pN_p=n$ for their occupancy counts, and then let $k\to\infty$.

## Standard deviation

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_deviation)

The standard deviation is the nonnegative square root $\sigma_X=\sqrt{\operatorname{Var}(X)}$ of the [variance](variance.md).

## Covariance

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covariance)

The [covariance](#covariance) measures the average product of two centered deviations. For real [square-integrable](measure-theory.md#square-integrable-function) [random variables](random-variable.md) $X$ and $Y$,

$$
\operatorname{Cov}(X,Y)
=\mathbb E[(X-\mathbb EX)(Y-\mathbb EY)]
=\mathbb E[XY]-\mathbb E X\,\mathbb E Y.
$$

Deviations with the same sign contribute positively; deviations with opposite signs contribute negatively. Their magnitudes and [probabilities](probability-theory.md#probability) determine the net result. Taking $Y=X$ recovers the [variance](variance.md). The definitions and algebraic properties are presented in [Orloff and Bloom, MIT 18.05, Covariance and Correlation, sections 2–2.1](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class07-prep-b.pdf).

For a worked example, let $X,Z$ be [independent random variables](random-variable.md#independent-random-variables), each equally likely to be $-1$, $0$ or $1$, and put $Y=2X+Z$. All nine pairs $(X,Z)$ have [probability](probability-theory.md#probability) $1/9$. The [expected values](expected-value.md) are zero, while [linearity of covariance](#linearity-of-covariance) and the vanishing [covariance](#covariance) of [independent random variables](random-variable.md#independent-random-variables) give

$$
\operatorname{Var}(X)=\operatorname{Var}(Z)=\frac23,\qquad
\operatorname{Cov}(X,Y)=2\operatorname{Var}(X)=\frac43,\qquad
\operatorname{Var}(Y)=4\operatorname{Var}(X)+\operatorname{Var}(Z)=\frac{10}{3}.
$$

The shared $X$ term makes large $X$ accompany large $Y$ on average. Replacing $2X$ by $-2X$ reverses the [covariance](#covariance) to $-4/3$ without changing either [variance](variance.md).

<a id="image-positive-negative-independent-and-nonlinear-relationships-have-different-covariance-behavior"></a>
![](covariance-and-dependence.png)

**[Figure 2](#image-positive-negative-independent-and-nonlinear-relationships-have-different-covariance-behavior). Positive, negative, independent, and nonlinear relationships have different covariance behavior**. In the first three panels, $X$ and $Z$ independently take $-1$, $0$ and $1$ with equal [probabilities](probability-theory.md#probability); each point has [probability](probability-theory.md#probability) $1/9$. In the last panel, $Y=X^2$, and the three marked outcomes each have [probability](probability-theory.md#probability) $1/3$. The thin curve shows that [quadratic function](polynomial.md#quadratic-function). Its zero [covariance](#covariance) leaves strong nonlinear [statistical dependence](random-variable.md#statistical-dependence) visible.

The [covariance](#covariance) is useful whenever deviations are added or subtracted. Expanding the square gives

$$
\operatorname{Var}(X+Y)
=\operatorname{Var}(X)+\operatorname{Var}(Y)+2\operatorname{Cov}(X,Y),\qquad
\operatorname{Var}(X-Y)
=\operatorname{Var}(X)+\operatorname{Var}(Y)-2\operatorname{Cov}(X,Y).
$$

For the worked model, these are $20/3$ and $4/3$. Positive [covariance](#covariance) increases variation in the sum while reducing variation in the difference: the same shared fluctuation reinforces one combination and partly cancels in the other. The identity applies beyond [independent random variables](random-variable.md#independent-random-variables).

The size of a [covariance](#covariance) depends on the measurement scale. For constants $a,b,c,d$, [linearity of covariance](#linearity-of-covariance) gives $\operatorname{Cov}(aX+b,cY+d)=ac\operatorname{Cov}(X,Y)$. Adding offsets has no effect; rescaling either measurement rescales the [covariance](#covariance). The [Pearson correlation coefficient](#pearson-correlation-coefficient) divides by both [standard deviations](#standard-deviation) to describe the standardized linear relationship.

### Law of total covariance

↑ **Parent:** [Covariance](#covariance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_total_covariance)

For square-integrable random variables, expand $X$ and $Y$ into their [conditional expectations](measure-theory.md#conditional-expectation) and their centered conditional residuals. The cross terms vanish by the [law of total expectation](measure-theory.md#law-of-total-expectation), giving the displayed [covariance](#covariance) decomposition. Conditional independence can therefore coexist with positive unconditional covariance from a shared [latent variable](latent-variable.md).

### Strict positive covariance with an increasing payoff

↑ **Parent:** [Covariance](#covariance)

If $Z$ is nondegenerate, $g$ is strictly increasing and the relevant products are [integrable](measure-theory.md#integrability), an independent copy $Z'$ gives $2\operatorname{Cov}(g(Z),Z)=\mathbb E[(g(Z)-g(Z'))(Z-Z')]$. The integrand is positive exactly when $Z\ne Z'$, so the [covariance](#covariance) is strictly positive. The same argument applies within each conditional law and yields a positive terminal [stock](mathematical-finance.md#stock) hedge for an attainable increasing payoff.

### Conditional covariance

↑ **Parent:** [Covariance](#covariance)

For square-integrable random variables, $\operatorname{Cov}(X,Z\mid\mathcal G)=\mathbb E[XZ\mid\mathcal G]-\mathbb E[X\mid\mathcal G]\mathbb E[Z\mid\mathcal G]$. It is a $\mathcal G$-measurable random variable. Replacing $X$ by its [conditional expectation](measure-theory.md#conditional-expectation) given a larger sigma-field leaves this [covariance](#covariance) unchanged when $Z$ is measurable with respect to that larger sigma-field. This observation underlies [recovery of a martingale-transform integrand by conditional covariance](martingale.md#recovery-of-a-martingale-transform-integrand-by-conditional-covariance).

### Sample correlation coefficient

↑ **Parent:** [Covariance](#covariance)

For paired observations $(x_i,y_i)$, the [sample correlation coefficient](#sample-correlation-coefficient) is

$$
r_{XY}=\frac{\sum_i(x_i-\overline x)(y_i-\overline y)}
{\sqrt{\sum_i(x_i-\overline x)^2\sum_i(y_i-\overline y)^2}}.
$$

It is the normalized [inner product](inner-product.md) of the centered data [vectors](vector-space.md#vector), or the [sample covariance](#sample-covariance) divided by the product of the corresponding sample [standard deviations](#standard-deviation). The choice of divisor $n$ or $n-1$ cancels when used consistently in all three quantities. It is undefined if either centered data [vector](vector-space.md#vector) is zero, which occurs when that variable is constant in the observed [statistical sample](statistical-inference.md#statistical-sample).

For $x=(1,2,3,4)$ and $y=(2,1,4,3)$, both [sample means](#sample-mean) are $2.5$. The sum of centered products is $3$, and each sum of centered squares is $5$, hence **the sample correlation coefficient is $3/5=0.6$**. This is a summary of these four observed pairs; it is not automatically the population [Pearson correlation coefficient](#pearson-correlation-coefficient). [Philip Stark, Computing the correlation coefficient](https://www.stat.berkeley.edu/~stark/SticiGui/Text/computeR.htm) explains the centered and standardized calculation.

#### Sample correlation matrix

↑ **Parent:** [Sample correlation coefficient](#sample-correlation-coefficient)

A [sample correlation matrix](#sample-correlation-matrix) rescales a [sample covariance matrix](#sample-covariance-matrix) $S$ to unit diagonal, for variables with positive sample variance. Its off-diagonal entries are [sample correlation coefficients](#sample-correlation-coefficient). Strong correlations between predictors can indicate [multicollinearity](normal-linear-model.md#multicollinearity), but pairwise correlations alone do not exclude higher-order linear dependence.

### Complex covariance

↑ **Parent:** [Covariance](#covariance)

For square-integrable complex [random variables](random-variable.md), the Hermitian covariance is $\operatorname{Cov}_{\mathbb C}(Z,W)=\mathbb E[(Z-\mathbb EZ)\overline{(W-\mathbb EW)}]$. Its diagonal is nonnegative and equals $\mathbb E|Z-\mathbb EZ|^2$. The conjugation distinguishes it from the [pseudo-covariance](#pseudo-covariance).

#### Pseudo-covariance

↑ **Parent:** [Complex covariance](#complex-covariance)

For a centered complex [random variable](random-variable.md) $Z=A+iB$, the pseudo-covariance is $P=\mathbb EZ^2$. Together with $V=\mathbb E|Z|^2$ it determines the real [covariance matrix](#covariance-matrix): $\mathbb EA^2=(V+\operatorname{Re}P)/2$, $\mathbb EB^2=(V-\operatorname{Re}P)/2$, and $\mathbb EAB=\operatorname{Im}P/2$.

### Linearity of covariance

↑ **Parent:** [Covariance](#covariance)

Covariance is bilinear: for constants $a_i,b_j$ and square-integrable random variables,

$$
\operatorname{Cov}\!\left(\sum_i a_iX_i,\sum_jb_jY_j\right)
=\sum_{i,j}a_ib_j\operatorname{Cov}(X_i,Y_j).
$$

### Uncorrelated random variables

↑ **Parent:** [Covariance](#covariance)

Two [square-integrable](measure-theory.md#square-integrable-function) [random variables](random-variable.md) $X,Y$ are [uncorrelated random variables](#uncorrelated-random-variables) when $\operatorname{Cov}(X,Y)=0$. [Independent random variables](random-variable.md#independent-random-variables) with finite [second moments](expected-value.md#second-moment) are [uncorrelated random variables](#uncorrelated-random-variables), but zero [covariance](#covariance) does not generally imply [independence](random-variable.md#independent-random-variables).

For an explicit counterexample, let $X$ take $-1$, $0$, $1$ with equal [probabilities](probability-theory.md#probability), and let $Y=X^2$. Then $\mathbb E X=\mathbb E X^3=0$, so $\operatorname{Cov}(X,Y)=\mathbb E X^3-\mathbb E X\,\mathbb E X^2=0$. Nevertheless, $Y$ is completely determined by $X$: $\mathbb P(Y=0\mid X=0)=1$, while $\mathbb P(Y=0)=1/3$. Thus these are [uncorrelated random variables](#uncorrelated-random-variables) with [statistical dependence](random-variable.md#statistical-dependence). In this example, opposite contributions from the [odd function](calculus.md#odd-function) $x^3$ cancel; the [even function](calculus.md#even-function) $x^2$ still retains information about $|X|$. The last panel of the [covariance](#covariance) diagram shows the relationship.

There are useful special cases. [Uncorrelated jointly normal variables are independent](probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent), and the [Bernoulli independence from zero covariance](#bernoulli-independence-from-zero-covariance) result supplies another setting where the converse holds. Their distribution assumptions do the extra work; zero [covariance](#covariance) alone does not.

#### Bernoulli independence from zero covariance

↑ **Parent:** [Uncorrelated random variables](#uncorrelated-random-variables)

For two [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) with joint probabilities $a,b,c,d$ in the order $(0,0),(0,1),(1,0),(1,1)$, their [covariance](#covariance) is $d-(c+d)(b+d)=ad-bc$. Zero covariance fixes the $(1,1)$ probability to the product of its marginals; subtracting this from each marginal fixes all three remaining joint probabilities to their products. Thus [uncorrelated random variables](#uncorrelated-random-variables) taking only zero and one are independent, including degenerate marginals. The implication is special to this two-point setting and fails for general distributions.

### Covariance matrix

↑ **Parent:** [Covariance](#covariance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covariance_matrix)

For a real [random vector](random-variable.md#random-vector) $X=(X_1,\ldots,X_p)^T$ with finite [second moments](expected-value.md#second-moment), its [covariance matrix](#covariance-matrix) collects all pairwise [covariances](#covariance):

$$
\Sigma=\mathbb E[(X-\mathbb EX)(X-\mathbb EX)^T],\qquad
\Sigma_{ij}=\operatorname{Cov}(X_i,X_j).
$$

The diagonal entries are [variances](variance.md). The [covariance matrix](#covariance-matrix) is a [symmetric matrix](linear-algebra.md#symmetric-matrix) and a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix), because for every real [vector](vector-space.md#vector) $a$,

$$
a^T\Sigma a=\operatorname{Var}(a^TX)\geq0.
$$

Thus one [matrix](vector-space.md#matrix) describes the [variance](variance.md) of every [linear combination](vector-space.md#linear-combination) of the coordinates. It is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) exactly when no nonzero [linear combination](vector-space.md#linear-combination) is constant [almost surely](convergence-of-random-variables.md#almost-sure-convergence). A deterministic linear relation produces a zero [eigenvalue](linear-operator-theory.md#eigenvalue).

For example,

$$
\Sigma=\begin{pmatrix}1&0.8\\0.8&1\end{pmatrix}
$$

has unit coordinate [variances](variance.md), [covariance](#covariance) $0.8$, and [eigenvalues](linear-operator-theory.md#eigenvalue) $1.8$ and $0.2$. Its unit [eigenvectors](linear-operator-theory.md#eigenvector) $(1,1)^T/\sqrt2$ and $(1,-1)^T/\sqrt2$ describe directions of greatest and least projected [variance](variance.md). For a unit [vector](vector-space.md#vector) $a=(\cos\theta,\sin\theta)^T$, direct multiplication gives $a^T\Sigma a=1+0.8\sin(2\theta)$: the variation in the sum direction is nine times that in the difference direction.

<a id="image-a-covariance-matrix-encodes-projected-variance-in-every-direction"></a>
![](covariance-projection-geometry.png)

**[Figure 3](#image-a-covariance-matrix-encodes-projected-variance-in-every-direction). A covariance matrix encodes projected variance in every direction**. Left: the [covariance ellipse](#covariance-ellipse) has a [semi-major axis](celestial-mechanics.md#semi-major-axis) of [length](physics.md#length) $\sqrt{1.8}$ and a [semi-minor axis](celestial-mechanics.md#semi-minor-axis) of [length](physics.md#length) $\sqrt{0.2}$ along the [eigenvectors](linear-operator-theory.md#eigenvector) of $\Sigma$. Right: the [variance](variance.md) of the unit-direction projection is $1+0.8\sin(2\theta)$. This is exact [matrix](vector-space.md#matrix) geometry for the stipulated [covariance matrix](#covariance-matrix), with no sampled observations or claimed probability coverage.

The [spectral theorem](hilbert-space.md#spectral-theorem) supplies an [orthonormal basis](inner-product.md#orthonormal-basis) of these directions. This connects [covariance matrices](#covariance-matrix) to [principal component analysis](statistical-learning.md#principal-component-analysis): its leading [eigenvector](linear-operator-theory.md#eigenvector) identifies the unit-direction projection with the largest [variance](variance.md). For a [linear transformation](vector-space.md#linear-map) $A$, the transformed [random vector](random-variable.md#random-vector) has [covariance matrix](#covariance-matrix) $A\Sigma A^T$, so uncertainties propagate through a linear model by [matrix multiplication](vector-space.md#matrix-multiplication).

#### Covariance ellipse

↑ **Parent:** [Covariance matrix](#covariance-matrix)

For a two-dimensional [positive-definite](bilinear-form.md#positive-definite-bilinear-form) [covariance matrix](#covariance-matrix) $\Sigma$, the centered [covariance ellipse](#covariance-ellipse) is the image of the [unit circle](complex-analysis.md#complex-unit-circle) under its positive definite [square root of a matrix](quadratic-form.md#square-root-of-a-matrix). Equivalently, it satisfies $x^T\Sigma^{-1}x=1$. Its [semi-major and semi-minor axes](euclidean-geometry.md#semi-major-and-semi-minor-axes) have [lengths](physics.md#length) given by the square roots of the larger and smaller [eigenvalues](linear-operator-theory.md#eigenvalue), along the corresponding [eigenvectors](linear-operator-theory.md#eigenvector). The [ellipse](euclidean-geometry.md#ellipse) encodes a second-moment geometry; a probability-coverage interpretation needs additional information about the [probability distribution](probability-distribution.md) and the chosen scale.

#### Correlation matrix

↑ **Parent:** [Covariance matrix](#covariance-matrix)

For a random vector with [covariance](#covariance) $\Sigma$ and positive coordinate [variances](variance.md), let $D=\operatorname{diag}(\Sigma)$. Its [correlation matrix](#correlation-matrix) is the [covariance](#covariance) of $D^{-1/2}(X-\mathbb EX)$, so it is positive semidefinite with unit diagonal. Each entry is the [correlation](#pearson-correlation-coefficient) of the corresponding pair of variables. In particular $\operatorname{tr}(C)=p$, explaining why an [eigenvalue](linear-operator-theory.md#eigenvalue) in correlation-based [principal component analysis](statistical-learning.md#principal-component-analysis) represents that [eigenvalue](linear-operator-theory.md#eigenvalue) divided by $p$ of the total [variance](variance.md). The empirical version is the [sample correlation matrix](#sample-correlation-matrix).

#### Equicorrelation covariance matrix

↑ **Parent:** [Covariance matrix](#covariance-matrix)

This unit-variance [covariance matrix](#covariance-matrix) has [eigenvalue](linear-operator-theory.md#eigenvalue) $1+(p-1)r$ on the constant-vector direction and [eigenvalue](linear-operator-theory.md#eigenvalue) $1-r$ on its orthogonal complement. It is positive semidefinite exactly when $-1/(p-1)\le r\le1$. For positive $r$, the first [population principal component](statistical-learning.md#population-principal-component) is the normalized sum of the centered variables.

#### Mahalanobis distance

↑ **Parent:** [Covariance matrix](#covariance-matrix)

For a [positive-definite](bilinear-form.md#positive-definite-bilinear-form) [covariance matrix](#covariance-matrix), this is [Euclidean distance](topological-analysis.md#euclidean-distance) after whitening. It accounts for both scales and correlations and is invariant under consistent nonsingular linear changes of coordinates. Estimating the covariance can be unstable with small samples, and a singular covariance requires restricting to a nonsingular subspace rather than claiming an ordinary [metric](topological-analysis.md#metric) on the full space.

#### Compound-symmetry covariance

↑ **Parent:** [Covariance matrix](#covariance-matrix)

A [compound-symmetry covariance](#compound-symmetry-covariance) matrix has a common diagonal entry and a common off-diagonal entry: $\Sigma=aI+cJ$. For a group of size $k$, its within-group [eigenvalue](linear-operator-theory.md#eigenvalue) is $a$ and its constant-direction [eigenvalue](linear-operator-theory.md#eigenvalue) is $a+kc$. Thus $a\geq0$ and $a+kc\geq0$ characterize [positive semidefiniteness](quadratic-form.md#positive-semidefinite-matrix). When $c\geq0$, an independent shared [random intercept](generalized-linear-model.md#random-intercept) plus individual noise realizes this covariance. A group mean has [variance](variance.md) $c+a/k$; a difference of two disjoint subgroup means within the same group cancels $c$.

#### Rank-one covariance spike

↑ **Parent:** [Covariance matrix](#covariance-matrix)

For a unit vector $u$ and $\theta>0$, a rank-one covariance spike is the [covariance matrix](#covariance-matrix) $I+\theta uu^\top$. Its [eigenvalue](linear-operator-theory.md#eigenvalue) is $1+\theta$ in the direction $u$ and one on the [orthogonal complement](hilbert-space.md#orthogonal-complement). It arises by adding an independent scalar [normal distribution](probability-distribution.md#normal-distribution) signal $Yu$ to a standard [Gaussian random vector](probability-and-statistics.md#gaussian-random-vector).

#### Sample mean and covariance

↑ **Parent:** [Covariance matrix](#covariance-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sample_mean_and_covariance)

The sample mean and covariance estimate the first two moments of a [random vector](random-variable.md#random-vector) from repeated observations.

##### Uncentered empirical second-moment matrix

↑ **Parent:** [Sample mean and covariance](#sample-mean-and-covariance)

The uncentered empirical second-moment matrix averages the outer products of the observations. Its [expected value](expected-value.md) is $\operatorname{Cov}(X)+\mathbb E[X]\mathbb E[X]^\top$. It is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the [covariance matrix](#covariance-matrix) when the population [expected value](expected-value.md) is known to be zero. It differs from a [sample covariance matrix](#sample-covariance-matrix) centered at the sample mean.

##### Sample mean

↑ **Parent:** [Sample mean and covariance](#sample-mean-and-covariance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sample_mean)

For observations $X_1,\ldots,X_n$, the sample mean is $\overline X=n^{-1}\sum_{i=1}^nX_i$.

##### Sample covariance matrix

↑ **Parent:** [Sample mean and covariance](#sample-mean-and-covariance)

For observations $x_1,\ldots,x_n$, the sample covariance matrix is $n^{-1}\sum_i(x_i-\bar x)(x_i-\bar x)^T$, or the same sum divided by $n-1$ under the unbiased convention.

###### Rank of a centered sample covariance matrix

↑ **Parent:** [Sample covariance matrix](#sample-covariance-matrix)

If $H=I_n-\mathbf1\mathbf1^T/n$ and $S=X^THX/n$, then $\operatorname{rank}S=\operatorname{rank}(HX)\leq\min(p,n-1)$. In particular [full column rank](vector-space.md#full-column-rank) of raw $X$ does not ensure a nonsingular centered [sample covariance matrix](#sample-covariance-matrix). When $S$ is singular, its Gaussian precision [profile likelihood](maximum-likelihood-estimation.md#profile-likelihood) has no finite maximizer: increase precision along a nonzero null vector.

###### Sample covariance

↑ **Parent:** [Sample covariance matrix](#sample-covariance-matrix)

For paired scalar observations $(x_i,y_i)$, their sample covariance is $n^{-1}\sum_i(x_i-\bar x)(y_i-\bar y)$, or the same sum divided by $n-1$ under the unbiased convention. It is an off-diagonal entry of the [sample covariance matrix](#sample-covariance-matrix) of the paired vectors.

###### Effective rank of a covariance matrix

↑ **Parent:** [Sample covariance matrix](#sample-covariance-matrix)

The effective rank measures the total variance of a covariance matrix relative to its largest directional variance.

###### Gaussian sample-covariance operator-norm bound

↑ **Parent:** [Effective rank of a covariance matrix](#effective-rank-of-a-covariance-matrix)

For independent centered Gaussian vectors with covariance $\Sigma$ and uncentered sample covariance $\widehat\Sigma=n^{-1}\sum_ix_ix_i^T$, with probability at least $1-e^{-t}$,

$$
\lVert\widehat\Sigma-\Sigma\rVert_{\mathrm{op}}
\leq C\lVert\Sigma\rVert_{\mathrm{op}}
\left(\sqrt{\frac{r(\Sigma)+t}{n}}+\frac{r(\Sigma)+t}{n}\right).
$$

#### Precision matrix

↑ **Parent:** [Covariance matrix](#covariance-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Precision_matrix)

The precision matrix is the inverse of a nonsingular [covariance matrix](#covariance-matrix). For a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), a zero off-diagonal precision entry encodes conditional independence of the corresponding coordinates given all remaining coordinates.

##### Gaussian conditional variance from precision

↑ **Parent:** [Precision matrix](#precision-matrix)

For a nonsingular [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) with [precision matrix](#precision-matrix) $\Omega$, fixing all coordinates except $X_i$ leaves a density proportional to $\exp[-\Omega_{ii}(x_i-m_i)^2/2]$ after completing the square. Thus its [conditional variance](#conditional-variance) is the reciprocal diagonal precision entry. This is conditioning on every other coordinate, not the marginal [variance](variance.md) $(\Omega^{-1})_{ii}$.

##### Conditional regression coefficients from a Gaussian precision matrix

↑ **Parent:** [Precision matrix](#precision-matrix)

In a [Gaussian graphical model](random-variable.md#gaussian-graphical-model), regressing component $k$ on the others gives the displayed coefficients, residual variance $1/\Omega_{kk}$ and intercept $\mu_k-\mu_{-k}^{\mathsf T}\theta_{-k,k}$. Opposite directions have identical zero patterns and signs because $\Omega$ is symmetric with positive diagonal, but generally unequal coefficient magnitudes.

##### Profile likelihood for a Gaussian precision matrix

↑ **Parent:** [Precision matrix](#precision-matrix)

For independent [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) observations with unknown mean and nonsingular covariance, profiling the mean at its sample value gives negative log-likelihood proportional to $-\log\det\Omega+\operatorname{tr}(S\Omega)$ over $\Omega\succ0$. The [sample covariance matrix](#sample-covariance-matrix) uses divisor $n$. Its minimizer exists exactly when $S\succ0$, and is then $S^{-1}$.

##### Gaussian sampling from a precision Cholesky factor

↑ **Parent:** [Precision matrix](#precision-matrix)

If a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) $Q=LL^T$ is the [precision matrix](#precision-matrix) of a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), draw independent $\xi\sim N(0,I)$ and solve $L^T\eta=\xi$. Then $m+\eta$ has covariance $L^{-T}L^{-1}=Q^{-1}$. This avoids forming the inverse and exploits a banded [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) when $Q$ is banded.

##### CLIME precision-matrix estimator

↑ **Parent:** [Precision matrix](#precision-matrix)

The constrained $\ell^1$ minimization estimator minimizes $\lVert\Omega\rVert_1$ subject to

$$
\lVert\widehat\Sigma\Omega-I\rVert_{\max}\leq\lambda.
$$

Its constraints and objective separate by columns. Feasibility of the true precision matrix and elementary matrix-norm inequalities yield entrywise error bounds under an entrywise covariance-estimation bound.

##### Graphical Lasso

↑ **Parent:** [Precision matrix](#precision-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graphical_Lasso)

The graphical Lasso estimates a sparse [precision matrix](#precision-matrix) by minimizing a Gaussian negative log-likelihood plus an entrywise $\ell^1$ penalty.

###### Graphical Lasso column regression

↑ **Parent:** [Graphical Lasso](#graphical-lasso)

For a [Graphical Lasso](#graphical-lasso) solution with inverse $\widehat\Sigma$, the unique minimizer of $\tfrac12\|Wb-W^{-1}S_{-j,j}\|_2^2+\lambda\|b\|_1$, $W^2=\widehat\Sigma_{-j,-j}\succ0$, is $b=-\widehat\Omega_{-j,j}/\widehat\Omega_{jj}$. The inverse identity gives $\widehat\Sigma_{-j,j}=\widehat\Sigma_{-j,-j}b$, and the off-diagonal [Graphical-Lasso Karush-Kuhn-Tucker conditions](#graphical-lasso-karush-kuhn-tucker-conditions) become the column [Lasso](lasso.md) conditions because the corresponding signs are opposite.

###### Graphical-Lasso Karush-Kuhn-Tucker conditions

↑ **Parent:** [Graphical Lasso](#graphical-lasso)

For objective $-\log\det\Omega+\operatorname{Tr}(S\Omega)+\lambda\lVert\Omega\rVert_{1,\mathrm{entry}}$, the KKT conditions are $-\Omega^{-1}+S+\lambda Z=0$ with $Z_{ij}\in\partial|\Omega_{ij}|$.

#### Pearson correlation coefficient

↑ **Parent:** [Covariance matrix](#covariance-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)

The [Pearson correlation coefficient](#pearson-correlation-coefficient) is the [covariance](#covariance) divided by the product of the [standard deviations](#standard-deviation). For real [random variables](random-variable.md) with finite, strictly positive [variances](variance.md),

$$
\rho_{X,Y}=\frac{\operatorname{Cov}(X,Y)}{\sqrt{\operatorname{Var}(X)\operatorname{Var}(Y)}}.
$$

It is the [expected value](expected-value.md) of the product of the two centered variables after dividing each by its [standard deviation](#standard-deviation). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $-1\leq\rho_{X,Y}\leq1$. This removes measurement units, while retaining the direction and strength of the linear relationship. Constant [random variables](random-variable.md) have zero [standard deviation](#standard-deviation), so their [Pearson correlation coefficient](#pearson-correlation-coefficient) is undefined.

For the [covariance](#covariance) model $Y=2X+Z$, with $X,Z$ independently uniform on $\{-1,0,1\}$, the calculation gives

$$
\rho_{X,Y}=\frac{4/3}{\sqrt{(2/3)(10/3)}}=\frac2{\sqrt5}\approx0.894427.
$$

The positive [correlation](#pearson-correlation-coefficient) is less than one because the independent $Z$ term introduces extra variation. For $Y=-2X+Z$ the [correlation](#pearson-correlation-coefficient) is $-2/\sqrt5$. Both examples appear in the [covariance](#covariance) diagram.

For nonzero real $a,c$, the [correlation](#pearson-correlation-coefficient) of $aX+b$ and $cY+d$ is $\operatorname{sgn}(ac)\rho_{X,Y}$. Positive rescaling and added offsets therefore leave the [correlation](#pearson-correlation-coefficient) unchanged; reversing one scale reverses its sign. Equality $|\rho_{X,Y}|=1$ means that one [random variable](random-variable.md) is an [affine function](vector-space.md#affine-function) of the other [almost surely](convergence-of-random-variables.md#almost-sure-convergence), with a nonzero slope of the corresponding sign. This is the equality condition in the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), and includes [perfect positive correlation](#perfect-positive-correlation).

Zero [correlation](#pearson-correlation-coefficient) says that the centered variables are [orthogonal](inner-product.md#orthogonal-vectors) in their square-integrable [inner product](inner-product.md). It permits nonlinear [statistical dependence](random-variable.md#statistical-dependence), as the example $Y=X^2$ in [uncorrelated random variables](#uncorrelated-random-variables) demonstrates. More generally, a [correlation](#pearson-correlation-coefficient) is a statement about a [joint probability distribution](probability-distribution.md#joint-probability-distribution); identifying effects of interventions is the separate task of [causal inference](causal-inference.md). This distinction keeps an observed association from being mistaken for a demonstrated mechanism.

An early source for standardized association is [Francis Galton](probability-and-statistics.md#francis-galton)'s 1888 paper “Co-relations and their Measurement, chiefly from Anthropometric Data”. He compared stature and forearm measurements and changed each measurement to units of its own variability so the two regression directions could be compared. His scale used [probable error](probability-distribution.md#probable-error), so it should not be identified word for word with the modern [standard deviation](#standard-deviation) formula above. [Galton's original paper, Proceedings of the Royal Society 45, 135–145](https://galton.org/essays/1880-1889/galton-1888-co-relations-royal-soc/galton_corr.html).

##### Conditional correlation

↑ **Parent:** [Pearson correlation coefficient](#pearson-correlation-coefficient)

The [correlation coefficient](#pearson-correlation-coefficient) computed under a [conditional distribution](probability-theory.md#conditional-distribution), using its [conditional covariance](#conditional-covariance) and positive [conditional variances](#conditional-variance). It can depend on the observed conditioning value. For a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), conditioning on other coordinates gives the corresponding [partial correlation](#partial-correlation).

##### Partial correlation

↑ **Parent:** [Pearson correlation coefficient](#pearson-correlation-coefficient)

The partial [correlation](#pearson-correlation-coefficient) is the [correlation](#pearson-correlation-coefficient) of residuals after linearly projecting each of two variables on the conditioning variables and an intercept. With nonsingular [covariance matrix](#covariance-matrix), subtracting the two least-squares predictors gives residual [covariance](#covariance) $\sigma_{12}-\sigma_{13}\sigma_{23}/\sigma_{33}$ and residual [variances](variance.md) $\sigma_{ii}-\sigma_{i3}^2/\sigma_{33}$. Dividing gives the displayed formula. For a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), it is also the [conditional correlation](#conditional-correlation), independent of the conditioning value; this equality need not hold for general distributions.

##### Perfect positive correlation

↑ **Parent:** [Pearson correlation coefficient](#pearson-correlation-coefficient)

For square-integrable variables of positive [variance](variance.md), correlation one is equivalent to $X-\mathbb EX=c(Y-\mathbb EY)$ with $c>0$. The squared norm of the difference between the two standardized centered variables is $2(1-\rho)$, proving the equivalence. For uncentered variables the relationship can have a nonzero intercept; it need not be proportionality.

###### Terminal proportionality identifies bounded stock volatility

↑ **Parent:** [Perfect positive correlation](#perfect-positive-correlation)

For two strictly positive zero-rate stock [martingales](martingale.md) with bounded volatilities and the same initial value, proportional terminal prices must be equal because their [expectations](expected-value.md) coincide. [Conditional expectation](measure-theory.md#conditional-expectation) then makes the whole paths equal. Comparing their stochastic integrals by the [Itô isometry](stochastic-calculus.md#ito-isometry) gives equality of the volatility coefficients almost everywhere in time and probability. [Perfect positive correlation](#perfect-positive-correlation) alone does not provide the required proportionality.

###### Terminal correlation does not identify adapted stock volatility

↑ **Parent:** [Perfect positive correlation](#perfect-positive-correlation)

The stocks $S_t=e^{B_t-t/2}$ and $S'_t=(1+S_t)/2$ start at one, are true square-integrable zero-rate [martingales](martingale.md), and have [perfect positive correlation](#perfect-positive-correlation) at each positive time. Their bounded multiplicative volatilities are $1$ and $S_t/(1+S_t)$, which differ throughout. The additive intercept is what allows the same correlation but different stochastic-exponential coefficients.

##### Serial correlation

↑ **Parent:** [Pearson correlation coefficient](#pearson-correlation-coefficient)

Responses observed on the same process or individual at different times may have nonzero [correlation coefficients](#pearson-correlation-coefficient). Such serial correlation can arise from a shared [random effect](latent-variable.md#random-effect) or from history-dependent conditional means. A scalar [dispersion parameter](exponential-family.md#dispersion-parameter) adjustment alone does not represent this temporal dependence.

##### Intraclass correlation coefficient

↑ **Parent:** [Pearson correlation coefficient](#pearson-correlation-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intraclass_correlation_coefficient)

The intraclass correlation coefficient measures the correlation between observations in the same group. In a random-intercept model with group variance $\sigma_G^2$ and individual variance $\sigma_I^2$, it is $\sigma_G^2/(\sigma_G^2+\sigma_I^2)$.

<h2 id="popoviciu-s-inequality-on-variances">Popoviciu's inequality on variances</h2>

↑ **Parent:** [Variance](variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Popoviciu's_inequality_on_variances)

If a [random variable](random-variable.md) $X$ takes values in $[m,M]$, then

$$
\operatorname{Var}(X)\leq\frac{(M-m)^2}{4}.
$$

## ↑ Ancestors (6)

1. [Expected value](expected-value.md)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (1290)

- [Additional measurements decrease known-error covariance](normal-linear-model.md#additional-measurements-decrease-known-error-covariance)
- [Adjusted coefficient of determination](linear-regression.md#adjusted-coefficient-of-determination)
- [Affine invariance of kurtosis](probability-distribution.md#affine-invariance-of-kurtosis)
- [Amplitude-squared squeezing](quantum-optics.md#amplitude-squared-squeezing)
- [Anderson–Darling test](probability-distribution.md#anderson-darling-test)
- [Antithetic Cauchy-tail integration on a finite interval](monte-carlo-method.md#antithetic-cauchy-tail-integration-on-a-finite-interval)
- [Antithetic variates](monte-carlo-method.md#antithetic-variates)
- [Aperture photometry with an estimated background](optical-instrument.md#aperture-photometry-with-an-estimated-background)
- [Approximate experimental design](design-of-experiments.md#approximate-experimental-design)
- [Arcsine distribution on a bounded interval](continuous-probability-distribution.md#arcsine-distribution-on-a-bounded-interval)
- [Arcsine quantiles and moments](continuous-probability-distribution.md#arcsine-quantiles-and-moments)
- [Arithmetic stock model with constant volatility](mathematical-finance.md#arithmetic-stock-model-with-constant-volatility)
- [Asymptotic mean integrated squared error](statistical-modelling.md#asymptotic-mean-integrated-squared-error)
- [Asymptotic mean squared error](statistical-modelling.md#asymptotic-mean-squared-error)
- [Asymptotic normality of the Watterson estimator](population-genetics.md#asymptotic-normality-of-the-watterson-estimator)
- [Atomic compound Poisson process with drift](stochastic-process.md#atomic-compound-poisson-process-with-drift)
- [Autocorrelation](time-series.md#autocorrelation)
- [Autocovariance](time-series.md#autocovariance)
- [Autocovariance of an AR(1) process](time-series.md#autocovariance-of-an-ar-1-process)
- [Autocovariance of an MA(1) process](time-series.md#autocovariance-of-an-ma-1-process)
- [Autoregressive conditional heteroscedasticity](time-series.md#autoregressive-conditional-heteroscedasticity)
- [Autoregressive process of order one](time-series.md#autoregressive-process-of-order-one)
- [Availability curvature and equilibrium fluctuations](thermodynamic-potential.md#availability-curvature-and-equilibrium-fluctuations)
- [Average conditional variance decreases with more information](#average-conditional-variance-decreases-with-more-information)
- [Balanced photodetection](optical-instrument.md#balanced-photodetection)
- [Barely-supercritical largest-component expectation](random-graph.md#barely-supercritical-largest-component-expectation)
- [Baseline covariate](statistical-model.md#baseline-covariate)
- [Bayesian posterior](bayesian-statistics.md#bayesian-posterior)
- [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution)
- [Bernoulli process](stochastic-process.md#bernoulli-process)
- [Bernstein polynomial](functional-analysis.md#bernstein-polynomial)
- [Best linear unbiased prediction](generalized-linear-model.md#best-linear-unbiased-prediction)
- [Beta-binomial distribution](bayesian-statistics.md#beta-binomial-distribution)
- [Beta distribution](probability-distribution.md#beta-distribution)
- [Between-study heterogeneity](statistical-inference.md#between-study-heterogeneity)
- [Bias and variance of a three-neighbour weighted smoother](statistical-learning.md#bias-and-variance-of-a-three-neighbour-weighted-smoother)
- [Bias of pooled flat-field ratio gain](optical-instrument.md#bias-of-pooled-flat-field-ratio-gain)
- [Biased random walk](random-walk.md#biased-random-walk)
- [Binomial distribution](discrete-probability-distribution.md#binomial-distribution)
- [Binomial proportion](discrete-probability-distribution.md#binomial-proportion)
- [Blackett-Occhialini triggered cloud-chamber experiment](particle-detection.md#blackett-occhialini-triggered-cloud-chamber-experiment)
- [Boxcar averaging of Poisson shot noise](electrical-engineering.md#boxcar-averaging-of-poisson-shot-noise)
- [Bragg wavelength error propagation](electromagnetic-radiation.md#bragg-wavelength-error-propagation)
- [Breathing Gaussian state in a harmonic oscillator](quantum-harmonic-oscillator.md#breathing-gaussian-state-in-a-harmonic-oscillator)
- [Brier score](statistical-inference.md#brier-score)
- [Brownian exit-skeleton clock convergence](brownian-motion.md#brownian-exit-skeleton-clock-convergence)
- [Brownian motion](brownian-motion.md)
- [Brownian scaling](brownian-motion.md#brownian-scaling)
- [Brownian symmetric interval-exit moments](brownian-motion.md#brownian-symmetric-interval-exit-moments)
- [Brownian zero mode of a fluctuating interface](stochastic-process.md#brownian-zero-mode-of-a-fluctuating-interface)
- [BUGS](bayesian-statistics.md#bugs)
- [Burn-in total variation comparison](bayesian-statistics.md#burn-in-total-variation-comparison)
- [Burstiness of queue input](queueing-theory.md#burstiness-of-queue-input)
- [Cameron-Martin space of a Gaussian random variable in a Banach space](gaussian-process.md#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space)
- [Canonical energy variance](canonical-ensemble.md#canonical-energy-variance)
- [Canonical gradient](statistical-inference.md#canonical-gradient)
- [Canonical identifiability of Gaussian ARMA models](time-series.md#canonical-identifiability-of-gaussian-arma-models)
- [Canonical partition function](canonical-ensemble.md#canonical-partition-function)
- [Cantelli inequality](probability-inequality.md#cantelli-inequality)
- [Capillary height-difference correlation](mathematical-biology.md#capillary-height-difference-correlation)
- [CCD noise budget](optical-instrument.md#ccd-noise-budget)
- [Center-point curvature contrast](design-of-experiments.md#center-point-curvature-contrast)
- [Centered truncation of a Wigner matrix](probability-theory.md#centered-truncation-of-a-wigner-matrix)
- [Central limit theorem](convergence-of-random-variables.md#central-limit-theorem)
- [Central limit theorem for a geometrically ergodic Markov chain](bayesian-statistics.md#central-limit-theorem-for-a-geometrically-ergodic-markov-chain)
- [Central moment](expected-value.md#central-moment)
- [Characteristic-function derivatives from finite absolute moments](characteristic-function.md#characteristic-function-derivatives-from-finite-absolute-moments)
- [Characteristic functions of symmetric sign sums](characteristic-function.md#characteristic-functions-of-symmetric-sign-sums)
- [Charge-transfer efficiency](optical-instrument.md#charge-transfer-efficiency)
- [Chebyshev's inequality](probability-inequality.md#chebyshev-s-inequality)
- [Chirped Gaussian wave packet](quantum-theory.md#chirped-gaussian-wave-packet)
- [Cholesky decomposition as a sum of squares](quadratic-form.md#cholesky-decomposition-as-a-sum-of-squares)
- [Claim count distribution](actuarial-statistics.md#claim-count-distribution)
- [Coefficient recovery and factorial moments of a probability generating function](probability-distribution.md#coefficient-recovery-and-factorial-moments-of-a-probability-generating-function)
- [Combining means of groups](arithmetic.md#combining-means-of-groups)
- [Common-coin averaging](random-variable.md#common-coin-averaging)
- [Compatibility of independent lifetime measurements](statistical-inference.md#compatibility-of-independent-lifetime-measurements)
- [Complex Wishart matrix](probability-theory.md#complex-wishart-matrix)
- [Compound Poisson cumulants](actuarial-statistics.md#compound-poisson-cumulants)
- [Compound-symmetry covariance](#compound-symmetry-covariance)
- [Conditional bootstrap variance of a sample mean](statistical-modelling.md#conditional-bootstrap-variance-of-a-sample-mean)
- [Conditional photon-number bias](quantum-optics.md#conditional-photon-number-bias)
- [Conditional variance](#conditional-variance)
- [Conditioning on a sum can create dependence](random-variable.md#conditioning-on-a-sum-can-create-dependence)
- [Confocal pinhole throughput](fluorescence.md#confocal-pinhole-throughput)
- [Constant intensity does not imply independence](probability-theory.md#constant-intensity-does-not-imply-independence)
- [Continuous-time symmetric simple random walk](stochastic-process.md#continuous-time-symmetric-simple-random-walk)
- [Control variates](monte-carlo-method.md#control-variates)
- [Convolution](fourier-analysis.md#convolution)
- [Correlated random-intercept and random-slope model](generalized-linear-model.md#correlated-random-intercept-and-random-slope-model)
- [Correlation matrix](#correlation-matrix)
- [Covariance](#covariance)
- [Covariance and bias of a ridge regression estimator](linear-regression.md#covariance-and-bias-of-a-ridge-regression-estimator)
- [Covariance criterion for diversification of factor residuals](mathematical-finance.md#covariance-criterion-for-diversification-of-factor-residuals)
- [Covariance function](stochastic-process.md#covariance-function)
- [Covariance induced by a shared latent variable](random-variable.md#covariance-induced-by-a-shared-latent-variable)
- [Covariance matrix](#covariance-matrix)
- [Cumulant](probability-distribution.md#cumulant)
- [Curie's law](statistical-physics.md#curie-s-law)
- [Cycles-per-time spectral density](time-series.md#cycles-per-time-spectral-density)
- [Dependence in Poisson thinning](poisson-process.md#dependence-in-poisson-thinning)
- [DerSimonian–Laird estimator](statistical-inference.md#dersimonian-laird-estimator)
- [Design effect](statistical-inference.md#design-effect)
- [Detector bias frame](optical-instrument.md#detector-bias-frame)
- [Detector conversion gain](optical-instrument.md#detector-conversion-gain)
- [Differentiable modification of a stationary Gaussian process](gaussian-process.md#differentiable-modification-of-a-stationary-gaussian-process)
- [Differential entropy of a Gaussian law](information-entropy.md#differential-entropy-of-a-gaussian-law)
- [Diffusive broadening of electrophoretic bands](physical-chemistry.md#diffusive-broadening-of-electrophoretic-bands)
- [Discrete Dupire equation](fundamental-theorem-of-asset-pricing.md#discrete-dupire-equation)
- [Discrete geometric average under the stock-numeraire measure](fundamental-theorem-of-asset-pricing.md#discrete-geometric-average-under-the-stock-numeraire-measure)
- [Discrete probability distribution](discrete-probability-distribution.md)
- [Discrete random variable](random-variable.md#discrete-random-variable)
- [Discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution)
- [Discrete uniform moments on an integer interval](discrete-probability-distribution.md#discrete-uniform-moments-on-an-integer-interval)
- [Discrete wavelet transform](fourier-analysis.md#discrete-wavelet-transform)
- [Doppler cooling](atomic-physics.md#doppler-cooling)
- [Dyadic quadratic variation of Brownian motion](stochastic-calculus.md#dyadic-quadratic-variation-of-brownian-motion)
- [Edgeworth series](probability-distribution.md#edgeworth-series)
- [Effective noise bandwidth](electrical-engineering.md#effective-noise-bandwidth)
- [Efficiency (statistics)](statistical-inference.md#efficiency-statistics)
- [Efron–Stein inequality](probability-inequality.md#efron-stein-inequality)
- [Electrical noise reduction](electrical-engineering.md#electrical-noise-reduction)
- [Ellipsoid rotational diffusion microscopy experiment](thermodynamics.md#ellipsoid-rotational-diffusion-microscopy-experiment)
- [EM for an independent missing normal coordinate](latent-variable.md#em-for-an-independent-missing-normal-coordinate)
- [EM maximization step](latent-variable.md#em-maximization-step)
- [Empirical distribution function](probability-distribution.md#empirical-distribution-function)
- [Empirical variance](statistical-inference.md#empirical-variance)
- [Entropy mode](ideal-magnetohydrodynamics.md#entropy-mode)
- [Entropy power](information-entropy.md#entropy-power)
- [Equal-cell replication variance formula](normal-linear-model.md#equal-cell-replication-variance-formula)
- [Equal-covariance Gaussian classification error](statistical-inference.md#equal-covariance-gaussian-classification-error)
- [Equality in Cantelli's inequality](probability-inequality.md#equality-in-cantelli-s-inequality)
- [Equality in Chebyshev's inequality](probability-inequality.md#equality-in-chebyshev-s-inequality)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Equipartition trap calibration](optics.md#equipartition-trap-calibration)
- [Estimator](statistical-modelling.md#estimator)
- [Even coherent-state superposition](quantum-optics.md#even-coherent-state-superposition)
- [Exact bootstrap distribution for three observations](statistical-modelling.md#exact-bootstrap-distribution-for-three-observations)
- [Exact Gaussian overflow constraint](queueing-theory.md#exact-gaussian-overflow-constraint)
- [Exact pooled two-sample t statistic](statistical-hypothesis-test.md#exact-pooled-two-sample-t-statistic)
- [Exact sampling of an Ornstein-Uhlenbeck process](gaussian-process.md#exact-sampling-of-an-ornstein-uhlenbeck-process)
- [Excess kurtosis](probability-distribution.md#excess-kurtosis)
- [Expectation-maximization algorithm](latent-variable.md#expectation-maximization-algorithm)
- [Expectation value](quantum-system.md#expectation-value)
- [Expected process variance](actuarial-statistics.md#expected-process-variance)
- [Expected value premium principle](actuarial-statistics.md#expected-value-premium-principle)
- [Explained variance of a principal component](statistical-learning.md#explained-variance-of-a-principal-component)
- [Exponential limit of a one-sided periodogram](time-series.md#exponential-limit-of-a-one-sided-periodogram)
- [Exponential Markov bound](probability-inequality.md#exponential-markov-bound)
- [Exponential-utility trading with Gaussian increments](mathematical-finance.md#exponential-utility-trading-with-gaussian-increments)
- [Exposure time for a Poisson rate at fixed fractional precision](generalized-linear-model.md#exposure-time-for-a-poisson-rate-at-fixed-fractional-precision)
- [Fano factor](#fano-factor)
- [Fano-limited X-ray CCD energy resolution](optical-instrument.md#fano-limited-x-ray-ccd-energy-resolution)
- [Fermi window](quantum-ideal-gas-statistics.md#fermi-window)
- [Field-squared quadrature](quantum-optics.md#field-squared-quadrature)
- [Fieller's theorem](statistical-inference.md#fieller-s-theorem)
- [Filtered shot noise](electrical-engineering.md#filtered-shot-noise)
- [Finite-dimensional distribution](stochastic-process.md#finite-dimensional-distribution)
- [Finite-exposure correction to fluctuation force calibration](electromagnetism.md#finite-exposure-correction-to-fluctuation-force-calibration)
- [Finite initialization of an AR(1) process](time-series.md#finite-initialization-of-an-ar-1-process)
- [Finite population correction](discrete-probability-distribution.md#finite-population-correction)
- [Finite-size rounding](statistical-physics.md#finite-size-rounding)
- [Finite-volume angular source selection](quantum-field-theory.md#finite-volume-angular-source-selection)
- [First moment method](probability-inequality.md#first-moment-method)
- [First-vertex degree in the LCD model](random-graph.md#first-vertex-degree-in-the-lcd-model)
- [Five-point symmetric quadratic trend smoother](time-series.md#five-point-symmetric-quadratic-trend-smoother)
- [Fixed-effect meta-analysis](statistical-inference.md#fixed-effect-meta-analysis)
- [Flicker noise](electrical-engineering.md#flicker-noise)
- [Fourier weight](analysis-of-boolean-functions.md#fourier-weight)
- [Fourth inverse-power sum of the cantilever spectrum](mathematical-biology.md#fourth-inverse-power-sum-of-the-cantilever-spectrum)
- [Fourth moment](expected-value.md#fourth-moment)
- [Fractional Brownian motion](gaussian-process.md#fractional-brownian-motion)
- [Franck-Hertz spacing fit and contact offset](energy-eigenvalue.md#franck-hertz-spacing-fit-and-contact-offset)
- [Free-filament variance with fixed translation and tilt](elasticity-physics.md#free-filament-variance-with-fixed-translation-and-tilt)
- [G-optimal design](design-of-experiments.md#g-optimal-design)
- [Gain estimation from flat-field ratios](optical-instrument.md#gain-estimation-from-flat-field-ratios)
- [Gamma frailty hazard ratio](survival-analysis.md#gamma-frailty-hazard-ratio)
- [Gamma random-intercept Poisson model](generalized-linear-model.md#gamma-random-intercept-poisson-model)
- [Gas clumping factor](fluid-mechanics.md#gas-clumping-factor)
- [Gaussian absolute-magnitude Malmquist shift](astrophysics.md#gaussian-absolute-magnitude-malmquist-shift)
- [Gaussian AR1 bridge](time-series.md#gaussian-ar1-bridge)
- [Gaussian Bayesian network](statistical-model.md#gaussian-bayesian-network)
- [Gaussian chain](mathematical-biology.md#gaussian-chain)
- [Gaussian change-point posterior with proper priors](probability-and-statistics.md#gaussian-change-point-posterior-with-proper-priors)
- [Gaussian characterization by independent sum and difference](probability-distribution.md#gaussian-characterization-by-independent-sum-and-difference)
- [Gaussian chirped pulse compression](laser.md#gaussian-chirped-pulse-compression)
- [Gaussian conditional variance from precision](#gaussian-conditional-variance-from-precision)
- [Gaussian diffusion of a smooth initial profile](multivariable-calculus.md#gaussian-diffusion-of-a-smooth-initial-profile)
- [Gaussian effective bandwidth](queueing-theory.md#gaussian-effective-bandwidth)
- [Gaussian even-moment pairing count](probability-distribution.md#gaussian-even-moment-pairing-count)
- [Gaussian filtering with exact observations](control-theory.md#gaussian-filtering-with-exact-observations)
- [Gaussian fourth moment](probability-distribution.md#gaussian-fourth-moment)
- [Gaussian independence of linear and quadratic statistics](probability-and-statistics.md#gaussian-independence-of-linear-and-quadratic-statistics)
- [Gaussian integral](integral.md#gaussian-integral)
- [Gaussian likelihood Gibbs annealing](mathematical-optimization.md#gaussian-likelihood-gibbs-annealing)
- [Gaussian log-response model](statistical-modelling.md#gaussian-log-response-model)
- [Gaussian mixture distribution](probability-distribution.md#gaussian-mixture-distribution)
- [Gaussian phase-screen correlation](partial-differential-equation.md#gaussian-phase-screen-correlation)
- [Gaussian process regression](gaussian-process.md#gaussian-process-regression)
- [Gaussian random variable](probability-distribution.md#gaussian-random-variable)
- [Gaussian random vector](probability-and-statistics.md#gaussian-random-vector)
- [Gaussian regression score](statistical-modelling.md#gaussian-regression-score)
- [Gaussian regression toward the mean](probability-and-statistics.md#gaussian-regression-toward-the-mean)
- [Gaussian semivariogram](statistical-modelling.md#gaussian-semivariogram)
- [Gaussian variational energy for the harmonic oscillator](quantum-theory.md#gaussian-variational-energy-for-the-harmonic-oscillator)
- [Geometric distribution](discrete-probability-distribution.md#geometric-distribution)
- [Geometric mutation count in a coalescent epoch](continuous-time-markov-chain.md#geometric-mutation-count-in-a-coalescent-epoch)
- [Geometric pair-number distribution](quantum-harmonic-oscillator.md#geometric-pair-number-distribution)
- [Grand-canonical single-level occupation variance](statistical-physics.md#grand-canonical-single-level-occupation-variance)
- [Grand-potential particle-number variance](statistical-physics.md#grand-potential-particle-number-variance)
- [Greenwood formula](survival-analysis.md#greenwood-formula)
- [Grouped Bernoulli failure counts](discrete-probability-distribution.md#grouped-bernoulli-failure-counts)
- [Haar density estimator](nonparametric-statistics.md#haar-density-estimator)
- [Haar projection estimator in Gaussian white noise](fourier-analysis.md#haar-projection-estimator-in-gaussian-white-noise)
- [Haar scaling function](fourier-analysis.md#haar-scaling-function)
- [Half-normal distribution](probability-distribution.md#half-normal-distribution)
- [Haploid selection recurrence](biology.md#haploid-selection-recurrence)
- [Harrison-Peebles-Zeldovich spectrum](linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum)
- [Hasselmann stochastic climate model](geophysics.md#hasselmann-stochastic-climate-model)
- [Heavy-tailed distribution](probability-distribution.md#heavy-tailed-distribution)
- [Heavy-traffic limit of a queue](queueing-theory.md#heavy-traffic-limit-of-a-queue)
- [Hedging a Gaussian income stream with exponential utility](mathematical-finance.md#hedging-a-gaussian-income-stream-with-exponential-utility)
- [Heisenberg uncertainty relation](quantum-theory.md#heisenberg-uncertainty-relation)
- [Hellinger distance between normal distributions](f-divergence.md#hellinger-distance-between-normal-distributions)
- [Heterogeneous individual claims model](actuarial-statistics.md#heterogeneous-individual-claims-model)
- [Heteroscedastic](statistical-modelling.md#heteroscedastic)
- [High-resolution quantization approximation](electrical-engineering.md#high-resolution-quantization-approximation)
- [Hoeffding inequality](probability-inequality.md#hoeffding-inequality)
- [Hoeffding lemma](probability-inequality.md#hoeffding-lemma)
- [Hoeffding projection](statistical-modelling.md#hoeffding-projection)
- [Hoeffding sample size for Bernoulli frequencies](probability-inequality.md#hoeffding-sample-size-for-bernoulli-frequencies)
- [Homoscedasticity](statistical-model.md#homoscedasticity)
- [Homoscedasticity and heteroscedasticity](statistical-modelling.md#homoscedasticity-and-heteroscedasticity)
- [Hurst exponent](gaussian-process.md#hurst-exponent)
- [Hydrogen rotational heat capacity](molecule.md#hydrogen-rotational-heat-capacity)
- [Hypergeometric distribution](discrete-probability-distribution.md#hypergeometric-distribution)
- [Identical-mean EM trap](latent-variable.md#identical-mean-em-trap)
- [IID does not imply finite moments](random-variable.md#iid-does-not-imply-finite-moments)
- [Importance sampling of a Cauchy tail](monte-carlo-method.md#importance-sampling-of-a-cauchy-tail)
- [Incremental net monetary benefit](statistical-inference.md#incremental-net-monetary-benefit)
- [Independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables)
- [Independent increments](stochastic-process.md#independent-increments)
- [Independent minimum and gap of two exponential variables](probability-theory.md#independent-minimum-and-gap-of-two-exponential-variables)
- [Independent mutation counts in coalescent epochs](continuous-time-markov-chain.md#independent-mutation-counts-in-coalescent-epochs)
- [Independent-record averaging versus high detector bandwidth](stochastic-process.md#independent-record-averaging-versus-high-detector-bandwidth)
- [Independent subgroup contrast in meta-analysis](statistical-inference.md#independent-subgroup-contrast-in-meta-analysis)
- [Indirect treatment comparison](statistical-inference.md#indirect-treatment-comparison)
- [Inertial Brownian displacement with zero initial velocity](stochastic-calculus.md#inertial-brownian-displacement-with-zero-initial-velocity)
- [Infinite divisibility (probability)](probability-distribution.md#infinite-divisibility-probability)
- [Influence function of the mean](robust-statistics.md#influence-function-of-the-mean)
- [Infrared qualification of a scale-invariant covariance](cosmic-inflation.md#infrared-qualification-of-a-scale-invariant-covariance)
- [Integrated Gaussian forward-rate process](mathematical-finance.md#integrated-gaussian-forward-rate-process)
- [Integrated Ornstein-Uhlenbeck displacement](gaussian-process.md#integrated-ornstein-uhlenbeck-displacement)
- [Integrated random-walk limit](convergence-of-random-variables.md#integrated-random-walk-limit)
- [Interior first-order bias cancellation for local constant regression](nonparametric-statistics.md#interior-first-order-bias-cancellation-for-local-constant-regression)
- [Intrinsically stationary random field](statistical-modelling.md#intrinsically-stationary-random-field)
- [Inverse-variance weight](statistical-modelling.md#inverse-variance-weight)
- [Inverse-variance weighted mean](statistical-modelling.md#inverse-variance-weighted-mean)
- [Ising ring bond correlation](spin-model.md#ising-ring-bond-correlation)
- [Ising ring magnetization fluctuations](spin-model.md#ising-ring-magnetization-fluctuations)
- [Isotropic cosmological correlation-power-spectrum relation](large-scale-structure-of-the-universe.md#isotropic-cosmological-correlation-power-spectrum-relation)
- [Isotropic turbulence](turbulence.md#isotropic-turbulence)
- [Jackknife bias correction](statistical-inference.md#jackknife-bias-correction)
- [Jackknife variance estimator](statistical-inference.md#jackknife-variance-estimator)
- [Jensen gap](real-analysis.md#jensen-gap)
- [Jensen's inequality](real-analysis.md#jensen-s-inequality)
- [Kahn-Kalai-Linial theorem](analysis-of-boolean-functions.md#kahn-kalai-linial-theorem)
- [Kalman filter](control-theory.md#kalman-filter)
- [Kalman filtering of a moving scalar state](control-theory.md#kalman-filtering-of-a-moving-scalar-state)
- [Kalman gain](control-theory.md#kalman-gain)
- [Kalman prediction step](control-theory.md#kalman-prediction-step)
- [Kernel density estimation](nonparametric-statistics.md#kernel-density-estimation)
- [Kolmogorov maximal inequality](martingale.md#kolmogorov-maximal-inequality)
- [Kriging](statistical-modelling.md#kriging)
- [Kundt tube spacing fit](linear-acoustics.md#kundt-tube-spacing-fit)
- [Kurtosis](probability-distribution.md#kurtosis)
- [L2 construction of compensated Poisson integrals](poisson-point-process.md#l2-construction-of-compensated-poisson-integrals)
- [Lack-of-fit F-test](normal-linear-model.md#lack-of-fit-f-test)
- [Lamb-Mössbauer factor](mossbauer-effect.md#lamb-mossbauer-factor)
- [Lamb shift line-centre model](atomic-physics.md#lamb-shift-line-centre-model)
- [Laplace distribution](continuous-probability-distribution.md#laplace-distribution)
- [Latent factor](latent-variable.md#latent-factor)
- [Lateral mobility of membrane proteins](cell-membrane.md#lateral-mobility-of-membrane-proteins)
- [Law of the unconscious statistician](expected-value.md#law-of-the-unconscious-statistician)
- [Law of total variance](probability-theory.md#law-of-total-variance)
- [Lehmann–Scheffé theorem](probability-and-statistics.md#lehmann-scheffe-theorem)
- [Likelihood-power annealing](mathematical-optimization.md#likelihood-power-annealing)
- [Lilliefors test](statistical-inference.md#lilliefors-test)
- [Limiting MA(1) innovations coefficient](time-series.md#limiting-ma-1-innovations-coefficient)
- [Lindeberg-Feller central limit theorem](convergence-of-random-variables.md#lindeberg-feller-central-limit-theorem)
- [Linkage disequilibrium](population-genetics.md#linkage-disequilibrium)
- [Lipschitz error bound for Bernstein approximation](functional-analysis.md#lipschitz-error-bound-for-bernstein-approximation)
- [Living versus terminating chain populations](polymer.md#living-versus-terminating-chain-populations)
- [Local-level state-space model](time-series.md#local-level-state-space-model)
- [Log absolute value stabilization of a normal scale family](statistical-inference.md#log-absolute-value-stabilization-of-a-normal-scale-family)
- [Log odds ratio](statistical-modelling.md#log-odds-ratio)
- [Log risk ratio](statistical-modelling.md#log-risk-ratio)
- [Logarithmic-regime giant component](random-graph.md#logarithmic-regime-giant-component)
- [Logistic interaction as a ratio of odds ratios](normal-linear-model.md#logistic-interaction-as-a-ratio-of-odds-ratios)
- [Lognormal intermittency model](turbulence.md#lognormal-intermittency-model)
- [Lossless two-channel thickness scattering model](optics.md#lossless-two-channel-thickness-scattering-model)
- [Luria-Delbrück experiment](genetics.md#luria-delbruck-experiment)
- [Lyapunov condition](convergence-of-random-variables.md#lyapunov-condition)
- [Manometer height-to-pressure calibration](fluid-mechanics.md#manometer-height-to-pressure-calibration)
- [Mantel–Haenszel pooled odds ratio](statistical-inference.md#mantel-haenszel-pooled-odds-ratio)
- [Marked-set connectivity threshold](random-graph.md#marked-set-connectivity-threshold)
- [Maximum likelihood estimation](maximum-likelihood-estimation.md)
- [Maxwell-Boltzmann velocity distribution](quantum-ideal-gas-statistics.md#maxwell-boltzmann-velocity-distribution)
- [MCAR auxiliary-variable efficiency](probability-and-statistics.md#mcar-auxiliary-variable-efficiency)
- [Mean and variance of a Galton-Watson generation](galton-watson-process.md#mean-and-variance-of-a-galton-watson-generation)
- [Mean displacement](classical-mechanics.md#mean-displacement)
- [Mean-square relative displacement in EXAFS](physics.md#mean-square-relative-displacement-in-exafs)
- [Mean squared displacement](brownian-motion.md#mean-squared-displacement)
- [Meta-analysis](statistical-inference.md#meta-analysis)
- [Minimum-variance combination of unbiased sample means](monte-carlo-method.md#minimum-variance-combination-of-unbiased-sample-means)
- [Minimum-variance importance distribution](monte-carlo-method.md#minimum-variance-importance-distribution)
- [Moderate deviation principle](convergence-of-random-variables.md#moderate-deviation-principle)
- [Molecular diffusion](thermodynamics.md#molecular-diffusion)
- [Moment equations of a linear birth-death process](continuous-time-markov-chain.md#moment-equations-of-a-linear-birth-death-process)
- [Moment matching for a beta prior](probability-distribution.md#moment-matching-for-a-beta-prior)
- [Moments of a marked Poisson integral](poisson-point-process.md#moments-of-a-marked-poisson-integral)
- [Moments of the mutation count on a neutral coalescent tree](continuous-time-markov-chain.md#moments-of-the-mutation-count-on-a-neutral-coalescent-tree)
- [Monte Carlo integration](monte-carlo-method.md#monte-carlo-integration)
- [Monte Carlo standard error](monte-carlo-method.md#monte-carlo-standard-error)
- [Moving average](electrical-engineering.md#moving-average)
- [Moving-average process of order one](time-series.md#moving-average-process-of-order-one)
- [Multinomial aggregation](discrete-probability-distribution.md#multinomial-aggregation)
- [Multinomial distribution](discrete-probability-distribution.md#multinomial-distribution)
- [Multiple-imputation confidence interval](probability-and-statistics.md#multiple-imputation-confidence-interval)
- [Natural visibility weighting](astrophysics.md#natural-visibility-weighting)
- [Negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution)
- [Nested measurements](design-of-experiments.md#nested-measurements)
- [Neutrino event classification model](particle-detection.md#neutrino-event-classification-model)
- [Noise sensitivity of a quadrature rule](numerical-integration.md#noise-sensitivity-of-a-quadrature-rule)
- [Normal approximation](convergence-of-random-variables.md#normal-approximation)
- [Normal approximation to a compound Poisson aggregate](actuarial-statistics.md#normal-approximation-to-a-compound-poisson-aggregate)
- [Normal distribution](probability-distribution.md#normal-distribution)
- [Normal-inverse-gamma prior](exponential-family.md#normal-inverse-gamma-prior)
- [Normal linear model maximum-likelihood sampling distributions](normal-linear-model.md#normal-linear-model-maximum-likelihood-sampling-distributions)
- [Normal mean posterior with an exponential prior](bayesian-statistics.md#normal-mean-posterior-with-an-exponential-prior)
- [Normal scale mixture representation of Student t](continuous-probability-distribution.md#normal-scale-mixture-representation-of-student-t)
- [Nugget effect](statistical-modelling.md#nugget-effect)
- [Number squeezing](quantum-optics.md#number-squeezing)
- [Number variance of an interacting defect](statistical-physics.md#number-variance-of-an-interacting-defect)
- [Offspring distribution of a branching process](galton-watson-process.md#offspring-distribution-of-a-branching-process)
- [On-off X-ray photon counting](astrophysics.md#on-off-x-ray-photon-counting)
- [One-electron defect plateau](statistical-physics.md#one-electron-defect-plateau)
- [One-sided spectral density of a real stationary time series](time-series.md#one-sided-spectral-density-of-a-real-stationary-time-series)
- [Optical squeezing degradation by loss](quantum-optics.md#optical-squeezing-degradation-by-loss)
- [Optical trap calibration uncertainty](optics.md#optical-trap-calibration-uncertainty)
- [Optical trap drag calibration](optics.md#optical-trap-drag-calibration)
- [Optical trap Langevin calibration](optics.md#optical-trap-langevin-calibration)
- [Optimal cost-constrained stratified sampling allocation](statistical-inference.md#optimal-cost-constrained-stratified-sampling-allocation)
- [Optimal experimental design](design-of-experiments.md#optimal-experimental-design)
- [Ordinary kriging](statistical-modelling.md#ordinary-kriging)
- [Ornstein-Uhlenbeck multiplicative amplification](gaussian-process.md#ornstein-uhlenbeck-multiplicative-amplification)
- [Ornstein-Uhlenbeck process](gaussian-process.md#ornstein-uhlenbeck-process)
- [Ornstein-Uhlenbeck stationary initialization](gaussian-process.md#ornstein-uhlenbeck-stationary-initialization)
- [Ornstein-Uhlenbeck transition distribution](gaussian-process.md#ornstein-uhlenbeck-transition-distribution)
- [Oscillator uncertainty and allocation of classical energy](quantum-harmonic-oscillator.md#oscillator-uncertainty-and-allocation-of-classical-energy)
- [Overdispersion of nondegenerate mixed Poisson counts](discrete-probability-distribution.md#overdispersion-of-nondegenerate-mixed-poisson-counts)
- [Paired log-rank reduction to a sign test](survival-analysis.md#paired-log-rank-reduction-to-a-sign-test)
- [Pairwise independent random variables](random-variable.md#pairwise-independent-random-variables)
- [Parametric-rate kernel estimation of a bandlimited density](nonparametric-statistics.md#parametric-rate-kernel-estimation-of-a-bandlimited-density)
- [Pareto moment threshold](continuous-probability-distribution.md#pareto-moment-threshold)
- [Pareto top shares and the 80/20 rule](continuous-probability-distribution.md#pareto-top-shares-and-the-80-20-rule)
- [Parity construction of pairwise independent bits](probability-theory.md#parity-construction-of-pairwise-independent-bits)
- [Parity estimator for a zero-truncated Poisson count](discrete-probability-distribution.md#parity-estimator-for-a-zero-truncated-poisson-count)
- [Partial correlation](#partial-correlation)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/b/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/d/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#13/c/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#7/c/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#7/e/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#7/f/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-genetics-course-of-the-university-of-cambridge/2025/paper-4.md#4/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-1.md#a1/b/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-1.md#e8/b/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-1.md#e8/c/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#4/f/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#4/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2.md#12f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41.md#3/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-54.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#10f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4.md#3h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#2/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#2/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#4/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-57.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-57.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-77.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1.md#18a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1.md#3h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4.md#12h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#5/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-39.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-39.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#3f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1.md#10h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1.md#21h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#4/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#4/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40.md#5/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-41.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-66.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#13i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#27i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#27i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#6e/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#13e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#13e/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#13e/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#6/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#6/viii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-43.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#5/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2.md#9f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1.md#18c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2.md#27j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46.md#3/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#5/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#5/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-73.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#18c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#7c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3.md#7b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#19c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#19c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#19c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-70.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#13j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#27i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#34e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-43.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-46.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-46.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-64.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2.md#9f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#28i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#13i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#17f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#25j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#29j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-34.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-34.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-37.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#4f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#4f/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#9f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#25i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#13j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#29i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#3/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-38.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#13j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#13j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#27k/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2.md#12f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2.md#9f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-44.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-44.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#2/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#3/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#3/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-74.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2.md#8h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-28.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-28.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-28.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#7h/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33.md#5/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#2/e/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#2/e/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#4/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#25j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#10j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#6/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-75.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#12f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#2/2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#3/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#3/3/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#3/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2.md#9f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#7d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#19h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#7h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#28k/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#5j/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#5j/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#26k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#27j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#5j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#26k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#6b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#12j/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#2/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#6c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#4/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#4/iii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-312.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#27k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2.md#4f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#15b/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#17g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#29j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#6e/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#30k/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#6c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#13j/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#14c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-122.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-331.md#1/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#12/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#12/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#12/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2.md#8/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#section-b/3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#15/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1.md#12/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2.md#17/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1.md#12/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#18/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#18/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#18/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#11/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#18/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#18/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#16/a/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2.md#16/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#14/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#16/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#16/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1.md#16/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#16/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#16/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#14/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#14/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#14/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#14/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2.md#5/c/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2012/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2014/paper-1.md#2/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2014/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2.md#section-a/4/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2.md#section-d/d12/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-1.md#section-a/4/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1.md#section-c/c11/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-c/c11/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-d/d13/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-d/d12/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-d/d12/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-d/d13/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-a/4/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b7/c/solution)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-a/2/solution)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2012/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3.md#1/e/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3.md#1/h/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3.md#2/a/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3.md#2/c/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2012/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2012/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2015/paper-1.md#4/d/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2016/paper-1.md#1/e/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017.md#2/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/5/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/6/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/6/b/solution)
- [Pearson correlation coefficient](#pearson-correlation-coefficient)
- [Perfect positive correlation](#perfect-positive-correlation)
- [Periodic utility indifference payment for Gaussian income](utility-function.md#periodic-utility-indifference-payment-for-gaussian-income)
- [Phase-dependent cat-state quadrature variance](quantum-optics.md#phase-dependent-cat-state-quadrature-variance)
- [Photodiode responsivity measurement](optical-instrument.md#photodiode-responsivity-measurement)
- [Photoelectron peak overlap and resolution](physical-chemistry.md#photoelectron-peak-overlap-and-resolution)
- [Photon statistics of a squeezed vacuum](quantum-harmonic-oscillator.md#photon-statistics-of-a-squeezed-vacuum)
- [Pinned capillary-wave correlation](mathematical-biology.md#pinned-capillary-wave-correlation)
- [Planar rotational diffusion](thermodynamics.md#planar-rotational-diffusion)
- [Pointwise minimax rate for Lipschitz regression](nonparametric-statistics.md#pointwise-minimax-rate-for-lipschitz-regression)
- [Poisson binomial distribution](discrete-probability-distribution.md#poisson-binomial-distribution)
- [Poisson counting in a coherent state](quantum-theory.md#poisson-counting-in-a-coherent-state)
- [Poisson cumulative probability at its growing mean](discrete-probability-distribution.md#poisson-cumulative-probability-at-its-growing-mean)
- [Poisson distribution](discrete-probability-distribution.md#poisson-distribution)
- [Poisson mixture](discrete-probability-distribution.md#poisson-mixture)
- [Poisson photon counting](electrical-engineering.md#poisson-photon-counting)
- [Poisson process](poisson-process.md)
- [Poisson score linearization under proportional variance](generalized-linear-model.md#poisson-score-linearization-under-proportional-variance)
- [Poisson slope information after eliminating an intercept](generalized-linear-model.md#poisson-slope-information-after-eliminating-an-intercept)
- [Poisson variance after sky subtraction](optical-instrument.md#poisson-variance-after-sky-subtraction)
- [Population principal component](statistical-learning.md#population-principal-component)
- [Portfolio diversification](mathematical-finance.md#portfolio-diversification)
- [Position uncertainty](quantum-system.md#position-uncertainty)
- [Posterior variance](bayesian-statistics.md#posterior-variance)
- [Power spectral density](electrical-engineering.md#power-spectral-density)
- [Preparation uncertainty](quantum-theory.md#preparation-uncertainty)
- [Principal component analysis on a correlation matrix](statistical-learning.md#principal-component-analysis-on-a-correlation-matrix)
- [Principal component score](statistical-learning.md#principal-component-score)
- [Prior probability](bayesian-statistics.md#prior-probability)
- [Probability generating function of an independent random sum](probability-distribution.md#probability-generating-function-of-an-independent-random-sum)
- [Probability generating function of an independent sum](probability-distribution.md#probability-generating-function-of-an-independent-sum)
- [Probability inequality](probability-inequality.md)
- [Probability theory](probability-theory.md)
- [Probable error](probability-distribution.md#probable-error)
- [Propagation of uncertainty](wave-equation.md#propagation-of-uncertainty)
- [Quadrature squeezing](quantum-optics.md#quadrature-squeezing)
- [Quantum state tomography](quantum-measurement.md#quantum-state-tomography)
- [Quasibinomial regression](generalized-linear-model.md#quasibinomial-regression)
- [Quota share comparison at matched retained variance](actuarial-statistics.md#quota-share-comparison-at-matched-retained-variance)
- [Quota share reinsurance](actuarial-statistics.md#quota-share-reinsurance)
- [Radial moments of an isotropic Gaussian vector](probability-distribution.md#radial-moments-of-an-isotropic-gaussian-vector)
- [Radius of gyration](polymer.md#radius-of-gyration)
- [Radius sensitivity in the Perrin sedimentation experiment](brownian-motion.md#radius-sensitivity-in-the-perrin-sedimentation-experiment)
- [Random-design nonparametric regression](nonparametric-statistics.md#random-design-nonparametric-regression)
- [Random-effects meta-analysis](statistical-inference.md#random-effects-meta-analysis)
- [Random measurement error](probability-and-statistics.md#random-measurement-error)
- [Random-phase amplitude and the Rayleigh distribution](continuous-probability-distribution.md#random-phase-amplitude-and-the-rayleigh-distribution)
- [Random sum of independent claims](actuarial-statistics.md#random-sum-of-independent-claims)
- [Random variable](random-variable.md)
- [Random-walk maximum limit from Donsker invariance](convergence-of-random-variables.md#random-walk-maximum-limit-from-donsker-invariance)
- [Randomly shifted lattice point process](probability-theory.md#randomly-shifted-lattice-point-process)
- [Range of a semivariogram](statistical-modelling.md#range-of-a-semivariogram)
- [Rao-Blackwell estimator for a uniform scale interval](probability-and-statistics.md#rao-blackwell-estimator-for-a-uniform-scale-interval)
- [Rao-Blackwellization of a multinomial probability product](probability-and-statistics.md#rao-blackwellization-of-a-multinomial-probability-product)
- [Rare-outlier three-point distribution](probability-distribution.md#rare-outlier-three-point-distribution)
- [Raw moment recursion for a compound Poisson distribution](actuarial-statistics.md#raw-moment-recursion-for-a-compound-poisson-distribution)
- [Rayleigh distribution](continuous-probability-distribution.md#rayleigh-distribution)
- [Rayleigh radius from Gaussian components](continuous-probability-distribution.md#rayleigh-radius-from-gaussian-components)
- [Refinement variance identity for regularity energy](probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy)
- [Refractive-index uncertainty from Snell's law](wave-equation.md#refractive-index-uncertainty-from-snell-s-law)
- [Regression diagnostics](linear-regression.md#regression-diagnostics)
- [Regression outlier](linear-regression.md#regression-outlier)
- [Release-expansion thermometry](atomic-physics.md#release-expansion-thermometry)
- [Repeated-measurement latent signal model](probability-and-statistics.md#repeated-measurement-latent-signal-model)
- [Replication in experimental design](design-of-experiments.md#replication-in-experimental-design)
- [Residual estimate of Gaussian noise variance](normal-linear-model.md#residual-estimate-of-gaussian-noise-variance)
- [Residual estimate of slope uncertainty through the origin](normal-linear-model.md#residual-estimate-of-slope-uncertainty-through-the-origin)
- [Resistor-capacitor equilibrium noise](electrical-engineering.md#resistor-capacitor-equilibrium-noise)
- [Retained compound Poisson aggregate](actuarial-statistics.md#retained-compound-poisson-aggregate)
- [Retained stop loss moments for an exponential aggregate](actuarial-statistics.md#retained-stop-loss-moments-for-an-exponential-aggregate)
- [Rigid-motion-projected thermal covariance of a free filament](elasticity-physics.md#rigid-motion-projected-thermal-covariance-of-a-free-filament)
- [Robertson uncertainty principle](quantum-theory.md#robertson-uncertainty-principle)
- [Rotational diffusion](thermodynamics.md#rotational-diffusion)
- [Rubin's rules](probability-and-statistics.md#rubin-s-rules)
- [Sample mean of iid Bernoulli variables](random-variable.md#sample-mean-of-iid-bernoulli-variables)
- [Sample mean sufficiency depends on the model](probability-and-statistics.md#sample-mean-sufficiency-depends-on-the-model)
- [Sample mean under simple random sampling](statistical-inference.md#sample-mean-under-simple-random-sampling)
- [Sample size for comparing two proportions](probability-and-statistics.md#sample-size-for-comparing-two-proportions)
- [Sampling fraction](statistical-inference.md#sampling-fraction)
- [Sampling uncertainty of an endpoint diffusivity estimate](stokes-flow.md#sampling-uncertainty-of-an-endpoint-diffusivity-estimate)
- [Scalar Gaussian Kalman recursion](control-theory.md#scalar-gaussian-kalman-recursion)
- [Second moment](expected-value.md#second-moment)
- [Second-moment bound for positivity](probability-inequality.md#second-moment-bound-for-positivity)
- [Second moment method](probability-inequality.md#second-moment-method)
- [Shared zero-inflated Gamma-Poisson count model](statistical-modelling.md#shared-zero-inflated-gamma-poisson-count-model)
- [Sharp subcritical largest-component scale](probabilistic-combinatorics.md#sharp-subcritical-largest-component-scale)
- [Short-scale variance modulation by local non-Gaussianity](cosmology.md#short-scale-variance-modulation-by-local-non-gaussianity)
- [Shot noise](electrical-engineering.md#shot-noise)
- [Shot noise counting model](electrical-engineering.md#shot-noise-counting-model)
- [Shot noise departures from Poisson statistics](electrical-engineering.md#shot-noise-departures-from-poisson-statistics)
- [Shot noise photocurrent measurement](electrical-engineering.md#shot-noise-photocurrent-measurement)
- [Shot noise worked example](electrical-engineering.md#shot-noise-worked-example)
- [Sill of a semivariogram](statistical-modelling.md#sill-of-a-semivariogram)
- [Simple kriging](statistical-modelling.md#simple-kriging)
- [Simple linear regression](linear-regression.md#simple-linear-regression)
- [Simple random sampling](statistical-inference.md#simple-random-sampling)
- [Simple random walk](random-walk.md#simple-random-walk)
- [Simple random walk on the integer line](random-walk.md#simple-random-walk-on-the-integer-line)
- [Single-observation location minimax bound](statistical-model.md#single-observation-location-minimax-bound)
- [Skorokhod embedding theorem](martingale.md#skorokhod-embedding-theorem)
- [Slepian's lemma](gaussian-process.md#slepian-s-lemma)
- [Smoothing bandwidth](nonparametric-statistics.md#smoothing-bandwidth)
- [Spectral phase in pulse compression](laser.md#spectral-phase-in-pulse-compression)
- [Spectral representation theorem for a stationary time series](time-series.md#spectral-representation-theorem-for-a-stationary-time-series)
- [Spin expectation value](quantum-system.md#spin-expectation-value)
- [Square-root tail bound for martingale absorption](martingale.md#square-root-tail-bound-for-martingale-absorption)
- [Squeezed thermal state](quantum-system.md#squeezed-thermal-state)
- [Standard deviation](#standard-deviation)
- [Standard Gaussian random vector](probability-and-statistics.md#standard-gaussian-random-vector)
- [Standard normal distribution](probability-distribution.md#standard-normal-distribution)
- [Standard normal random variable](probability-distribution.md#standard-normal-random-variable)
- [Standard score](probability-theory.md#standard-score)
- [Standardized Euclidean distance](topological-analysis.md#standardized-euclidean-distance)
- [Standardized regression residual](probability-and-statistics.md#standardized-regression-residual)
- [Stationary covariance bound for reversible Markov chains](bayesian-statistics.md#stationary-covariance-bound-for-reversible-markov-chains)
- [Stationary increments](stochastic-process.md#stationary-increments)
- [Stationary process](time-series.md#stationary-process)
- [Stationary trapped Brownian displacement](gaussian-process.md#stationary-trapped-brownian-displacement)
- [Statistical physics](statistical-physics.md)
- [Stern-Gerlach discrete and classical profiles](angular-momentum-operator.md#stern-gerlach-discrete-and-classical-profiles)
- [Stochastic cooling variance model](particle-accelerator.md#stochastic-cooling-variance-model)
- [Stochastic process](stochastic-process.md)
- [Stock-delivery option with a geometric average](fundamental-theorem-of-asset-pricing.md#stock-delivery-option-with-a-geometric-average)
- [Stop loss variance minimization principle](actuarial-statistics.md#stop-loss-variance-minimization-principle)
- [Stratified log-rank statistic](survival-analysis.md#stratified-log-rank-statistic)
- [Strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers)
- [Student's t-distribution](continuous-probability-distribution.md#student-s-t-distribution)
- [Student t random-effect model](statistical-inference.md#student-t-random-effect-model)
- [Sub-step estimation with uniform dither](electrical-engineering.md#sub-step-estimation-with-uniform-dither)
- [Symmetric stable distribution](probability-distribution.md#symmetric-stable-distribution)
- [Tagged-label Rayleigh quotient for adjacent transpositions](markov-chain.md#tagged-label-rayleigh-quotient-for-adjacent-transpositions)
- [Thermal calibration of an optical trap](optics.md#thermal-calibration-of-an-optical-trap)
- [Thermal covariance of an elastic filament](elasticity-physics.md#thermal-covariance-of-an-elastic-filament)
- [Thermal diffusion length](heat.md#thermal-diffusion-length)
- [Thermal light](quantum-optics.md#thermal-light)
- [Thermal noise spectral convention](electrical-engineering.md#thermal-noise-spectral-convention)
- [Third-order pointwise kernel error bound](nonparametric-statistics.md#third-order-pointwise-kernel-error-bound)
- [Time series](time-series.md)
- [Time-sliced diffusion path integral](quantum-field-theory.md#time-sliced-diffusion-path-integral)
- [Total differential](multivariable-calculus.md#total-differential)
- [Total variance stationary condition for excess of loss](actuarial-statistics.md#total-variance-stationary-condition-for-excess-of-loss)
- [Transform-limited pulse](optics.md#transform-limited-pulse)
- [Translational and two-level energy variance](canonical-ensemble.md#translational-and-two-level-energy-variance)
- [Transverse energy instability of nonconstant temperature rolls](dynamical-systems.md#transverse-energy-instability-of-nonconstant-temperature-rolls)
- [Trapped-ion fluorescence count model](atomic-physics.md#trapped-ion-fluorescence-count-model)
- [Treatment contrast](normal-linear-model.md#treatment-contrast)
- [Two-Gaussian mixture example](statistical-modelling.md#two-gaussian-mixture-example)
- [Two-predictor variance inflation](normal-linear-model.md#two-predictor-variance-inflation)
- [Two-sided stationary inverse of an autoregressive polynomial](time-series.md#two-sided-stationary-inverse-of-an-autoregressive-polynomial)
- [Two-step prediction for an MA(1) process](time-series.md#two-step-prediction-for-an-ma-1-process)
- [Typical-set concentration for a biased coin](information-theory.md#typical-set-concentration-for-a-biased-coin)
- [Unbiased endpoint estimator for a shifted exponential sample](statistical-modelling.md#unbiased-endpoint-estimator-for-a-shifted-exponential-sample)
- [Unbiased likelihood estimator](bayesian-statistics.md#unbiased-likelihood-estimator)
- [Uniform distribution with an atom at zero](probability-distribution.md#uniform-distribution-with-an-atom-at-zero)
- [Uniform minimum variance conditionally unbiased estimator](statistical-modelling.md#uniform-minimum-variance-conditionally-unbiased-estimator)
- [Uniform order statistic](probability-theory.md#uniform-order-statistic)
- [Uniformly minimum-variance unbiased estimator](statistical-modelling.md#uniformly-minimum-variance-unbiased-estimator)
- [Universal kriging](statistical-modelling.md#universal-kriging)
- [Unknown-variance risk estimation in a saturated Gaussian model](statistical-inference.md#unknown-variance-risk-estimation-in-a-saturated-gaussian-model)
- [Unnormalized time autocorrelation](stochastic-process.md#unnormalized-time-autocorrelation)
- [Unsmoothed matter-density reduced skewness](large-scale-structure-of-the-universe.md#unsmoothed-matter-density-reduced-skewness)
- [Upper-truncated Poisson distribution](discrete-probability-distribution.md#upper-truncated-poisson-distribution)
- [Variance](variance.md)
- [Variance comparison for compound portfolio approximations](actuarial-statistics.md#variance-comparison-for-compound-portfolio-approximations)
- [Variance-minimizing exponential retention](actuarial-statistics.md#variance-minimizing-exponential-retention)
- [Variance-minimizing quota share split](actuarial-statistics.md#variance-minimizing-quota-share-split)
- [Variance-minimizing retention for shape-three Pareto claims](actuarial-statistics.md#variance-minimizing-retention-for-shape-three-pareto-claims)
- [Variance of a fitted regression mean](normal-linear-model.md#variance-of-a-fitted-regression-mean)
- [Variance of a long-time mean in a harmonic trap](gaussian-process.md#variance-of-a-long-time-mean-in-a-harmonic-trap)
- [Variance of a sample mean](expected-value.md#variance-of-a-sample-mean)
- [Variance of an estimator](statistical-modelling.md#variance-of-an-estimator)
- [Variance of hypothetical means](actuarial-statistics.md#variance-of-hypothetical-means)
- [Variance of nested measurements](design-of-experiments.md#variance-of-nested-measurements)
- [Variance of the Watterson estimator](population-genetics.md#variance-of-the-watterson-estimator)
- [Variance-stabilizing transformation](statistical-inference.md#variance-stabilizing-transformation)
- [Velocity moments of an isotropic Mestel disk](astrophysical-disk.md#velocity-moments-of-an-isotropic-mestel-disk)
- [Visibility-domain matched filter](electrical-engineering.md#visibility-domain-matched-filter)
- [Volume fluctuations of a closed gas bubble](statistical-physics.md#volume-fluctuations-of-a-closed-gas-bubble)
- [Waiting time to observe both Bernoulli outcomes](discrete-probability-distribution.md#waiting-time-to-observe-both-bernoulli-outcomes)
- [Wavelet regression estimator](nonparametric-statistics.md#wavelet-regression-estimator)
- [Weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers)
- [Weakly stationary process](time-series.md#weakly-stationary-process)
- [Weighted realized variance](stochastic-calculus.md#weighted-realized-variance)
- [Welch's t-test](statistical-hypothesis-test.md#welch-s-t-test)
- [White noise](time-series.md#white-noise)
- [White-noise likelihood for a square-integrable shift](gaussian-process.md#white-noise-likelihood-for-a-square-integrable-shift)
- [Wigner matrix](probability-theory.md#wigner-matrix)
- [Wilcoxon signed-rank statistic](nonparametric-statistics.md#wilcoxon-signed-rank-statistic)
- [Wild bootstrap](statistical-modelling.md#wild-bootstrap)
- [WinBUGS](bayesian-statistics.md#winbugs)
- [Wire-address position model](particle-detection.md#wire-address-position-model)
- [Work in a two-level sudden quench](quantum-mechanics.md#work-in-a-two-level-sudden-quench)
- [Working correlation matrix](statistical-inference.md#working-correlation-matrix)
- [Yule-Walker equations](time-series.md#yule-walker-equations)
- [Zero-energy filament mode](elasticity-physics.md#zero-energy-filament-mode)
- [Zero-inflated negative binomial model](statistical-modelling.md#zero-inflated-negative-binomial-model)
- [Zero-residual degeneracy of regression prediction](statistical-inference.md#zero-residual-degeneracy-of-regression-prediction)
- [Zero-variance boundary of an overflow constraint](queueing-theory.md#zero-variance-boundary-of-an-overflow-constraint)
