# Statistical hypothesis test

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_hypothesis_test)

Statistical hypothesis testing compares data against a null hypothesis using a controlled rejection probability.

**Table of contents**

- [False alarm rate](#false-alarm-rate)
- [Statistical hypothesis](#statistical-hypothesis)
- [Sequential probability ratio test](#sequential-probability-ratio-test)
- [Statistical significance](#statistical-significance)
  - [Poisson tail discovery probability](#poisson-tail-discovery-probability)
  - [Look-elsewhere effect](#look-elsewhere-effect)
- [Two-sided hypothesis test](#two-sided-hypothesis-test)
- [One-sided hypothesis test](#one-sided-hypothesis-test)
- [Alternative hypothesis](#alternative-hypothesis)
- [Hotelling's T-squared statistic](#hotelling-s-t-squared-statistic)
  - [Affine invariance of Hotelling's statistic](#affine-invariance-of-hotelling-s-statistic)
  - [Hotelling test of linear hypotheses](#hotelling-test-of-linear-hypotheses)
    - [Second-difference test of a linear mean profile](#second-difference-test-of-a-linear-mean-profile)
- [Rejection region](#rejection-region)
- [McNemar's test](#mcnemar-s-test)
  - [Equality criterion for paired and unpaired allele tests](#equality-criterion-for-paired-and-unpaired-allele-tests)
  - [Paired binary sample size calculation](#paired-binary-sample-size-calculation)
- [Significant and nonsignificant results need not differ significantly](#significant-and-nonsignificant-results-need-not-differ-significantly)
- [Monte Carlo test](#monte-carlo-test)
- [Predictive discrepancy statistic](#predictive-discrepancy-statistic)
- [Scan statistic](#scan-statistic)
  - [Cyclic interval overlap bound](#cyclic-interval-overlap-bound)
  - [Quadratic scan statistic](#quadratic-scan-statistic)
- [Least-favourable null configuration](#least-favourable-null-configuration)
- [Pearson chi-squared test of homogeneity](#pearson-chi-squared-test-of-homogeneity)
  - [Empty groups in a binomial homogeneity test](#empty-groups-in-a-binomial-homogeneity-test)
  - [Pearson chi-squared statistic for contingency tables](#pearson-chi-squared-statistic-for-contingency-tables)
    - [Yates's correction for continuity](#yates-s-correction-for-continuity)
- [Statistical test](#statistical-test)
  - [Most powerful test](#most-powerful-test)
- [Test statistic](#test-statistic)
- [Student's t-test](#student-s-t-test)
  - [Welch's t-test](#welch-s-t-test)
  - [Exact pooled two-sample t statistic](#exact-pooled-two-sample-t-statistic)
  - [Normal-mean likelihood ratio with unknown variance](#normal-mean-likelihood-ratio-with-unknown-variance)
  - [Regression coefficient test power ignores nuisance coefficients](#regression-coefficient-test-power-ignores-nuisance-coefficients)
- [Fixed alternative](#fixed-alternative)
- [Local alternative](#local-alternative)
- [Randomization test](#randomization-test)
  - [Conditional randomization test](#conditional-randomization-test)
  - [Permutation test](#permutation-test)
  - [Sign-flip randomization test](#sign-flip-randomization-test)
- [Null hypothesis](#null-hypothesis)
- [Simple hypothesis](#simple-hypothesis)
- [Size of a statistical test](#size-of-a-statistical-test)
- [Significance level](#significance-level)
- [P-value](#p-value)
  - [Super-uniform random variable](#super-uniform-random-variable)
- [Fisher's exact test](#fisher-s-exact-test)
  - [Exact power of Fisher's exact test](#exact-power-of-fisher-s-exact-test)
- [Maximin test](#maximin-test)
- [Multiple hypothesis testing](#multiple-hypothesis-testing)
  - [Intersection hypothesis](#intersection-hypothesis)
    - [Closure of a family of statistical hypotheses](#closure-of-a-family-of-statistical-hypotheses)
  - [Hochberg procedure](#hochberg-procedure)
  - [Simes inequality](#simes-inequality)
    - [Simes test](#simes-test)
  - [Weighted interval testing for a piecewise-constant mean](#weighted-interval-testing-for-a-piecewise-constant-mean)
  - [Intersection-union test](#intersection-union-test)
  - [Bonferroni correction](#bonferroni-correction)
    - [Weighted Bonferroni correction](#weighted-bonferroni-correction)
      - [Weighted Holm step-down procedure](#weighted-holm-step-down-procedure)
    - [Holm–Bonferroni method](#holm-bonferroni-method)
      - [First true null argument for Holm control](#first-true-null-argument-for-holm-control)
  - [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure)
    - [Benjamini-Hochberg leave-one-out identity](#benjamini-hochberg-leave-one-out-identity)
      - [Benjamini-Hochberg leave-two-out identity](#benjamini-hochberg-leave-two-out-identity)
        - [Second moment of the Benjamini-Hochberg false discovery proportion](#second-moment-of-the-benjamini-hochberg-false-discovery-proportion)
      - [Exact false discovery rate under independent null p-values](#exact-false-discovery-rate-under-independent-null-p-values)
  - [False discovery rate](#false-discovery-rate)
    - [False discovery proportion](#false-discovery-proportion)
  - [Familywise error rate](#familywise-error-rate)
    - [Familywise error control for a laminar hypothesis family](#familywise-error-control-for-a-laminar-hypothesis-family)
  - [Closed testing procedure](#closed-testing-procedure)
    - [Closed-testing control of the familywise error rate](#closed-testing-control-of-the-familywise-error-rate)
- [Joint hypothesis test](#joint-hypothesis-test)
- [Power function of a statistical test](#power-function-of-a-statistical-test)
- [Uniformly most powerful test](#uniformly-most-powerful-test)
  - [Crossing-power obstruction to a uniformly most powerful test](#crossing-power-obstruction-to-a-uniformly-most-powerful-test)
- [Pearson's chi-squared test](#pearson-s-chi-squared-test)
  - [Pearson chi-squared goodness-of-fit test](#pearson-chi-squared-goodness-of-fit-test)
    - [Binomial goodness-of-fit with an estimated parameter](#binomial-goodness-of-fit-with-an-estimated-parameter)
    - [Pearson chi-squared test of independence](#pearson-chi-squared-test-of-independence)
- [Likelihood-ratio test of independence in a contingency table](#likelihood-ratio-test-of-independence-in-a-contingency-table)
  - [Aggregation can change a contingency-table independence test](#aggregation-can-change-a-contingency-table-independence-test)
- [Linear-by-linear association test](#linear-by-linear-association-test)
- [Wald test](#wald-test)
  - [Signed normal Wald statistic](#signed-normal-wald-statistic)
  - [Wald statistics with a shared control](#wald-statistics-with-a-shared-control)
  - [Multivariate Wald statistic](#multivariate-wald-statistic)
    - [Wald statistic for linear restrictions](#wald-statistic-for-linear-restrictions)
  - [Wald and likelihood-ratio asymptotic equivalence](#wald-and-likelihood-ratio-asymptotic-equivalence)
  - [Two-sided Gaussian p-value](#two-sided-gaussian-p-value)
- [Likelihood-ratio test](#likelihood-ratio-test)
  - [Gaussian covariance diagonality likelihood-ratio test](#gaussian-covariance-diagonality-likelihood-ratio-test)
  - [Gaussian diagonal-covariance likelihood-ratio test](#gaussian-diagonal-covariance-likelihood-ratio-test)
  - [One-sided likelihood-ratio test for two normal variances](#one-sided-likelihood-ratio-test-for-two-normal-variances)
  - [Boundary likelihood-ratio test for two Gaussian means](#boundary-likelihood-ratio-test-for-two-gaussian-means)
  - [Single-parameter boundary likelihood-ratio test](#single-parameter-boundary-likelihood-ratio-test)
  - [Variance-component likelihood-ratio test at a boundary](#variance-component-likelihood-ratio-test-at-a-boundary)
    - [Location-scale invariant simulation test for a Gaussian variance component](#location-scale-invariant-simulation-test-for-a-gaussian-variance-component)
  - [Likelihood ratio](#likelihood-ratio)
    - [Log-likelihood ratio](#log-likelihood-ratio)
  - [Likelihood-ratio test statistic](#likelihood-ratio-test-statistic)
    - [Bartlett correction](#bartlett-correction)
      - [Bartlett-corrected likelihood-ratio statistic](#bartlett-corrected-likelihood-ratio-statistic)
      - [Bartlett correction coefficient](#bartlett-correction-coefficient)
        - [Bartlett correction for a normal variance with unknown mean](#bartlett-correction-for-a-normal-variance-with-unknown-mean)
  - [Generalized likelihood-ratio test](#generalized-likelihood-ratio-test)
    - [Likelihood-ratio test of area-proportional Poisson means](#likelihood-ratio-test-of-area-proportional-poisson-means)
    - [Analysis of deviance for nested generalized linear models](#analysis-of-deviance-for-nested-generalized-linear-models)
      - [Residual deviance](#residual-deviance)
        - [Null deviance](#null-deviance)
    - [Likelihood-ratio test for equality of two normal means](#likelihood-ratio-test-for-equality-of-two-normal-means)
    - [Nested likelihood-ratio rejection regions](#nested-likelihood-ratio-rejection-regions)
- [Score test](#score-test)
  - [Restricted maximum-likelihood estimator](#restricted-maximum-likelihood-estimator)
  - [Score test under a simple null](#score-test-under-a-simple-null)
    - [Quadratic form of a standard normal vector](#quadratic-form-of-a-standard-normal-vector)
  - [Residual sum of squares in a normal sample](#residual-sum-of-squares-in-a-normal-sample)
    - [Chi-square central limit theorem](#chi-square-central-limit-theorem)
- [Neyman-Pearson lemma](#neyman-pearson-lemma)
  - [Most powerful test for a Laplace location shift](#most-powerful-test-for-a-laplace-location-shift)
  - [Minimum sum of errors in a simple hypothesis test](#minimum-sum-of-errors-in-a-simple-hypothesis-test)
  - [Exponential-rate likelihood-ratio test](#exponential-rate-likelihood-ratio-test)
  - [Uniformly most powerful test for an exponential rate](#uniformly-most-powerful-test-for-an-exponential-rate)
  - [Monotone likelihood ratio](#monotone-likelihood-ratio)
    - [Posterior odds are monotone under a monotone likelihood ratio](#posterior-odds-are-monotone-under-a-monotone-likelihood-ratio)
    - [Monotone test](#monotone-test)
    - [Karlin-Rubin theorem](#karlin-rubin-theorem)
      - [Uniformly most powerful upper-tail test for a logistic location](#uniformly-most-powerful-upper-tail-test-for-a-logistic-location)

## False alarm rate

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

The expected rate of detections exceeding a stated threshold under a specified background-only model. A time rate and a per-trial [significance level](#significance-level) require different normalizations.

## Statistical hypothesis

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A [statistical hypothesis](#statistical-hypothesis) is a specified set of possible data-generating [probability distributions](probability-distribution.md), usually expressed as a restriction on model parameters. A simple [statistical hypothesis](#statistical-hypothesis) specifies one distribution; a composite [statistical hypothesis](#statistical-hypothesis) permits several. A [hypothesis test](statistical-hypothesis-test.md) compares a [null hypothesis](#null-hypothesis) with an [alternative hypothesis](#alternative-hypothesis) using a statistic calibrated under the null.

## Sequential probability ratio test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A [sequential probability ratio test](#sequential-probability-ratio-test) accumulates the [log-likelihood ratio](#log-likelihood-ratio) for two specified simple [statistical hypotheses](#statistical-hypothesis) until it reaches an upper or lower boundary. An upper crossing favors the alternative, a lower crossing favors the null, and observations continue between them. Error-calibrated boundaries are approximately $\log[(1-\beta)/\alpha]$ and $\log[\beta/(1-\alpha)]$; discrete overshoot means these approximations need calibration.

## Statistical significance

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_significance)

A result is [statistically significant](#statistical-significance) at a specified [significance level](#significance-level) $\alpha$ when its valid [p-value](#p-value) is at most $\alpha$ and the corresponding [null hypothesis](#null-hypothesis) is rejected. Significance does not measure effect size, establish practical importance, or give the probability that the null is true. Software stars encode thresholds for $p$-values; they do not supply an additional statistic.

### Poisson tail discovery probability

↑ **Parent:** [Statistical significance](#statistical-significance)

For a known background rate $b$ observed for exposure $T$, independent events give a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with mean $\mu_b=bT$. An excess-count test of the background-only [null hypothesis](#null-hypothesis) uses the upper-tail [P-value](#p-value) in the title. The tail, rather than the probability of exactly $n$, counts all outcomes at least as discrepant in the chosen direction.

This probability is conditional on the null model; it is not the posterior probability that the null model is true. A stipulated discovery threshold is met only when the tail is below that threshold. Uncertainty in the background rate or selecting among many searches needs additional modelling rather than being absorbed into the same known-mean formula.

### Look-elsewhere effect

↑ **Parent:** [Statistical significance](#statistical-significance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Look-elsewhere_effect)

Searching many possible signal locations increases the chance of finding an apparently unusual fluctuation somewhere. A local [p-value](#p-value) for a specified location differs from the global [p-value](#p-value) for the search over locations.[Section 7](physics-bibliography.md#observation-of-a-new-particle-in-the-search-for-the-standard-model-higgs-boson-with-the-atlas-detector-at-the-lhc-by-atlas-collaboration)

## Two-sided hypothesis test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A [two-sided test](#two-sided-hypothesis-test) detects departures in either direction from the [null hypothesis](#null-hypothesis), for example $\theta\ne\theta_0$. With a continuous symmetric null statistic centred at zero, its [p-value](#p-value) is $P_0(|T|\ge|t_{\mathrm{obs}}|)=2P_0(T\ge|t_{\mathrm{obs}}|)$. This is the usual coefficient test printed by Gaussian regression summaries, unlike a directional one-sided comparison.

## One-sided hypothesis test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A [one-sided test](#one-sided-hypothesis-test) targets deviations in one specified direction, such as $\theta>\theta_0$. If larger values of a statistic $T$ indicate this direction, its [p-value](#p-value) is an upper-tail null probability $P_0(T\ge t_{\mathrm{obs}})$. The direction should be chosen from the scientific question before examining the data. An upper normal test uses $1-\Phi(z)$; a lower test uses $\Phi(z)$.

## Alternative hypothesis

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

The [alternative hypothesis](#alternative-hypothesis) specifies the parameter values or distributions against which a [null hypothesis](#null-hypothesis) is tested. If the null is $\theta\in\Theta_0$, the alternative is $\theta\in\Theta_1$ with $\Theta_0\cap\Theta_1=\varnothing$. For example an upper one-sided comparison uses $\theta>\theta_0$, while a two-sided comparison uses $\theta\ne\theta_0$. The alternative determines the relevant rejection tail. A [p-value](#p-value) is computed under the null; it is not the probability that the alternative is false.

<h2 id="hotelling-s-t-squared-statistic">Hotelling's T-squared statistic</h2>

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

For independent [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) observations with [positive-definite](bilinear-form.md#positive-definite-bilinear-form) covariance, this statistic is the maximum squared studentized mean contrast. With unbiased [sample covariance matrix](variance.md#sample-covariance-matrix) $S$ and $n>p$, its null distribution obeys $(n-p)T^2/(p(n-1))\sim F_{p,n-p}$. This follows from [independence](random-variable.md#independent-random-variables) of the Gaussian [sample mean](variance.md#sample-mean) and the residual [Wishart distribution](probability-theory.md#wishart-distribution).

<h3 id="affine-invariance-of-hotelling-s-statistic">Affine invariance of Hotelling's statistic</h3>

↑ **Parent:** [Hotelling's T-squared statistic](#hotelling-s-t-squared-statistic)

Under a nonsingular affine transformation $Y=AX+b$, transform the null mean by the same map. Then the centered sample mean becomes $A(\bar X-\mu_0)$ and the [sample covariance matrix](variance.md#sample-covariance-matrix) becomes $ASA^T$. Since $(ASA^T)^{-1}=A^{-T}S^{-1}A^{-1}$, the quadratic form in [Hotelling's T-squared statistic](#hotelling-s-t-squared-statistic) is unchanged. Its value and test decision are consequently invariant under changes of units, origin and nonsingular coordinates.

### Hotelling test of linear hypotheses

↑ **Parent:** [Hotelling's T-squared statistic](#hotelling-s-t-squared-statistic)

For a fixed rank-$m$ constraint matrix $B$, apply [Hotelling's T-squared statistic](#hotelling-s-t-squared-statistic) to the transformed observations $BX_j$. Under $B\mu=0$, $(n-m)T_B^2/(m(n-1))\sim F_{m,n-m}$ for $n>m$. If the displayed contrasts are dependent, use a basis of their row space and replace $m$ by the [rank](quadratic-form.md#rank-one-quadratic-form).

#### Second-difference test of a linear mean profile

↑ **Parent:** [Hotelling test of linear hypotheses](#hotelling-test-of-linear-hypotheses)

At equally spaced distinct times, a mean profile is affine exactly when its consecutive second differences vanish. These form $p-2$ independent contrasts. At unequal times, compare adjacent slopes instead: $(\mu_{i+1}-\mu_i)/(t_{i+1}-t_i)-(\mu_i-\mu_{i-1})/(t_i-t_{i-1})$. A [Hotelling test of linear hypotheses](#hotelling-test-of-linear-hypotheses) tests these restrictions jointly with unknown covariance.

## Rejection region

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A rejection region is the set of sample outcomes on which a [hypothesis test](statistical-hypothesis-test.md) rejects its [null hypothesis](#null-hypothesis). Its probability under the null determines the [Type I error](information-theory.md#type-i-and-type-ii-errors) rate.

<h2 id="mcnemar-s-test">McNemar's test</h2>

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/McNemar's_test)

For paired binary observations $(C_i,M_i)$, let $b$ count pairs $(1,0)$ and $c$ pairs $(0,1)$. Under the [null hypothesis](#null-hypothesis) of equal marginal event probabilities, these discordant outcomes have equal probabilities. Conditional on $b+c$, $b$ has the [binomial distribution](discrete-probability-distribution.md#binomial-distribution) $\operatorname{Bin}(b+c,1/2)$, giving an exact test. For enough discordant pairs, $(b-c)/\sqrt{b+c}$ has an approximate [standard normal distribution](probability-distribution.md#standard-normal-distribution), or its square has an approximate one-degree-of-freedom [chi-squared distribution](probability-distribution.md#chi-squared-distribution). Concordant pairs provide no information about the direction of the marginal difference. If there are no discordant pairs, there is no directional information and the divided statistic is not computed. The pairing and independence between pairs are essential; the usual independent-two-sample formula is not a paired test.

### Equality criterion for paired and unpaired allele tests

↑ **Parent:** [McNemar's test](#mcnemar-s-test)

Let a paired binary table have cells $a,b,c,d$ and $n=a+b+c+d$. The uncorrected [McNemar test](#mcnemar-s-test) is $(b-c)^2/(b+c)$, while the ordinary independent-sample [chi-squared test](statistical-inference.md#chi-squared-test) on the two marginal allele columns is $2n(b-c)^2/[(2a+b+c)(2d+b+c)]$. For nonzero difference and positive denominators, they coincide exactly when $(2a+b+c)(2d+b+c)=2n(b+c)$. Such numerical coincidence does not justify discarding pairing; altering concordant counts can change the unpaired statistic while leaving McNemar's statistic unchanged.

// Target: biology.bigb

### Paired binary sample size calculation

↑ **Parent:** [McNemar's test](#mcnemar-s-test)

For a paired binary difference $D=C-M$, set $\delta=P(C=1)-P(M=1)$ and $q=P(C\ne M)$. Then $\mathbb ED=\delta$ and $\operatorname{Var}(D)=q-\delta^2$. Under equal marginal probabilities the variance is $q$. The [McNemar test](#mcnemar-s-test) has approximate upper rejection boundary $z_{1-\alpha/2}\sqrt{nq}$ for the sum of differences. Requiring that the alternative mean $n\delta$ exceed this boundary by $z_{1-\beta}\sqrt{n(q-\delta^2)}$ gives the displayed planning size for a positive alternative, neglecting its very small lower-tail rejection probability. Use $z_{1-\alpha}$ for a pre-specified one-sided test. The marginal probabilities alone do not determine $q$: co-occurrence of positive outcomes must be specified or bounded. Discreteness and [clustered data](statistical-modelling.md#clustered-data) can change achieved [statistical power](probability-and-statistics.md#statistical-power).

## Significant and nonsignificant results need not differ significantly

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

For independent effect estimates $1.01$ with [standard error](statistical-inference.md#standard-error) $0.50$, and $0.99$ with standard error $0.51$, one two-sided [Wald test](#wald-test) is significant at five percent and the other is not. But their difference is $0.02$ with standard error $\sqrt{0.50^2+0.51^2}\approx0.714$, giving a negligible test statistic. Hence different significance labels do not establish an [interaction](statistical-model.md#interaction-statistics) or [between-study heterogeneity](statistical-inference.md#between-study-heterogeneity); compare the effects directly.

## Monte Carlo test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

Generate independent replicated datasets under a fully specified [null hypothesis](#null-hypothesis) and calculate the same [predictive discrepancy statistic](#predictive-discrepancy-statistic) for them and the observation. Their null exchangeability gives a finite-simulation rank test. The displayed add-one tail probability is valid with conservative treatment of ties, and avoids reporting zero solely because no replicate exceeds the observation.

## Predictive discrepancy statistic

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A measurable summary of a possible dataset is chosen to detect disagreement with a specified predictive model. Compare its observed value with its distribution under replicated datasets. Large-discrepancy statistics can be checked with $\mathbb P(T(X^{\mathrm{rep}})\ge T(x))$. A [posterior predictive check](bayesian-statistics.md#posterior-predictive-check) integrates over posterior parameter uncertainty; a fully specified null instead supplies a fixed reference law.

## Scan statistic

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A scan statistic searches a family of candidate locations or subsets and reports the largest local [statistic](statistical-inference.md#statistic). Under a [null hypothesis](#null-hypothesis), a [union bound](probability-inequality.md#boole-s-inequality) converts a tail estimate for each candidate into a bound for the maximum; no [independence](random-variable.md#independent-random-variables) between local [statistics](statistical-inference.md#statistic) is required. Structured alternatives often permit a [chi-squared testing lower bound](statistical-inference.md#chi-squared-testing-lower-bound) using the overlap geometry of two candidates.

### Cyclic interval overlap bound

↑ **Parent:** [Scan statistic](#scan-statistic)

For independent uniformly placed cyclic intervals of length $k<d$, an overlap is possible at at most $2k-1$ starting-point offsets, or at all $d$ offsets if that number exceeds $d$. Thus the overlap [probability](probability-theory.md#probability) is at most $\min\{1,(2k-1)/d\}$. If $R=|S\cap T|$, then $0\leq R\leq k$ and $\mathbb E(e^{aR/k}-1)\leq(2k/d)(e^a-1)$ for $a\geq0$. The overlap law is not the [hypergeometric distribution](discrete-probability-distribution.md#hypergeometric-distribution) for unrestricted random subsets.

### Quadratic scan statistic

↑ **Parent:** [Scan statistic](#scan-statistic)

A quadratic scan statistic maximizes a directional empirical second moment over candidate unit vectors. For a [Gaussian random vector](probability-and-statistics.md#gaussian-random-vector) sample with a [rank-one covariance spike](variance.md#rank-one-covariance-spike) in one of those directions, the matching statistic has its scale multiplied by the spike's [eigenvalue](linear-operator-theory.md#eigenvalue). A [chi-squared concentration inequality](probability-distribution.md#chi-squared-concentration-inequality) controls each direction.

## Least-favourable null configuration

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A least-favourable configuration maximizes a test procedure’s [Type I error](information-theory.md#type-i-and-type-ii-errors) probability over allowed [null hypothesis](#null-hypothesis) parameters. For one-sided normal comparisons with a fixed [covariance matrix](variance.md#covariance-matrix), coupling by common centered variables shows monotonicity in the means. For the [familywise error rate](#familywise-error-rate), mixed true and false null configurations must also be checked.

## Pearson chi-squared test of homogeneity

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

The Pearson chi-squared test of homogeneity tests whether several independent categorical samples have the same category probabilities. Under the null, expected cell counts equal the product of the corresponding row and column totals divided by the total sample size. The [Pearson chi-squared statistic for contingency tables](#pearson-chi-squared-statistic-for-contingency-tables) $\sum(O-E)^2/E$ has an asymptotic [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $(r-1)(c-1)$ [degrees of freedom](classical-mechanics.md#degree-of-freedom), when expected counts are sufficiently large. The sampling design differs from a [Pearson chi-squared test of independence](#pearson-chi-squared-test-of-independence), though the statistic has the same form.

### Empty groups in a binomial homogeneity test

↑ **Parent:** [Pearson chi-squared test of homogeneity](#pearson-chi-squared-test-of-homogeneity)

For independent $R_i\sim\operatorname{Bin}(n_i,p_i)$, a group with $n_i=0$ necessarily has $R_i=0$ and contributes [likelihood](maximum-likelihood-estimation.md#likelihood-function) one. Its [probability](probability-theory.md#probability) parameter is unidentifiable and supplies no restriction to test. If $k$ groups have positive sample sizes, the unrestricted model has $k$ [probability](probability-theory.md#probability) parameters and the common-probability model has one; the asymptotic homogeneity test therefore has $k-1$ degrees of freedom. Zero expected-count rows must be removed rather than divided by in the Pearson statistic.

### Pearson chi-squared statistic for contingency tables

↑ **Parent:** [Pearson chi-squared test of homogeneity](#pearson-chi-squared-test-of-homogeneity)

For observed counts $O_{ij}$ and positive expected counts $E_{ij}$ in a [contingency table](statistical-modelling.md#contingency-table), the statistic is $X^2=\sum_{ij}(O_{ij}-E_{ij})^2/E_{ij}$. Under common category probabilities or statistical independence, estimate $E_{ij}$ by the product of the row and column totals divided by the grand total. With large expected counts, this gives the test statistic for the [Pearson chi-squared test of homogeneity](#pearson-chi-squared-test-of-homogeneity) or the [Pearson chi-squared test of independence](#pearson-chi-squared-test-of-independence), with asymptotic [chi-squared distribution](probability-distribution.md#chi-squared-distribution) on $(r-1)(c-1)$ [degrees of freedom](classical-mechanics.md#degree-of-freedom).

<h4 id="yates-s-correction-for-continuity">Yates's correction for continuity</h4>

↑ **Parent:** [Pearson chi-squared statistic for contingency tables](#pearson-chi-squared-statistic-for-contingency-tables)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Yates's_correction_for_continuity)

For a two-by-two [contingency table](statistical-modelling.md#contingency-table), subtracting one half from each absolute observed-minus-expected count difference, with truncation at zero, gives the displayed corrected [Pearson chi-squared statistic](generalized-linear-model.md#pearson-chi-squared-statistic). Expected counts use the independence model $E_{ij}=O_{i+}O_{+j}/N$. The subtraction compensates approximately for using a continuous [chi-squared distribution](probability-distribution.md#chi-squared-distribution) for discrete counts. It can make the test conservative. The corrected statistic should be distinguished from the ordinary uncorrected [Pearson chi-squared statistic](generalized-linear-model.md#pearson-chi-squared-statistic).

## Statistical test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A statistical test is a measurable rule for deciding whether to reject a [null hypothesis](#null-hypothesis). Allowing randomisation, it is represented by a function $\varphi(x)\in[0,1]$ giving the conditional rejection [probability](probability-theory.md#probability) after observing $x$. A deterministic test takes only values zero and one. Under a simple null, $E_0\varphi$ is its [size of a statistical test](#size-of-a-statistical-test); under an alternative, $E_1\varphi$ is its [statistical power](probability-and-statistics.md#statistical-power). Randomisation on a [likelihood ratio](#likelihood-ratio) equality set allows a [Neyman-Pearson lemma](#neyman-pearson-lemma) threshold test to attain a prescribed size even for discrete data.

### Most powerful test

↑ **Parent:** [Statistical test](#statistical-test)

At level $\alpha$, a most powerful test against a specified simple alternative maximises [statistical power](probability-and-statistics.md#statistical-power) among [statistical tests](#statistical-test) whose [size of a statistical test](#size-of-a-statistical-test) is at most $\alpha$. The [Neyman-Pearson lemma](#neyman-pearson-lemma) constructs it by a [likelihood ratio](#likelihood-ratio) threshold. A [uniformly most powerful test](#uniformly-most-powerful-test) is most powerful simultaneously against every member of the specified alternative family; maximising power at one alternative alone need not give uniform optimality.

## Test statistic

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Test_statistic)

A test statistic is a measurable function of the sample whose observed value is compared with a null distribution or resampling distribution to decide whether to reject a hypothesis.

<h2 id="student-s-t-test">Student's t-test</h2>

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Student's_t-test)

Student's t-test divides a normally distributed estimated effect by its estimated standard error. Under its null hypothesis the statistic has a [Student's t-distribution](continuous-probability-distribution.md#student-s-t-distribution), with degrees of freedom determined by the variance estimate.

<h3 id="welch-s-t-test">Welch's t-test</h3>

↑ **Parent:** [Student's t-test](#student-s-t-test)

For two [independent](random-variable.md#independent-random-variables) samples from approximately [normal distributions](probability-distribution.md#normal-distribution), [Welch's t-test](#welch-s-t-test) compares their means without assuming equal unknown [variances](variance.md). The displayed [test statistic](#test-statistic) uses sample [variances](variance.md) $s_X^2,s_Y^2$. Under the equal-mean [null hypothesis](#null-hypothesis), its reference [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution) has approximate [statistical degrees of freedom](statistical-inference.md#statistical-degrees-of-freedom)

$$
\nu=\frac{(s_X^2/n_X+s_Y^2/n_Y)^2}{(s_X^2/n_X)^2/(n_X-1)+(s_Y^2/n_Y)^2/(n_Y-1)}.
$$

A [p-value](#p-value) from this approximation addresses the specified statistical error model; it cannot distinguish a material effect from an unmeasured experimenter bias when sample and experimenter are confounded.

### Exact pooled two-sample t statistic

↑ **Parent:** [Student's t-test](#student-s-t-test)

For independent normal samples of sizes $m,n$ with a common unknown [variance](variance.md) and equal means under the null, $Z=(\overline X-\overline Y)/(\sigma\sqrt{1/m+1/n})$ is standard normal. The independent centered sample sums of squares give $V=(m+n-2)S_p^2/\sigma^2\sim\chi^2_{m+n-2}$, independently of $Z$. Thus $Z/\sqrt{V/(m+n-2)}$ has the exact [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution), giving the statistic $(\overline X-\overline Y)/(S_p\sqrt{1/m+1/n})$. A lower one-sided test uses its lower-tail [probability](probability-theory.md#probability).

### Normal-mean likelihood ratio with unknown variance

↑ **Parent:** [Student's t-test](#student-s-t-test)

For an independent sample from a [normal distribution](probability-distribution.md#normal-distribution), maximization of the likelihood over the unknown variance gives the likelihood ratio for a fixed mean against an unrestricted mean as displayed, where $t=\sqrt n(\bar X-\mu_0)/S$ and $S^2=\sum_i(X_i-\bar X)^2/(n-1)$. It decreases with $|t|$. Under the null, the normal sample mean is independent of its centered sum of squares, so $t$ has the exact [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom. The resulting two-sided test requires no asymptotic chi-squared approximation.

### Regression coefficient test power ignores nuisance coefficients

↑ **Parent:** [Student's t-test](#student-s-t-test)

In a fixed full-rank [normal linear model](normal-linear-model.md), the studentized estimator of one coefficient has a [noncentral t-distribution](continuous-probability-distribution.md#noncentral-t-distribution) with noncentrality equal to that coefficient divided by its standard deviation. The fitted and residual [orthogonal projections](hilbert-space.md#orthogonal-projection) of the [Gaussian noise](probability-distribution.md#gaussian-noise) are [independent](random-variable.md#independent-random-variables). Therefore the [statistical power](probability-and-statistics.md#statistical-power) of its exact [Student's t-test](#student-s-t-test) does not depend on the other regression coefficients, with design and variance fixed.

## Fixed alternative

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A fixed alternative keeps a non-null data-generating distribution unchanged as sample size grows. A consistent test rejects with probability tending to one under every fixed alternative in its stated class.

## Local alternative

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A local alternative approaches the null as sample size grows, commonly at distance $n^{-1/2}$. It reveals the nontrivial limiting power of a test near the null.

## Randomization test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A randomization test compares a statistic with values obtained by applying transformations that preserve the joint distribution under the null hypothesis.

### Conditional randomization test

↑ **Parent:** [Randomization test](#randomization-test)

A conditional randomization test resamples a tested variable from its known or estimated conditional distribution given covariates. Under conditional independence from the outcome, the observed and resampled test statistics are exchangeable conditional on those covariates and outcomes.

### Permutation test

↑ **Parent:** [Randomization test](#randomization-test)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permutation_test)

A permutation test uses relabelings of observations as its null-preserving transformations and computes a p-value from the resulting orbit of the test statistic.

### Sign-flip randomization test

↑ **Parent:** [Randomization test](#randomization-test)

A sign-flip randomization test independently multiplies observations by signs in $\{-1,1\}$. It is finite-sample exact for a zero-centered null when the joint distribution is invariant under those sign changes.

## Null hypothesis

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Null_hypothesis)

The null hypothesis is the set of parameter values or probability distributions against which a statistical test controls its probability of rejection.

## Simple hypothesis

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A simple hypothesis specifies one probability distribution completely. A composite hypothesis permits more than one distribution or parameter value.

## Size of a statistical test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

The size of a test is the supremum, over distributions in its [null hypothesis](#null-hypothesis), of its rejection probability. For a simple null it is just the null rejection probability; a level-$\alpha$ test has size at most $\alpha$.

## Significance level

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

The significance level is the chosen upper bound on a test's probability of rejecting the null hypothesis when it is true.

A result is [statistically significant](#statistical-significance) when its calibrated [p-value](#p-value) falls below this chosen threshold.

## P-value

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P-value)

A p-value is the probability, computed under a null hypothesis, of obtaining a test statistic at least as unfavorable to that hypothesis as the observed value.

### Super-uniform random variable

↑ **Parent:** [P-value](#p-value)

A random variable $P\in[0,1]$ is super-uniform when $\mathbb P(P\leq\alpha)\leq\alpha$ for every $\alpha\in[0,1]$. A valid p-value is super-uniform under its null hypothesis.

<h2 id="fisher-s-exact-test">Fisher's exact test</h2>

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fisher's_exact_test)

Fisher's exact test conditions on the margins of a two-by-two contingency table and compares one cell count with its hypergeometric null distribution.

<h3 id="exact-power-of-fisher-s-exact-test">Exact power of Fisher's exact test</h3>

↑ **Parent:** [Fisher's exact test](#fisher-s-exact-test)

For two independent binomial counts, form the [Fisher exact test](#fisher-s-exact-test) rejection region from their conditional null [hypergeometric distribution](discrete-probability-distribution.md#hypergeometric-distribution). Summing alternative joint binomial [probabilities](probability-theory.md#probability) over that region gives its exact power. For equal group sizes, the null allocation is symmetric, so the two-sided [probability](probability-theory.md#probability)-ordering test agrees with doubled lower-tail [probabilities](probability-theory.md#probability). Conservative test discreteness can make a normal-approximation [sample size](probability-and-statistics.md#sample-size) underpowered even when both samples are large but event counts are low.

## Maximin test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A maximin test maximizes the smallest power over a composite alternative subject to controlling the largest rejection probability over a composite null.

## Multiple hypothesis testing

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiple_hypothesis_testing)

Multiple hypothesis testing applies tests to a family of null hypotheses while controlling an aggregate error criterion.

### Intersection hypothesis

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)

For a nonempty finite index set $I$, this hypothesis asserts that every member $H_i$ is true simultaneously. A valid local test must have its stated size under every parameter satisfying the entire intersection. The [Bonferroni correction](#bonferroni-correction) within $I$ always supplies such a test from valid elementary [p-values](#p-value).

#### Closure of a family of statistical hypotheses

↑ **Parent:** [Intersection hypothesis](#intersection-hypothesis)

The closure is the collection of all nonempty [intersection hypotheses](#intersection-hypothesis) from the original elementary family, including singletons. It is not a topological closure. The [closed testing procedure](#closed-testing-procedure) requires local level-$\alpha$ tests for these intersections and rejects an elementary hypothesis only when all intersections containing it reject.

### Hochberg procedure

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)

Order $m$ [p-values](#p-value) and reject the first $r$ hypotheses, where $r=\max\{j:p_{(j)}\le\alpha/(m-j+1)\}$, with $r=0$ for an empty set. Under independent valid true-null [p-values](#p-value), this step-up procedure controls the [familywise error rate](#familywise-error-rate). One proof embeds its rejections in the [closed testing procedure](#closed-testing-procedure) with [Simes tests](#simes-test): every intersection containing a rejected hypothesis passes its local [Simes test](#simes-test), so [closed-testing control of the familywise error rate](#closed-testing-control-of-the-familywise-error-rate) applies.

### Simes inequality

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)

For $m\ge1$ independent valid null [p-values](#p-value), the displayed inequality follows by applying the [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure) with all nulls true. Its [false discovery rate](#false-discovery-rate) then equals the [probability](probability-theory.md#probability) of at least one rejection. Valid means $\Pr(p_i\le t)\le t$ for $0\le t\le1$; independence is a sufficient hypothesis, and arbitrary dependence is not covered by this proof.

#### Simes test

↑ **Parent:** [Simes inequality](#simes-inequality)

For the intersection of $m$ null hypotheses, reject when $\min_i mp_{(i)}/i\le\alpha$. The [Simes inequality](#simes-inequality) establishes a level-$\alpha$ test under independence of valid true-null [p-values](#p-value). The displayed quantity is its combined [p-value](#p-value).

### Weighted interval testing for a piecewise-constant mean

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)

Given valid [p-values](#p-value) $q_J$ for constancy on intervals of length at least two, reject $I$ when $\max_{J\supseteq I}nq_J/|J|\leq\alpha$. Every rejected true interval forces rejection of its maximal constant block. A [union bound](probability-inequality.md#boole-s-inequality) over the non-singleton maximal blocks gives [familywise error rate](#familywise-error-rate) at most $\alpha$, since their lengths sum to at most $n$. Singleton blocks have no tested interval in this formulation.

### Intersection-union test

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)

For a null hypothesis that is a union $H_0=\bigcup_{i\in I}H_i$, an intersection-union test rejects $H_0$ only when every component $H_i$ is rejected. If each component test has level $\alpha$, then under any point of $H_0$ at least one component null is true, so the combined test also has level at most $\alpha$.

### Bonferroni correction

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bonferroni_correction)

The Bonferroni correction tests each of $m$ hypotheses at level $\alpha/m$. The [union bound](probability-inequality.md#boole-s-inequality) then controls the [familywise error rate](#familywise-error-rate) by $\alpha$ under arbitrary dependence.

#### Weighted Bonferroni correction

↑ **Parent:** [Bonferroni correction](#bonferroni-correction)

For positive deterministic weights $w_i$, the weighted Bonferroni correction rejects $H_i$ when

$$
p_i\leq\frac{\alpha w_i}{\sum_jw_j}.
$$

The [union bound](probability-inequality.md#boole-s-inequality) over the true nulls controls the [familywise error rate](#familywise-error-rate) without an independence assumption.

##### Weighted Holm step-down procedure

↑ **Parent:** [Weighted Bonferroni correction](#weighted-bonferroni-correction)

Order $q_i=p_i/w_i$ increasingly. At rank $k$, reject the corresponding hypothesis when

$$
q_{(k)}\leq\frac{\alpha}{\sum_{j=k}^m w_{(j)}}
$$

and otherwise stop. The first ordered true null reduces FWER control to a weighted [union bound](probability-inequality.md#boole-s-inequality); the shrinking denominator makes this procedure at least as powerful as the [Weighted Bonferroni correction](#weighted-bonferroni-correction).

<h4 id="holm-bonferroni-method">Holm–Bonferroni method</h4>

↑ **Parent:** [Bonferroni correction](#bonferroni-correction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holm–Bonferroni_method)

The Holm–Bonferroni method orders p-values and compares the $j$th smallest with $\alpha/(m-j+1)$, stopping at the first failed comparison. It controls the [familywise error rate](#familywise-error-rate) under arbitrary dependence.

##### First true null argument for Holm control

↑ **Parent:** [Holm–Bonferroni method](#holm-bonferroni-method)

If the [Holm step-down procedure](#holm-bonferroni-method) makes a false rejection, it must reject the first true null in the ordered list. All $m_0$ true nulls remain at that step, so its cutoff is at most $\alpha/m_0$. The [union bound](probability-inequality.md#boole-s-inequality) on their marginally valid [p-values](#p-value) gives [familywise error rate](#familywise-error-rate) at most $\alpha$. This proves strong control under arbitrary dependence, and super-uniformity suffices.

### Benjamini-Hochberg procedure

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Benjamini-Hochberg_procedure)

Order $m$ p-values as $p_{(1)}\leq\cdots\leq p_{(m)}$ and take the largest $k$ with $p_{(k)}\leq\alpha k/m$. The Benjamini-Hochberg procedure rejects the hypotheses corresponding to $p_{(1)},\ldots,p_{(k)}$ and controls the [false discovery rate](#false-discovery-rate) under independence and several forms of positive dependence.

#### Benjamini-Hochberg leave-one-out identity

↑ **Parent:** [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure)

Let $R$ be the number of rejections by the [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure) at level $\alpha$, and let $R_i$ be the rejection count after replacing $p_i$ by zero. Then $R_i\ge1$ and

$$
\frac{\mathbf1\{i\text{ rejected}\}}{R\vee1}=\frac{\mathbf1\{p_i\le\alpha R_i/m\}}{R_i}.
$$

If $i$ was rejected, lowering its [p-value](#p-value) does not change any ordered [p-value](#p-value) beyond rank $R$, so $R_i=R$. Conversely, if $p_i\le\alpha R_i/m$, the other $R_i-1$ rejected values together with $p_i$ satisfy the original threshold; monotonicity gives $R=R_i$. For a valid true-null [p-value](#p-value) independent of the others, conditioning on $R_i$ bounds the expectation of the right side by $\alpha/m$. Summing over true nulls proves [false discovery rate](#false-discovery-rate) at most $m_0\alpha/m$.

##### Benjamini-Hochberg leave-two-out identity

↑ **Parent:** [Benjamini-Hochberg leave-one-out identity](#benjamini-hochberg-leave-one-out-identity)

Replace two [p-values](#p-value) $P_i,P_j$ by zeros in the [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure) at level $\alpha$, keeping the original denominator $m$, and let $R^{(ij)}$ be the resulting rejection count. Equivalently, remove the two values and apply the step-up critical values $\alpha(k+2)/m$ to the remaining ordered [p-values](#p-value); their rejection count is $R_{-ij}=R^{(ij)}-2$. For $r\ge2$,

$$
\{P_i\le\alpha r/m,\ P_j\le\alpha r/m,\ R=r\}
=\{P_i\le\alpha r/m,\ P_j\le\alpha r/m,\ R^{(ij)}=r\}.
$$

If both original values are rejected, lowering them changes no ordered rank greater than $r$, so the rejection count stays $r$. Conversely, if the modified count is $r$ and both original values meet the rank-$r$ threshold, reinserting them leaves at least $r$ qualifying values. Monotonicity under lowering gives at most $r$ original rejections. This identity is deterministic and does not require [independence](random-variable.md#independent-random-variables) or a distributional assumption.

###### Second moment of the Benjamini-Hochberg false discovery proportion

↑ **Parent:** [Benjamini-Hochberg leave-two-out identity](#benjamini-hochberg-leave-two-out-identity)

For independent [p-values](#p-value), with $m_0$ true-null values independent and uniform on $[0,1]$, let $R^{(i)}$ denote the [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure) rejection count after replacing one true-null value by zero. The [Benjamini-Hochberg leave-one-out identity](#benjamini-hochberg-leave-one-out-identity) gives

$$
\mathbb E\frac{\mathbf1\{i\text{ rejected}\}}{(R\vee1)^2}=\frac\alpha m\mathbb E\frac1{R^{(i)}}.
$$

For distinct true-null indices, the [Benjamini-Hochberg leave-two-out identity](#benjamini-hochberg-leave-two-out-identity) gives

$$
\mathbb E\frac{\mathbf1\{i,j\text{ rejected}\}}{(R\vee1)^2}=\frac{\alpha^2}{m^2}.
$$

Indeed, conditional on the remaining values and $R^{(ij)}=r$, the two independent uniform values both meet their threshold with probability $(\alpha r/m)^2$, cancelling the denominator $r^2$. Expanding the square of the false rejection count into its diagonal terms and ordered distinct pairs, and using symmetry among the true-null values, proves

$$
\mathbb E(\operatorname{FDP}^2)=\frac{\alpha m_0}{m}\mathbb E\frac1{R^{(i)}}+\frac{\alpha^2m_0(m_0-1)}{m^2}.
$$

If no null is true, both sides are zero; if exactly one is true, the pair contribution is absent. This formula complements the exact [false discovery rate](#false-discovery-rate) $\alpha m_0/m$ by describing second-moment variability.

##### Exact false discovery rate under independent null p-values

↑ **Parent:** [Benjamini-Hochberg leave-one-out identity](#benjamini-hochberg-leave-one-out-identity)

For the [Benjamini-Hochberg procedure](#benjamini-hochberg-procedure), replace a true-null [p-value](#p-value) $P_i$ by zero and call the new rejection count $R^{(i)}$. The [Benjamini-Hochberg leave-one-out identity](#benjamini-hochberg-leave-one-out-identity) identifies rejection with $R=r$ with the event $P_i\leq\alpha r/m$ and $R^{(i)}=r$. If $P_i$ is uniform and independent of all the other [p-values](#p-value), each possible rejection count contributes $\alpha\mathbb P(R^{(i)}=r)/m$ to its expected false-discovery fraction. Summation gives $\alpha/m$ per true null and the displayed exact [false discovery rate](#false-discovery-rate). Super-uniform independent nulls yield the corresponding upper bound.

### False discovery rate

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/False_discovery_rate)

The false discovery rate is $\mathbb E[V/(R\vee1)]$, where $V$ is the number of rejected true null hypotheses and $R$ is the total number of rejections.

#### False discovery proportion

↑ **Parent:** [False discovery rate](#false-discovery-rate)

In [multiple hypothesis testing](#multiple-hypothesis-testing), let $R$ count all rejections and $V$ count rejected true [null hypotheses](#null-hypothesis). The false discovery proportion is the random variable $V/(R\vee1)$, defined to be zero when $R=0$. Its expectation is the [false discovery rate](#false-discovery-rate). Distinguishing the realized proportion from its expectation matters: controlling the [false discovery rate](#false-discovery-rate) does not by itself give a high-probability bound on the realized proportion.

### Familywise error rate

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Familywise_error_rate)

The familywise error rate is the probability of making at least one false rejection in a family of hypothesis tests.

#### Familywise error control for a laminar hypothesis family

↑ **Parent:** [Familywise error rate](#familywise-error-rate)

For nonempty index sets forming a [laminar family of sets](extremal-set-theory.md#laminar-family-of-sets), reject an [intersection hypothesis](#intersection-hypothesis) when the displayed adjusted value is at most $\alpha$. The inclusion-maximal true sets are disjoint and have total size at most $m$. Any false rejection forces some maximal true $J$ to have $p_J\leq\alpha|J|/m$. Validity and the [union bound](probability-inequality.md#boole-s-inequality) control the [familywise error rate](#familywise-error-rate) by $\alpha$, without independence or a complete closure.

### Closed testing procedure

↑ **Parent:** [Multiple hypothesis testing](#multiple-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_testing_procedure)

Choose a level-$\alpha$ local test for every nonempty intersection $H_I=\bigcap_{i\in I}H_i$. The closed testing procedure rejects an elementary hypothesis $H_i$ exactly when every intersection hypothesis containing it is rejected by its local test.

#### Closed-testing control of the familywise error rate

↑ **Parent:** [Closed testing procedure](#closed-testing-procedure)

If any true elementary hypothesis is rejected by a [closed testing procedure](#closed-testing-procedure), then the intersection of all true null hypotheses must also be rejected. Its local test has level $\alpha$, so the [familywise error rate](#familywise-error-rate) is at most $\alpha$ under arbitrary dependence.

## Joint hypothesis test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

A joint hypothesis test imposes several parameter restrictions simultaneously and accounts for dependence among their estimators; separate one-parameter confidence intervals do not generally determine its result.

## Power function of a statistical test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

For a test with rejection region $R$, its power function is

$$
\pi(\theta)=\mathbb P_\theta(X\in R).
$$

Its supremum over the null parameter space is the size of the test.

## Uniformly most powerful test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniformly_most_powerful_test)

A level-$\alpha$ test is uniformly most powerful when its power is at least that of every other level-$\alpha$ test at every parameter value in the alternative.

### Crossing-power obstruction to a uniformly most powerful test

↑ **Parent:** [Uniformly most powerful test](#uniformly-most-powerful-test)

If two tests have the same size and each has strictly greater power than the other at some alternative, neither test is uniformly most powerful.

<h2 id="pearson-s-chi-squared-test">Pearson's chi-squared test</h2>

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pearson's_chi-squared_test)

The Pearson chi-squared test compares observed categorical counts with null expected counts using the displayed statistic. Its applications include [Pearson chi-squared goodness-of-fit test](#pearson-chi-squared-goodness-of-fit-test) for specified probabilities and [Pearson chi-squared test of independence](#pearson-chi-squared-test-of-independence) for contingency tables; the fitted restrictions determine the limiting degrees of freedom.

### Pearson chi-squared goodness-of-fit test

↑ **Parent:** [Pearson's chi-squared test](#pearson-s-chi-squared-test)

For observed cell counts $O_j$ and null expected counts $E_j$, the statistic is

$$
X^2=\sum_j\frac{(O_j-E_j)^2}{E_j}.
$$

With $k$ specified null cell probabilities and sufficiently large expected counts, its null limit is $\chi^2_{k-1}$.

#### Binomial goodness-of-fit with an estimated parameter

↑ **Parent:** [Pearson chi-squared goodness-of-fit test](#pearson-chi-squared-goodness-of-fit-test)

For $N$ independent groups each containing $m$ independent [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial) with common probability $\theta$, the group count has a [binomial distribution](discrete-probability-distribution.md#binomial-distribution). If $O_j$ groups have count $j$, the [maximum-likelihood estimate](maximum-likelihood-estimation.md#maximum-likelihood-estimator) is $\widehat\theta=\sum_jjO_j/(mN)$. Form the [Pearson chi-squared statistic](generalized-linear-model.md#pearson-chi-squared-statistic) using $E_j=N\binom mj\widehat\theta^j(1-\widehat\theta)^{m-j}$. With all $m+1$ categories retained, an interior true parameter, and sufficiently large expected counts, its null limit is a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $m-1$ [statistical degrees of freedom](statistical-inference.md#statistical-degrees-of-freedom): one degree is removed by the fixed total and another by fitting $\theta$. Small expected counts require care with this approximation. If categories are pooled, the fitted parameter and calibration should correspond to the pooled statistical model; simply pooling a statistic after fitting the unpooled model does not automatically give the usual chi-squared limit.

#### Pearson chi-squared test of independence

↑ **Parent:** [Pearson chi-squared goodness-of-fit test](#pearson-chi-squared-goodness-of-fit-test)

For an $r$ by $c$ contingency table, the statistic

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}
$$

has asymptotically a chi-squared distribution with $(r-1)(c-1)$ degrees of freedom under independence.

## Likelihood-ratio test of independence in a contingency table

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

For observed counts $y_{ij}$ and fitted counts $\widehat\mu_{ij}=y_{i+}y_{+j}/y_{++}$ under independence, the likelihood-ratio statistic is

$$
G^2=2\sum_{i,j:y_{ij}>0}y_{ij}\log\frac{y_{ij}}{\widehat\mu_{ij}}.
$$

Under independence and standard large-sample regularity conditions, $G^2$ converges in distribution to $\chi^2_{(r-1)(c-1)}$.

### Aggregation can change a contingency-table independence test

↑ **Parent:** [Likelihood-ratio test of independence in a contingency table](#likelihood-ratio-test-of-independence-in-a-contingency-table)

Combining levels of a [categorical variable](statistical-modelling.md#categorical-variable) changes both the null hypothesis and the degrees of freedom of an independence test. Association that is coherent across the combined levels may become easier to detect because the grouped table has fewer degrees of freedom, while associations that cancel within groups may disappear. Conclusions from the original and aggregated tables therefore need not agree.

## Linear-by-linear association test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)

For a two-way [contingency table](statistical-modelling.md#contingency-table) whose row and column variables are [ordinal categorical variables](statistical-modelling.md#ordinal-categorical-variable), assign row scores $u_i$ and column scores $v_j$. The linear-by-linear association statistic measures the weighted covariance

$$
\sum_{i,j}y_{ij}(u_i-\bar u)(v_j-\bar v).
$$

After normalization, its square is asymptotically $\chi^2_1$ under independence. A signed, one-sided version tests a specified direction of ordinal association and can have greater [statistical power](probability-and-statistics.md#statistical-power) than an omnibus independence test against a monotone alternative.

## Wald test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wald_test)

For an approximately normal estimator, the one-parameter Wald statistic

$$
Z=\frac{\widehat\theta-\theta_0}{\operatorname{se}(\widehat\theta)}
$$

is approximately standard normal under $H_0:\theta=\theta_0$. A two-sided test reports $2\Phi(-|Z|)$.

### Signed normal Wald statistic

↑ **Parent:** [Wald test](#wald-test)

For an independent normal sample with known standard deviation $\sigma$, the signed [Wald statistic](#wald-test) for testing mean zero is $W=\sqrt n\bar Y/\sigma$. It has the [standard normal distribution](probability-distribution.md#standard-normal-distribution) under the [null hypothesis](#null-hypothesis) and distribution $N(\sqrt n\delta/\sigma,1)$ under mean $\delta$. Its square has a [chi-squared distribution](probability-distribution.md#chi-squared-distribution); retaining the sign permits a one-sided test.

### Wald statistics with a shared control

↑ **Parent:** [Wald test](#wald-test)

Independent normal arm means with variances $v_0,v_1,v_2$ give treatment-contrast [Wald test](#wald-test) statistics whose [correlation coefficient](variance.md#pearson-correlation-coefficient) is $v_0/\sqrt{(v_0+v_1)(v_0+v_2)}$. The common control mean creates positive dependence between comparisons.

### Multivariate Wald statistic

↑ **Parent:** [Wald test](#wald-test)

For a regular $p$-parameter model, the Wald statistic for a candidate $\theta$ is

$$
W_n(\theta)
=n(\widehat\theta_n-\theta)^T
I(\widehat\theta_n)
(\widehat\theta_n-\theta).
$$

Under the true parameter it converges in distribution to $\chi_p^2$.

#### Wald statistic for linear restrictions

↑ **Parent:** [Multivariate Wald statistic](#multivariate-wald-statistic)

For a full-row-rank $k\times p$ matrix $R$ and the null hypothesis $R\theta=r$, put

$$
W_{n,R}=n(R\widehat\theta_n-r)^T
\left[R I(\widehat\theta_n)^{-1}R^T\right]^{-1}
(R\widehat\theta_n-r).
$$

Under the null, asymptotic normality and [Slutsky theorem](statistical-inference.md#slutsky-theorem) give $W_{n,R}\xrightarrow d\chi_k^2$.

### Wald and likelihood-ratio asymptotic equivalence

↑ **Parent:** [Wald test](#wald-test)

In a regular scalar model under the null, Taylor expansion about the MLE gives

$$
2\{\ell_n(\widehat\theta)-\ell_n(\theta_0)\}
=-\ell_n''(\widetilde\theta)(\widehat\theta-\theta_0)^2.
$$

A uniform law of large numbers for the observed information makes  
$-\ell_n''(\widetilde\theta)/n$ and the Fisher information used in the Wald statistic converge to the same positive limit. Their ratio therefore converges in probability to one.

### Two-sided Gaussian p-value

↑ **Parent:** [Wald test](#wald-test)

For $\overline X\sim N(\mu,1/n)$ under $H_0:\mu=0$, the two-sided level-$\alpha$ test rejects when $|\sqrt n\,\overline X|>\Phi^{-1}(1-\alpha/2)$, and the observed p-value is

$$
p(\overline x)=2[1-\Phi(\sqrt n|\overline x|)].
$$

## Likelihood-ratio test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Likelihood-ratio_test)

A likelihood-ratio test rejects where the alternative likelihood is sufficiently large relative to the null likelihood.

### Gaussian covariance diagonality likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For independent observations from a nonsingular [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) with unknown mean, let $S=n^{-1}\sum_i(y_i-\bar y)(y_i-\bar y)^T$. The unrestricted [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator) of covariance is $S$, while the diagonal restriction gives $D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. The fitted trace terms both equal $p$, so twice the log-likelihood difference is $W=n\log(\det D/\det S)=-n\log\det R$, where $R$ is the [sample correlation matrix](variance.md#sample-correlation-matrix). Under the diagonal null hypothesis and fixed dimension, the [Wilks theorem](statistical-inference.md#wilks-theorem) gives $W\Rightarrow\chi^2_{p(p-1)/2}$.

### Gaussian diagonal-covariance likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For independent [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) observations with unrestricted [mean](expected-value.md) and positive-definite [sample covariance matrix](variance.md#sample-covariance-matrix) $S=n^{-1}\sum_i(x_i-\bar x)(x_i-\bar x)^T$, the unrestricted [maximum-likelihood estimates](maximum-likelihood-estimation.md#maximum-likelihood-estimator) are $\bar x,S$. Requiring a diagonal population [covariance matrix](variance.md#covariance-matrix) gives the same mean and covariance estimate $D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. Both fitted quadratic terms equal $np$, so their likelihood quotient is $(|S|/|D|)^{n/2}=|R|^{n/2}$, where $R=D^{-1/2}SD^{-1/2}$ is the [sample correlation matrix](variance.md#sample-correlation-matrix). Small determinants give evidence against diagonality. For two variables this is a two-sided test of their [sample correlation](variance.md#sample-correlation-coefficient).

### One-sided likelihood-ratio test for two normal variances

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For independent samples from [normal distributions](probability-distribution.md#normal-distribution) with separate unknown means, test equal variances against $\sigma_X^2>\sigma_Y^2$. Profiling the means gives sample means. Under the null the variance maximum is $(S_X+S_Y)/(n_X+n_Y)$; the separate maxima are $S_X/n_X$ and $S_Y/n_Y$. If the latter obey the proposed order, their likelihood quotient is

$$
\Lambda=\frac{(S_X/n_X)^{n_X/2}(S_Y/n_Y)^{n_Y/2}}{[(S_X+S_Y)/(n_X+n_Y)]^{(n_X+n_Y)/2}}.
$$

It decreases strictly as $(S_X/n_X)/(S_Y/n_Y)>1$ increases. Otherwise the ordered alternative maximum lies on the equal-variance boundary and the quotient is one. Under the null, [Cochran's theorem](normal-linear-model.md#cochran-s-theorem) gives independent chi-squared residual sums with degrees $n_X-1,n_Y-1$, so rejection is in the upper tail of the displayed [F-distribution](continuous-probability-distribution.md#f-distribution) statistic, calibrated at the desired significance level.

### Boundary likelihood-ratio test for two Gaussian means

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For independent unit-variance Gaussian samples with means $\mu_X,\mu_Y$, testing $\mu_X\geq A,\mu_Y=0$ against unrestricted means gives $T=-2\log\Lambda=n[\bar Y^2+(A-\bar X)_+^2]$. The unrestricted [maximum-likelihood estimators](maximum-likelihood-estimation.md#maximum-likelihood-estimator) are the two [sample means](variance.md#sample-mean), while the null estimators are $\max(A,\bar X)$ and zero. Under the null, write $W=\sqrt n(\bar X-A)=W_0+\delta$, $\delta=\sqrt n(\mu_X-A)\geq0$, and $Z=\sqrt n\bar Y$, with $W_0,Z$ independent standard Gaussian variables. Then $T=Z^2+(-W_0-\delta)_+^2$ decreases pointwise with $\delta$, so the largest rejection probability occurs at the boundary $\mu_X=A$. There its law is the [chi-bar-squared distribution](probability-distribution.md#chi-bar-squared-distribution) $\tfrac12\chi_1^2+\tfrac12\chi_2^2$. The exact size-$\alpha$ threshold $c_\alpha$ is therefore determined by $1-\Phi(\sqrt{c_\alpha})+\tfrac12e^{-c_\alpha/2}=\alpha$.

### Single-parameter boundary likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For a scalar parameter restricted to $\psi\ge0$, test $\psi=0$ against $\psi>0$ with identifiable interior [nuisance parameters](statistical-model.md#nuisance-parameter). A locally quadratic regular likelihood has an efficient null score $Z\sim N(0,1)$, and the constrained fit projects the unconstrained local maximizer onto the nonnegative half-line. Consequently

$$
2(\ell_{\rm full}-\ell_{\rm null})\Rightarrow(\max(0,Z))^2
\sim\tfrac12\delta_0+\tfrac12\chi^2_1.
$$

For a positive statistic, its asymptotic upper-tail [p-value](#p-value) is half the ordinary one-degree chi-squared tail. Its 5% critical value is the 90th chi-squared percentile, approximately 2.7055. Additional boundary [nuisance parameters](statistical-model.md#nuisance-parameter) or nonidentified mixture parameters can change this law.

### Variance-component likelihood-ratio test at a boundary

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

Testing a single nonnegative random-effect variance against zero puts the null on the boundary of the parameter space. In the usual regular increasing-independent-groups limit, the [likelihood-ratio test statistic](#likelihood-ratio-test-statistic) has limit $\tfrac12\delta_0+\tfrac12\chi_1^2$, rather than $\chi_1^2$. A finite-sample simulation calibrated for the actual design avoids relying on this asymptotic approximation.

#### Location-scale invariant simulation test for a Gaussian variance component

↑ **Parent:** [Variance-component likelihood-ratio test at a boundary](#variance-component-likelihood-ratio-test-at-a-boundary)

With fixed $X,Z$, compare $N(X\beta,\sigma^2I)$ and $N(X\beta,\sigma^2I+\tau^2ZZ^T)$ by maximizing the ordinary [likelihood function](maximum-likelihood-estimation.md#likelihood-function) in both models. Their [likelihood-ratio test statistic](#likelihood-ratio-test-statistic) is unchanged by $Y\mapsto Xb+cY$, $c>0$, because both maximized log-likelihoods change by the same $-n\log c$. Its null law can therefore be simulated using independent $N(0,I)$ responses. Comparing the observed statistic with simulated statistics by $(1+\#\{T_b\geq T_{obs}\})/(B+1)$ gives a conservative finite-sample Monte Carlo p-value, subject to correctly maximizing both likelihoods.

### Likelihood ratio

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For two parameter values $\theta_1$ and $\theta_0$, the likelihood ratio is $f(x\mid\theta_1)/f(x\mid\theta_0)$.

#### Log-likelihood ratio

↑ **Parent:** [Likelihood ratio](#likelihood-ratio)

A [log-likelihood ratio](#log-likelihood-ratio) compares two [likelihoods](maximum-likelihood-estimation.md#likelihood-function) on an additive scale. For independent observations its increments add. Under distributions $P_0,P_1$ with suitable integrability and common support, $E_0[\log(dP_1/dP_0)]=-D(P_0\Vert P_1)\le0$ and $E_1[\log(dP_1/dP_0)]=D(P_1\Vert P_0)\ge0$, where $D$ is [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence). This sign change motivates likelihood-based sequential monitoring.

### Likelihood-ratio test statistic

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

For nested null and alternative parameter spaces, the likelihood-ratio test statistic is

$$
-2\log\Lambda
=2\left\{\sup_{\theta\in\Theta_1}\ell(\theta)
-\sup_{\theta\in\Theta_0}\ell(\theta)\right\}.
$$

Under the regularity conditions of [Wilks theorem](statistical-inference.md#wilks-theorem), its null limit is a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) whose degrees of freedom equal the difference in model dimensions.

#### Bartlett correction

↑ **Parent:** [Likelihood-ratio test statistic](#likelihood-ratio-test-statistic)

A Bartlett correction rescales a regular [likelihood-ratio test statistic](#likelihood-ratio-test-statistic) so that its null expected value matches its limiting chi-squared degrees of freedom to a higher asymptotic order. If $\mathbb E_0W=d(1+b/n+O(n^{-2}))$, divide $W$ by $1+b/n$. The operation uses a model-specific [Bartlett correction coefficient](#bartlett-correction-coefficient); matching the mean alone is not a general proof of any claimed distributional error rate.

##### Bartlett-corrected likelihood-ratio statistic

↑ **Parent:** [Bartlett correction](#bartlett-correction)

If $\mathbb E_0W=d(1+b/n+O(n^{-2}))$, the Bartlett-corrected statistic has mean $d+O(n^{-2})$. It is commonly calibrated against a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $d$ degrees of freedom. Equivalently, to the displayed order, one may multiply $W$ by $1-b/n$.

##### Bartlett correction coefficient

↑ **Parent:** [Bartlett correction](#bartlett-correction)

The coefficient $b$ is the leading relative null-mean discrepancy of a regular [likelihood-ratio test statistic](#likelihood-ratio-test-statistic). It is distinct from the finite-sample divisor $1+b/n$ used in a [Bartlett correction](#bartlett-correction). Different conventions call either of these a correction factor, so the normalization should always be stated explicitly.

###### Bartlett correction for a normal variance with unknown mean

↑ **Parent:** [Bartlett correction coefficient](#bartlett-correction-coefficient)

For a sample of size $n\geq2$ from a [normal distribution](probability-distribution.md#normal-distribution) with unknown mean, the null variance [likelihood-ratio test statistic](#likelihood-ratio-test-statistic) is $W=n[-\log(U/n)+U/n-1]$, where $U\sim\chi^2_{n-1}$. With $V=(U-n)/n$, its expected Taylor terms start with $n[\mathbb EV^2/2-\mathbb EV^3/3+\mathbb EV^4/4]$. Here $\mathbb EV^2=(2n-1)/n^2$, $\mathbb EV^3=(2n-3)/n^3$, and $\mathbb EV^4=(12n^2+4n-15)/n^4$. Higher fixed-order terms contribute only $O(n^{-2})$ under valid termwise asymptotic integration. Thus $\mathbb E_0W=1+11/(6n)+O(n^{-2})$ and $W_B=W/[1+11/(6n)]$.

### Generalized likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](#likelihood-ratio-test)

A generalized likelihood-ratio test compares the likelihood maximized under the null with the likelihood maximized over the full parameter space.

#### Likelihood-ratio test of area-proportional Poisson means

↑ **Parent:** [Generalized likelihood-ratio test](#generalized-likelihood-ratio-test)

Two equally numerous groups of independent counts with [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) have areas $a$ and $2a$. Under common density their group means are in ratio $1:2$. With group sums $S_1,S_2$ and $T=S_1+S_2$, the maximized alternative-to-null likelihood ratio is

$$
\Lambda=(3S_1/T)^{S_1}(3S_2/(2T))^{S_2}.
$$

Use zero-count limits and $\Lambda=1$ when $T=0$. The regular [Wilks theorem](statistical-inference.md#wilks-theorem) calibration has one degree of freedom. Exactly conditioning on $T$ gives $S_1\sim\operatorname{Binomial}(T,1/3)$ under the null; this supports small-count testing without the large-sample approximation.

#### Analysis of deviance for nested generalized linear models

↑ **Parent:** [Generalized likelihood-ratio test](#generalized-likelihood-ratio-test)

The deviance of a fitted generalized linear model is

$$
D=2\{\ell_{\mathrm{sat}}-\ell_{\mathrm{fit}}\}.
$$

For regular nested models, the deviance reduction $D_0-D_1=2(\ell_1-\ell_0)$ is asymptotically chi-squared with degrees of freedom equal to the difference in fitted dimensions.

##### Residual deviance

↑ **Parent:** [Analysis of deviance for nested generalized linear models](#analysis-of-deviance-for-nested-generalized-linear-models)

The unscaled residual deviance of an [exponential dispersion family](exponential-family.md#exponential-dispersion-model) compares its fitted mean with the [saturated statistical model](statistical-modelling.md#saturated-statistical-model) at a common [dispersion parameter](exponential-family.md#dispersion-parameter). Its normalization removes the factor $1/\phi$ in the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood). In [Poisson regression](generalized-linear-model.md#poisson-regression) and [binomial regression](generalized-linear-model.md#binomial-regression), $\phi=1$, so it is twice the saturated-minus-fitted [log-likelihood](maximum-likelihood-estimation.md#log-likelihood). Under suitable regularity, $D/\phi$ has approximately a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with the [residual degrees of freedom](statistical-modelling.md#residual-degrees-of-freedom); this is not an automatic accurate approximation for sparse responses. Nested deviance reductions with estimated dispersion lead to approximate [F-tests](probability-and-statistics.md#f-test) after scaling by the dispersion estimate.

###### Null deviance

↑ **Parent:** [Residual deviance](#residual-deviance)

The [null deviance](#null-deviance) is the unscaled [deviance](exponential-family.md#exponential-family-deviance) of the intercept-only mean model relative to the saturated model at a common [dispersion parameter](exponential-family.md#dispersion-parameter) $\phi$, retaining any known [generalized linear model offset](generalized-linear-model.md#generalized-linear-model-offset). It supplies a baseline against which predictor terms improve the fit. Its difference from a fitted model's [residual deviance](#residual-deviance), divided by $\phi$, is the statistic for a [likelihood-ratio test](#likelihood-ratio-test) of those added terms, with nuisance parameters handled consistently in both fits. In Poisson and binomial families, $\phi=1$.

#### Likelihood-ratio test for equality of two normal means

↑ **Parent:** [Generalized likelihood-ratio test](#generalized-likelihood-ratio-test)

For independent unit-variance samples, testing equal means uses $Z=\sqrt{mn/(m+n)}(\bar X-\bar Y)$ and rejects for large $|Z|$.

#### Nested likelihood-ratio rejection regions

↑ **Parent:** [Generalized likelihood-ratio test](#generalized-likelihood-ratio-test)

Likelihood-ratio tests of different null subspaces can have crossing rejection regions; comparing their quadratic-form geometry exhibits observations accepted by one and rejected by another.

## Score test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Score_test)

The score test evaluates the likelihood gradient at the restricted estimator and scales its quadratic form by inverse Fisher information.

### Restricted maximum-likelihood estimator

↑ **Parent:** [Score test](#score-test)

A restricted maximum-likelihood estimator maximizes likelihood over the null parameter space rather than the full model.

### Score test under a simple null

↑ **Parent:** [Score test](#score-test)

Under a regular simple $p$-parameter null, the normalized score converges to $N_p(0,I_1)$, so its information-standardized squared norm converges to $\chi_p^2$.

#### Quadratic form of a standard normal vector

↑ **Parent:** [Score test under a simple null](#score-test-under-a-simple-null)

If $Z\sim N_p(0,I_p)$, then $Z^TZ=\sum_{j=1}^pZ_j^2\sim\chi_p^2$.

### Residual sum of squares in a normal sample

↑ **Parent:** [Score test](#score-test)

For independent $N(\mu,\sigma^2)$ observations, $\sum_i(X_i-\bar X)^2/\sigma^2$ has the $\chi_{n-1}^2$ distribution.

#### Chi-square central limit theorem

↑ **Parent:** [Residual sum of squares in a normal sample](#residual-sum-of-squares-in-a-normal-sample)

If $Q_m\sim\chi_m^2$, then $(Q_m-m)/\sqrt{2m}$ converges in distribution to $N(0,1)$.

## Neyman-Pearson lemma

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neyman-Pearson_lemma)

For testing one simple hypothesis against another, a test that rejects for sufficiently large likelihood ratio has greatest power among all tests of no greater size.

### Most powerful test for a Laplace location shift

↑ **Parent:** [Neyman-Pearson lemma](#neyman-pearson-lemma)

For two unit-scale [Laplace distributions](continuous-probability-distribution.md#laplace-distribution) with locations $\theta_0<\theta_1$, the [likelihood ratio](#likelihood-ratio) is nondecreasing in $X$, with constant tails and an increasing middle interval. Therefore an upper-tail [statistical test](#statistical-test) of exact [size of a statistical test](#size-of-a-statistical-test) $\alpha$ is a [most powerful test](#most-powerful-test). Its cutoff is $c_\alpha=\theta_0-\log(2\alpha)$ for $\alpha\leq1/2$, and $c_\alpha=\theta_0+\log(2(1-\alpha))$ otherwise. Under location $\theta_1$, its [statistical power](probability-and-statistics.md#statistical-power) is $\tfrac12e^{\theta_1-c_\alpha}$ if $c_\alpha\geq\theta_1$, and $1-\tfrac12e^{c_\alpha-\theta_1}$ otherwise. Constant [likelihood ratio](#likelihood-ratio) tails can make the [most powerful test](#most-powerful-test) nonunique.

### Minimum sum of errors in a simple hypothesis test

↑ **Parent:** [Neyman-Pearson lemma](#neyman-pearson-lemma)

For two [simple hypotheses](#simple-hypothesis) with [probability densities](wave-function.md#probability-density) $f_0,f_1$, a [critical region](#rejection-region) $C$ has sum of [Type I error](information-theory.md#type-i-and-type-ii-errors) and [Type II error](information-theory.md#type-i-and-type-ii-errors) probabilities $\int_Cf_0+\int_{C^c}f_1$. Pointwise minimization chooses $C=\{f_1>f_0\}$, with either decision allowed on the equality set. Thus the optimal [likelihood ratio](#likelihood-ratio) threshold is $1$, and the minimum is $\int\min(f_0,f_1)=1-\tfrac12\int|f_1-f_0|$. This criterion weights the two error probabilities equally; unequal costs or prior probabilities change the threshold.

### Exponential-rate likelihood-ratio test

↑ **Parent:** [Neyman-Pearson lemma](#neyman-pearson-lemma)

For independent [exponential distribution](continuous-probability-distribution.md#exponential-distribution) observations with rate $\lambda$, the likelihood ratio for a larger simple rate is decreasing in their sum. The [Neyman-Pearson lemma](#neyman-pearson-lemma) therefore selects a lower-tail sum threshold $c$. The sum has a [gamma distribution](continuous-probability-distribution.md#gamma-distribution), giving the displayed power; its derivative is $c e^{-\lambda c}(\lambda c)^{n-1}/(n-1)!>0$. Calibrating at $\lambda_0$ gives size $\alpha$ for the composite null $\lambda\le\lambda_0$ and a uniformly most powerful test against larger rates.

### Uniformly most powerful test for an exponential rate

↑ **Parent:** [Neyman-Pearson lemma](#neyman-pearson-lemma)

For independent samples from an [exponential distribution](continuous-probability-distribution.md#exponential-distribution), a test of rate at most $\lambda_0$ against rate greater than $\lambda_0$ rejects for small sample sums. All simple-alternative [likelihood ratios](#likelihood-ratio) against $\lambda_0$ decrease with that sum; its [gamma distribution](continuous-probability-distribution.md#gamma-distribution) calibrates the size at $\lambda_0$. Monotonicity of the rejection probability in the rate proves that this is a [uniformly most powerful test](#uniformly-most-powerful-test) for the composite hypotheses.

### Monotone likelihood ratio

↑ **Parent:** [Neyman-Pearson lemma](#neyman-pearson-lemma)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monotone_likelihood_ratio)

A one-parameter family has a monotone likelihood ratio in a statistic $T$ when $f(x\mid\theta_1)/f(x\mid\theta_0)$ is nondecreasing in $T(x)$ whenever $\theta_1>\theta_0$.

#### Posterior odds are monotone under a monotone likelihood ratio

↑ **Parent:** [Monotone likelihood ratio](#monotone-likelihood-ratio)

For a family with a [monotone likelihood ratio](#monotone-likelihood-ratio) in $T$, a prior density $\pi$ and cutoff $a$, the posterior odds of $\theta>a$ against $\theta\le a$ are nondecreasing in $T$. To prove it, write the unnormalized masses as $A(t)$ and $B(t)$. For $t_2>t_1$, the difference $A(t_2)B(t_1)-A(t_1)B(t_2)$ is the double integral over $\theta>a\ge\eta$ of $\pi(\theta)\pi(\eta)[f_\theta(t_2)f_\eta(t_1)-f_\theta(t_1)f_\eta(t_2)]$. Each integrand is nonnegative by the likelihood-ratio ordering. Common factors in the full-data likelihood cancel from the odds, so the same argument works when $T$ is a statistic rather than the complete observation. Interpret zero denominators by extended odds whenever the posterior is defined.

#### Monotone test

↑ **Parent:** [Monotone likelihood ratio](#monotone-likelihood-ratio)

An upper-tail monotone test in a real statistic $T$ has rejection probability $\phi=\mathbf1_{T>c}+\eta\mathbf1_{T=c}$, with $0\le\eta\le1$; the constant tests correspond to infinite cutoffs. For a family with positive densities on a common support and a [monotone likelihood ratio](#monotone-likelihood-ratio) in $T$, its [power function](#power-function-of-a-statistical-test) can cross that of an arbitrary competing test only from below to above as the parameter increases. If $r=f_{\theta_1}/f_{\theta_0}$ and $\theta_1>\theta_0$, choose a positive number $k$ between the ratios on opposite sides of the cutoff. The signs of $\phi-\phi'$ and $r-k$ agree away from $T=c$, and $r=k$ at a boundary with positive mass. Therefore $E_{\theta_1}(\phi-\phi')\ge kE_{\theta_0}(\phi-\phi')$. In particular strict positivity at $\theta_0$ propagates to $\theta_1$. Positivity of the densities matters for this strict conclusion; with changing supports only a weak conclusion may remain.

#### Karlin-Rubin theorem

↑ **Parent:** [Monotone likelihood ratio](#monotone-likelihood-ratio)

For a family with a [monotone likelihood ratio](#monotone-likelihood-ratio) in $T$, a level-$\alpha$ upper-tail test in $T$ is a [uniformly most powerful test](#uniformly-most-powerful-test) for the corresponding one-sided hypothesis.

##### Uniformly most powerful upper-tail test for a logistic location

↑ **Parent:** [Karlin-Rubin theorem](#karlin-rubin-theorem)

For one observation from the [logistic distribution](statistical-modelling.md#logistic-distribution), the size-$\alpha$ test of $H_0:\theta\leq0$ against $H_1:\theta>0$ rejects when

$$
X>\log\frac{1-\alpha}{\alpha}.
$$

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Chernoff information](information-theory.md#chernoff-information)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-5.md#section-1/1/m/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#8h/solution)
