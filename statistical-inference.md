# Statistical inference

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_inference)

[Statistical inference](statistical-inference.md) uses observed data and a [statistical model](statistical-model.md) to learn about unknown features of the process that generated them. In a [parametric statistical model](statistical-model.md#parametric-statistical-model), write $X\sim P_\theta$: the [probability distribution](probability-distribution.md) depends on an unknown [statistical parameter](statistical-model.md#statistical-parameter) $\theta$. An [estimand](#estimand) specifies the target, such as a [mean](expected-value.md) or a difference of [means](expected-value.md). A [statistic](#statistic) is a function of the observations; an [estimator](statistical-modelling.md#estimator) is a [statistic](#statistic) used to estimate the target. Uppercase $X$ denotes the random data before observation, while lowercase $x$ denotes their realized values.

Three questions lead to different outputs. [Statistical estimation](#statistical-estimation) asks which target value the observations suggest. A [confidence interval](#confidence-interval) asks for a range produced by a procedure with calibrated [coverage probability](#coverage-probability). A [hypothesis test](statistical-hypothesis-test.md) asks whether the observations depart sufficiently from a specified [null hypothesis](statistical-hypothesis-test.md#null-hypothesis) to enter its [rejection region](statistical-hypothesis-test.md#rejection-region). These outputs complement one another: an estimated [effect size](#effect-size) describes magnitude, while a [standard error](#standard-error) describes the [sampling distribution](statistical-modelling.md#sampling-distribution) of an [estimator](statistical-modelling.md#estimator). A [p-value](statistical-hypothesis-test.md#p-value) describes a tail [probability](probability-theory.md#probability) under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis).

The appeal of [statistical inference](statistical-inference.md) is that it turns variable observations into reproducible uncertainty statements. In the [normal mean confidence interval with known variance](#normal-mean-confidence-interval-with-known-variance) below, a [sample mean](variance.md#sample-mean) of $1.2$ has [standard error](#standard-error) $0.5$: both the estimated shift and its precision matter. The calibration depends on the [statistical model](statistical-model.md), including [independence](random-variable.md#independent-random-variables) and the specified [probability distribution](probability-distribution.md). Increasing [sample size](probability-and-statistics.md#sample-size) improves precision under those assumptions; it does not repair a systematically misleading sampling procedure. [Bayesian inference](bayesian-statistics.md) provides another framework, using a [prior distribution](bayesian-statistics.md#prior-probability) and a [likelihood function](maximum-likelihood-estimation.md#likelihood-function) to obtain a [posterior distribution](bayesian-statistics.md#bayesian-posterior).

**Table of contents**

- [Blind analysis](#blind-analysis)
- [Pseudolikelihood](#pseudolikelihood)
- [Winner's curse](#winner-s-curse)
- [Frequency estimation](#frequency-estimation)
- [Effect size](#effect-size)
- [Statistical process control](#statistical-process-control)
  - [CUSUM](#cusum)
    - [Poisson likelihood-ratio CUSUM](#poisson-likelihood-ratio-cusum)
    - [Average run length](#average-run-length)
    - [Fast initial response CUSUM](#fast-initial-response-cusum)
  - [Hospital mortality funnel plot](#hospital-mortality-funnel-plot)
    - [Binomial funnel control limits](#binomial-funnel-control-limits)
  - [Control limits](#control-limits)
- [Jackknife resampling](#jackknife-resampling)
  - [Jackknife variance estimator](#jackknife-variance-estimator)
    - [Jackknife and bootstrap variance of a sample second moment](#jackknife-and-bootstrap-variance-of-a-sample-second-moment)
- [Fisherian conditional inference](#fisherian-conditional-inference)
  - [Conditionality principle](#conditionality-principle)
- [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test)
  - [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic)
  - [Lilliefors test](#lilliefors-test)
  - [Two-sample Kolmogorov-Smirnov test](#two-sample-kolmogorov-smirnov-test)
- [Likelihood principle](#likelihood-principle)
  - [Exponential sampling stopped by a data-dependent coin](#exponential-sampling-stopped-by-a-data-dependent-coin)
- [Estimand](#estimand)
- [Efficiency (statistics)](#efficiency-statistics)
- [Statistical functional](#statistical-functional)
  - [Functional statistic](#functional-statistic)
  - [Density fourth-power functional](#density-fourth-power-functional)
    - [Spike obstruction to density-power differentiability](#spike-obstruction-to-density-power-differentiability)
  - [Pathwise differentiability of a statistical functional](#pathwise-differentiability-of-a-statistical-functional)
    - [Influence-function representer](#influence-function-representer)
      - [Canonical gradient](#canonical-gradient)
- [Statistical estimation](#statistical-estimation)
  - [Ratio estimator](#ratio-estimator)
    - [Absolute error bound for a ratio estimator with a controlled denominator](#absolute-error-bound-for-a-ratio-estimator-with-a-controlled-denominator)
- [Probability sampling](#probability-sampling)
  - [Sampling with replacement](#sampling-with-replacement)
  - [Inclusion probability](#inclusion-probability)
  - [Unequal probability sampling](#unequal-probability-sampling)
  - [Finite population mean](#finite-population-mean)
  - [Finite population variance](#finite-population-variance)
  - [Sampling without replacement](#sampling-without-replacement)
    - [Marginal and pair probabilities in sampling without replacement](#marginal-and-pair-probabilities-in-sampling-without-replacement)
    - [First return to equal counts in sampling without replacement](#first-return-to-equal-counts-in-sampling-without-replacement)
    - [First marked item in a random permutation](#first-marked-item-in-a-random-permutation)
  - [Cluster sampling](#cluster-sampling)
    - [Design effect](#design-effect)
  - [Stratified sampling](#stratified-sampling)
    - [Optimal cost-constrained stratified sampling allocation](#optimal-cost-constrained-stratified-sampling-allocation)
  - [Simple random sampling](#simple-random-sampling)
    - [Sample mean under simple random sampling](#sample-mean-under-simple-random-sampling)
      - [Sampling fraction](#sampling-fraction)
- [Scoring rule](#scoring-rule)
  - [Linear probability score](#linear-probability-score)
  - [Proper scoring rule](#proper-scoring-rule)
    - [Strictly proper scoring rule](#strictly-proper-scoring-rule)
      - [Brier score](#brier-score)
      - [Logarithmic scoring rule](#logarithmic-scoring-rule)
        - [Prequential log score identity](#prequential-log-score-identity)
- [Statistical degrees of freedom](#statistical-degrees-of-freedom)
- [Statistic](#statistic)
  - [Complete statistic](#complete-statistic)
    - [Boundedly complete statistic](#boundedly-complete-statistic)
- [Meta-analysis](#meta-analysis)
  - [Subgroup analysis in meta-analysis](#subgroup-analysis-in-meta-analysis)
  - [Forest plot](#forest-plot)
  - [Funnel plot](#funnel-plot)
    - [Small-study effect](#small-study-effect)
  - [Publication bias](#publication-bias)
    - [Selection model for publication bias](#selection-model-for-publication-bias)
      - [Odds under at-least-one-positive selection](#odds-under-at-least-one-positive-selection)
    - [Trim and fill](#trim-and-fill)
  - [Independent subgroup contrast in meta-analysis](#independent-subgroup-contrast-in-meta-analysis)
  - [Within-study bias](#within-study-bias)
    - [Bias-adjusted meta-analysis](#bias-adjusted-meta-analysis)
  - [Fixed-effect meta-analysis](#fixed-effect-meta-analysis)
    - [Mantel–Haenszel pooled odds ratio](#mantel-haenszel-pooled-odds-ratio)
  - [Leave-one-study-out influence analysis](#leave-one-study-out-influence-analysis)
  - [Random-effects meta-analysis](#random-effects-meta-analysis)
    - [Student t random-effect model](#student-t-random-effect-model)
    - [Between-study heterogeneity](#between-study-heterogeneity)
      - [Meta-regression](#meta-regression)
      - [Prior calibration for normal random-effect range](#prior-calibration-for-normal-random-effect-range)
      - [I-squared statistic](#i-squared-statistic)
      - [DerSimonian–Laird estimator](#dersimonian-laird-estimator)
      - [Cochran's Q statistic](#cochran-s-q-statistic)
  - [Network meta-analysis](#network-meta-analysis)
    - [Indirect treatment comparison](#indirect-treatment-comparison)
      - [Transitivity in network meta-analysis](#transitivity-in-network-meta-analysis)
- [Confidence region](#confidence-region)
  - [Confidence band](#confidence-band)
    - [Kolmogorov-Smirnov confidence band](#kolmogorov-smirnov-confidence-band)
  - [Confidence ellipsoid](#confidence-ellipsoid)
- [Statistical sample](#statistical-sample)
  - [Normal sample](#normal-sample)
- [Semiparametric statistics](#semiparametric-statistics)
  - [Adaptivity to an unknown covariate distribution](#adaptivity-to-an-unknown-covariate-distribution)
  - [Nuisance tangent space](#nuisance-tangent-space)
    - [Mean-preserving error tangent space](#mean-preserving-error-tangent-space)
    - [Efficient score](#efficient-score)
      - [Efficient score in independent-error regression](#efficient-score-in-independent-error-regression)
      - [Efficient-score projection identity](#efficient-score-projection-identity)
      - [Efficient information](#efficient-information)
  - [Semiparametric estimator](#semiparametric-estimator)
  - [Partially linear model](#partially-linear-model)
- [Fisher consistency](#fisher-consistency)
- [Scale estimator](#scale-estimator)
- [Consistency (statistics)](#consistency-statistics)
- [Plug-in estimator](#plug-in-estimator)
- [Assouad's lemma](#assouad-s-lemma)
  - [Assouad hypercube](#assouad-hypercube)
- [Nonparametric statistics](nonparametric-statistics.md)
  - [Rank test](nonparametric-statistics.md#rank-test)
  - [Wilcoxon signed-rank test](nonparametric-statistics.md#wilcoxon-signed-rank-test)
    - [Walsh average](nonparametric-statistics.md#walsh-average)
    - [Wilcoxon signed-rank statistic](nonparametric-statistics.md#wilcoxon-signed-rank-statistic)
  - [Mann–Whitney U test](nonparametric-statistics.md#mann-whitney-u-test)
    - [Normal approximation for a rank sum](nonparametric-statistics.md#normal-approximation-for-a-rank-sum)
    - [Exact null distribution of a rank sum](nonparametric-statistics.md#exact-null-distribution-of-a-rank-sum)
      - [Exact rank-sum tail one above the minimum](nonparametric-statistics.md#exact-rank-sum-tail-one-above-the-minimum)
  - [Fourier deconvolution](nonparametric-statistics.md#fourier-deconvolution)
  - [Empirical likelihood](nonparametric-statistics.md#empirical-likelihood)
    - [Empirical likelihood with mixed censoring](nonparametric-statistics.md#empirical-likelihood-with-mixed-censoring)
      - [Likelihood support reduction under censoring](nonparametric-statistics.md#likelihood-support-reduction-under-censoring)
      - [Monotonicity bound for a mixed-censoring likelihood](nonparametric-statistics.md#monotonicity-bound-for-a-mixed-censoring-likelihood)
  - [Nonparametric maximum-likelihood estimator](nonparametric-statistics.md#nonparametric-maximum-likelihood-estimator)
  - [Density estimation](nonparametric-statistics.md#density-estimation)
    - [Haar density estimator](nonparametric-statistics.md#haar-density-estimator)
    - [Quadratic density derivative functional](nonparametric-statistics.md#quadratic-density-derivative-functional)
      - [Diagonal correction for a quadratic density derivative estimate](nonparametric-statistics.md#diagonal-correction-for-a-quadratic-density-derivative-estimate)
    - [Nearest neighbour density estimation](nonparametric-statistics.md#nearest-neighbour-density-estimation)
    - [Kernel for density estimation](nonparametric-statistics.md#kernel-for-density-estimation)
      - [Triweight kernel](nonparametric-statistics.md#triweight-kernel)
        - [Triweight density minimizes integrated squared curvature](nonparametric-statistics.md#triweight-density-minimizes-integrated-squared-curvature)
      - [Gaussian density kernel](nonparametric-statistics.md#gaussian-density-kernel)
      - [Epanechnikov kernel](nonparametric-statistics.md#epanechnikov-kernel)
        - [Optimality of the Epanechnikov kernel](nonparametric-statistics.md#optimality-of-the-epanechnikov-kernel)
      - [Flat-top kernel for density estimation](nonparametric-statistics.md#flat-top-kernel-for-density-estimation)
        - [Parametric-rate kernel estimation of a bandlimited density](nonparametric-statistics.md#parametric-rate-kernel-estimation-of-a-bandlimited-density)
      - [Kernel of order ell](nonparametric-statistics.md#kernel-of-order-ell)
        - [Legendre polynomial kernel construction](nonparametric-statistics.md#legendre-polynomial-kernel-construction)
      - [Kernel density estimation](nonparametric-statistics.md#kernel-density-estimation)
        - [Gaussian kernel density worked example](nonparametric-statistics.md#gaussian-kernel-density-worked-example)
        - [History of kernel density estimation](nonparametric-statistics.md#history-of-kernel-density-estimation)
        - [Exact mean integrated squared error of a kernel density estimator](nonparametric-statistics.md#exact-mean-integrated-squared-error-of-a-kernel-density-estimator)
        - [Pointwise optimal kernel bandwidth](nonparametric-statistics.md#pointwise-optimal-kernel-bandwidth)
          - [Normal-density local-to-global bandwidth ratio](nonparametric-statistics.md#normal-density-local-to-global-bandwidth-ratio)
        - [Canonical kernel for density estimation](nonparametric-statistics.md#canonical-kernel-for-density-estimation)
        - [Pointwise central limit theorem for a kernel density estimator](nonparametric-statistics.md#pointwise-central-limit-theorem-for-a-kernel-density-estimator)
        - [Third-order pointwise kernel error bound](nonparametric-statistics.md#third-order-pointwise-kernel-error-bound)
        - [Integrated variance of a kernel density estimator](nonparametric-statistics.md#integrated-variance-of-a-kernel-density-estimator)
          - [Gaussian autoregressive kernel variance correction](nonparametric-statistics.md#gaussian-autoregressive-kernel-variance-correction)
        - [Pointwise minimax rate for Hölder density estimation](nonparametric-statistics.md#pointwise-minimax-rate-for-holder-density-estimation)
        - [Bias of a kernel density estimator](nonparametric-statistics.md#bias-of-a-kernel-density-estimator)
          - [Boundary bias of a kernel density estimator](nonparametric-statistics.md#boundary-bias-of-a-kernel-density-estimator)
          - [Integrated second-order kernel bias bound](nonparametric-statistics.md#integrated-second-order-kernel-bias-bound)
          - [Integrated squared bias from a density jump](nonparametric-statistics.md#integrated-squared-bias-from-a-density-jump)
            - [Box-kernel bias of a piecewise constant density](nonparametric-statistics.md#box-kernel-bias-of-a-piecewise-constant-density)
          - [Second-order pointwise bias bound for kernel density estimation](nonparametric-statistics.md#second-order-pointwise-bias-bound-for-kernel-density-estimation)
        - [Lepski bandwidth selection method](nonparametric-statistics.md#lepski-bandwidth-selection-method)
        - [Derivative kernel density estimator](nonparametric-statistics.md#derivative-kernel-density-estimator)
          - [Second derivative kernel density estimator](nonparametric-statistics.md#second-derivative-kernel-density-estimator)
            - [Integrated squared density curvature](nonparametric-statistics.md#integrated-squared-density-curvature)
              - [Scale-invariant density curvature](nonparametric-statistics.md#scale-invariant-density-curvature)
          - [Nikolsky class](nonparametric-statistics.md#nikolsky-class)
          - [MISE rate for derivative kernel density estimation](nonparametric-statistics.md#mise-rate-for-derivative-kernel-density-estimation)
  - [Nonparametric regression](nonparametric-statistics.md#nonparametric-regression)
    - [Random-design nonparametric regression](nonparametric-statistics.md#random-design-nonparametric-regression)
    - [Smoothing parameter](nonparametric-statistics.md#smoothing-parameter)
    - [Smoothing spline](nonparametric-statistics.md#smoothing-spline)
      - [Quadratic smoothing spline for interval averages](nonparametric-statistics.md#quadratic-smoothing-spline-for-interval-averages)
      - [Cubic smoothing spline](nonparametric-statistics.md#cubic-smoothing-spline)
        - [Roughness-matrix formula for a natural cubic smoothing spline](nonparametric-statistics.md#roughness-matrix-formula-for-a-natural-cubic-smoothing-spline)
    - [Fixed-design nonparametric regression](nonparametric-statistics.md#fixed-design-nonparametric-regression)
      - [Wavelet regression estimator](nonparametric-statistics.md#wavelet-regression-estimator)
        - [Wavelet coefficient thresholding](nonparametric-statistics.md#wavelet-coefficient-thresholding)
          - [Simultaneous wavelet coefficient noise bound](nonparametric-statistics.md#simultaneous-wavelet-coefficient-noise-bound)
      - [Window occupancy for an equally spaced regression design](nonparametric-statistics.md#window-occupancy-for-an-equally-spaced-regression-design)
      - [Pointwise minimax rate for Lipschitz regression](nonparametric-statistics.md#pointwise-minimax-rate-for-lipschitz-regression)
    - [Linear estimator in nonparametric regression](nonparametric-statistics.md#linear-estimator-in-nonparametric-regression)
      - [Smoothing matrix](nonparametric-statistics.md#smoothing-matrix)
    - [Kernel regression](nonparametric-statistics.md#kernel-regression)
    - [Local polynomial regression](nonparametric-statistics.md#local-polynomial-regression)
      - [Mean absolute error bound for local polynomial regression](nonparametric-statistics.md#mean-absolute-error-bound-for-local-polynomial-regression)
      - [Local linear regression](nonparametric-statistics.md#local-linear-regression)
      - [Kernel for nonparametric regression](nonparametric-statistics.md#kernel-for-nonparametric-regression)
        - [Smoothing bandwidth](nonparametric-statistics.md#smoothing-bandwidth)
          - [Plug-in bandwidth selection](nonparametric-statistics.md#plug-in-bandwidth-selection)
            - [Fourth-derivative pilot estimate of density curvature](nonparametric-statistics.md#fourth-derivative-pilot-estimate-of-density-curvature)
        - [Uniform smoothing kernel](nonparametric-statistics.md#uniform-smoothing-kernel)
          - [Unit-width box kernel](nonparametric-statistics.md#unit-width-box-kernel)
      - [Local polynomial Gram matrix](nonparametric-statistics.md#local-polynomial-gram-matrix)
      - [Effective kernel weight](nonparametric-statistics.md#effective-kernel-weight)
      - [Polynomial reproduction property of local polynomial regression](nonparametric-statistics.md#polynomial-reproduction-property-of-local-polynomial-regression)
      - [Local polynomial derivative estimator](nonparametric-statistics.md#local-polynomial-derivative-estimator)
      - [Nadaraya–Watson estimator](nonparametric-statistics.md#nadaraya-watson-estimator)
        - [Interior absolute-error rate of the Nadaraya-Watson estimator](nonparametric-statistics.md#interior-absolute-error-rate-of-the-nadaraya-watson-estimator)
        - [Boundary bias of local constant regression](nonparametric-statistics.md#boundary-bias-of-local-constant-regression)
          - [Second-order boundary expansion for local constant regression](nonparametric-statistics.md#second-order-boundary-expansion-for-local-constant-regression)
        - [Mean absolute error of local constant regression](nonparametric-statistics.md#mean-absolute-error-of-local-constant-regression)
        - [Interior first-order bias cancellation for local constant regression](nonparametric-statistics.md#interior-first-order-bias-cancellation-for-local-constant-regression)
    - [Isotonic regression](nonparametric-statistics.md#isotonic-regression)
      - [Pool adjacent violators algorithm](nonparametric-statistics.md#pool-adjacent-violators-algorithm)
      - [Minimax rate for isotonic sequence estimation](nonparametric-statistics.md#minimax-rate-for-isotonic-sequence-estimation)
- [Robust statistics](robust-statistics.md)
  - [Translation-invariant estimator](robust-statistics.md#translation-invariant-estimator)
  - [Minimax asymptotic bias](robust-statistics.md#minimax-asymptotic-bias)
  - [Trimmed mean](robust-statistics.md#trimmed-mean)
    - [Influence function of a trimmed mean](robust-statistics.md#influence-function-of-a-trimmed-mean)
  - [M-estimator](robust-statistics.md#m-estimator)
    - [Sandwich variance of an M-estimator](robust-statistics.md#sandwich-variance-of-an-m-estimator)
    - [Argmin consistency under uniform convergence in probability](robust-statistics.md#argmin-consistency-under-uniform-convergence-in-probability)
      - [Global argmin may escape a compact convergence set](robust-statistics.md#global-argmin-may-escape-a-compact-convergence-set)
    - [Scale M-estimator](robust-statistics.md#scale-m-estimator)
  - [Catoni mean estimator](robust-statistics.md#catoni-mean-estimator)
  - [B-robust estimator](robust-statistics.md#b-robust-estimator)
  - [Contamination (statistics)](robust-statistics.md#contamination-statistics)
    - [Kolmogorov neighborhood of a distribution](robust-statistics.md#kolmogorov-neighborhood-of-a-distribution)
    - [Epsilon-contamination neighborhood](robust-statistics.md#epsilon-contamination-neighborhood)
      - [Huber contamination](robust-statistics.md#huber-contamination)
  - [Influence function](robust-statistics.md#influence-function)
    - [Influence function of the mean](robust-statistics.md#influence-function-of-the-mean)
    - [Influence function of a Huber location estimator](robust-statistics.md#influence-function-of-a-huber-location-estimator)
    - [Normal-location influence curves](robust-statistics.md#normal-location-influence-curves)
    - [Finite contamination bias of normal location](robust-statistics.md#finite-contamination-bias-of-normal-location)
    - [Local influence versus replacement breakdown](robust-statistics.md#local-influence-versus-replacement-breakdown)
    - [Rejection point of an influence function](robust-statistics.md#rejection-point-of-an-influence-function)
    - [Local-shift sensitivity](robust-statistics.md#local-shift-sensitivity)
    - [Influence function of a quantile](robust-statistics.md#influence-function-of-a-quantile)
    - [Empirical influence function](robust-statistics.md#empirical-influence-function)
    - [Sensitivity curve](robust-statistics.md#sensitivity-curve)
    - [One-step estimator](robust-statistics.md#one-step-estimator)
    - [Asymptotic linear representation](robust-statistics.md#asymptotic-linear-representation)
    - [Gross-error sensitivity](robust-statistics.md#gross-error-sensitivity)
    - [Influence function of the sample median](robust-statistics.md#influence-function-of-the-sample-median)
  - [Breakdown point](robust-statistics.md#breakdown-point)
    - [Finite-sample maximum bias](robust-statistics.md#finite-sample-maximum-bias)
    - [Replacement breakdown point](robust-statistics.md#replacement-breakdown-point)
  - [Huber location estimator](robust-statistics.md#huber-location-estimator)
    - [Huber location response to one outlier](robust-statistics.md#huber-location-response-to-one-outlier)
    - [Huber score](robust-statistics.md#huber-score)
      - [Optimal bounded influence function for normal location](robust-statistics.md#optimal-bounded-influence-function-for-normal-location)
    - [Huber loss](robust-statistics.md#huber-loss)
      - [Huber gradient regularizer](robust-statistics.md#huber-gradient-regularizer)
  - [Median-of-means estimator](robust-statistics.md#median-of-means-estimator)
  - [Tukey median](robust-statistics.md#tukey-median)
  - [Asymptotic distribution of a sample median](robust-statistics.md#asymptotic-distribution-of-a-sample-median)
- [Kolmogorov-Smirnov theorem](#kolmogorov-smirnov-theorem)
- [Standard error](#standard-error)
- [Efficient unbiased estimator implies exponential family](#efficient-unbiased-estimator-implies-exponential-family)
- [Wilks theorem](#wilks-theorem)
- [Chi-squared test](#chi-squared-test)
  - [Chi-squared comparison of a calibrated attenuation model](#chi-squared-comparison-of-a-calibrated-attenuation-model)
  - [Compatibility of independent lifetime measurements](#compatibility-of-independent-lifetime-measurements)
  - [Chi-squared test of independence](#chi-squared-test-of-independence)
- [Statistical decision theory](#statistical-decision-theory)
  - [Statistical invariance principle](#statistical-invariance-principle)
  - [Cost-effectiveness analysis](#cost-effectiveness-analysis)
    - [Incremental net monetary benefit](#incremental-net-monetary-benefit)
      - [Cost-effectiveness acceptability curve](#cost-effectiveness-acceptability-curve)
    - [Cost-effectiveness plane](#cost-effectiveness-plane)
    - [Incremental cost-effectiveness ratio](#incremental-cost-effectiveness-ratio)
  - [Bayesian decision problem](#bayesian-decision-problem)
  - [Decision rule](#decision-rule)
  - [Absolute-error loss](#absolute-error-loss)
    - [Asymmetric absolute-error loss](#asymmetric-absolute-error-loss)
      - [Bayes quantile under asymmetric absolute-error loss](#bayes-quantile-under-asymmetric-absolute-error-loss)
  - [Squared-error loss](#squared-error-loss)
    - [Quadratic risk](#quadratic-risk)
      - [Mean-vector prediction risk](#mean-vector-prediction-risk)
        - [Unbiased Gaussian projection risk estimate](#unbiased-gaussian-projection-risk-estimate)
          - [Unknown-variance risk estimation in a saturated Gaussian model](#unknown-variance-risk-estimation-in-a-saturated-gaussian-model)
  - [Le Cam two-point lemma](#le-cam-two-point-lemma)
    - [Metric two-point risk bound](#metric-two-point-risk-bound)
    - [Metric squared-loss two-point bound](#metric-squared-loss-two-point-bound)
      - [Mean-estimation minimax lower bound for continuous densities](#mean-estimation-minimax-lower-bound-for-continuous-densities)
    - [Chi-squared testing lower bound](#chi-squared-testing-lower-bound)
    - [Le Cam lower bound under absolute-error loss](#le-cam-lower-bound-under-absolute-error-loss)
      - [Gaussian location minimax lower bound under absolute-error loss](#gaussian-location-minimax-lower-bound-under-absolute-error-loss)
    - [Two-point lower bound with a triangular bump](#two-point-lower-bound-with-a-triangular-bump)
  - [Bayes classifier](#bayes-classifier)
    - [Cost-sensitive Bayes classifier](#cost-sensitive-bayes-classifier)
    - [Minimum-integral decision region](#minimum-integral-decision-region)
    - [Gaussian Bayes classifier](#gaussian-bayes-classifier)
      - [Prior-dependent Gaussian discriminant boundary](#prior-dependent-gaussian-discriminant-boundary)
      - [Equal-covariance Gaussian classification error](#equal-covariance-gaussian-classification-error)
    - [Uniqueness of a Bayes classifier](#uniqueness-of-a-bayes-classifier)
  - [Risk of a decision rule](#risk-of-a-decision-rule)
  - [Bayes risk](#bayes-risk)
    - [Bayes act](#bayes-act)
      - [Highest density region](#highest-density-region)
    - [Least favorable prior](#least-favorable-prior)
  - [Minimax decision rule](#minimax-decision-rule)
    - [Alpha-beta pruning](#alpha-beta-pruning)
    - [Equalizer rule](#equalizer-rule)
      - [Minimax Gaussian Bayes classifier from equal class errors](#minimax-gaussian-bayes-classifier-from-equal-class-errors)
    - [Constant-risk limit-of-Bayes-risk criterion](#constant-risk-limit-of-bayes-risk-criterion)
    - [Minimax sample mean for a nonnegative normal location](#minimax-sample-mean-for-a-nonnegative-normal-location)
- [Confidence interval](#confidence-interval)
  - [Normal mean confidence interval with known variance](#normal-mean-confidence-interval-with-known-variance)
    - [Normal mean confidence interval and hypothesis test duality](#normal-mean-confidence-interval-and-hypothesis-test-duality)
  - [Coverage probability](#coverage-probability)
  - [Extreme-order-statistic tolerance interval](#extreme-order-statistic-tolerance-interval)
  - [Exponential-mean confidence interval by pivot inversion](#exponential-mean-confidence-interval-by-pivot-inversion)
  - [Fieller's theorem](#fieller-s-theorem)
  - [Confidence bound](#confidence-bound)
  - [Likelihood-ratio confidence interval](#likelihood-ratio-confidence-interval)
  - [Confidence interval for a reciprocal rate](#confidence-interval-for-a-reciprocal-rate)
  - [Order-statistic confidence interval for a median](#order-statistic-confidence-interval-for-a-median)
  - [Support-restricted confidence interval for a uniform location parameter](#support-restricted-confidence-interval-for-a-uniform-location-parameter)
- [Prediction interval](#prediction-interval)
  - [Normal prediction interval with maximum-likelihood variance](#normal-prediction-interval-with-maximum-likelihood-variance)
  - [Prediction interval in a normal linear model](#prediction-interval-in-a-normal-linear-model)
    - [Zero-residual degeneracy of regression prediction](#zero-residual-degeneracy-of-regression-prediction)
  - [Prediction interval for a ratio of log-normal responses](#prediction-interval-for-a-ratio-of-log-normal-responses)
- [Student t confidence interval](#student-t-confidence-interval)
  - [Confidence interval for the difference of independent regression slopes](#confidence-interval-for-the-difference-of-independent-regression-slopes)
  - [Student t confidence interval for a centered regression intercept](#student-t-confidence-interval-for-a-centered-regression-intercept)
- [Bayesian statistics](bayesian-statistics.md)
  - [Selection conditioning in Bayesian inference](bayesian-statistics.md#selection-conditioning-in-bayesian-inference)
  - [Likelihood reconstruction from posterior simulation](bayesian-statistics.md#likelihood-reconstruction-from-posterior-simulation)
  - [BUGS](bayesian-statistics.md#bugs)
    - [Zeros trick](bayesian-statistics.md#zeros-trick)
  - [Variational inference](bayesian-statistics.md#variational-inference)
    - [Reparameterization gradient](bayesian-statistics.md#reparameterization-gradient)
    - [Markov chain variational inference](bayesian-statistics.md#markov-chain-variational-inference)
    - [Mean-field variational inference](bayesian-statistics.md#mean-field-variational-inference)
  - [Data augmentation](bayesian-statistics.md#data-augmentation)
  - [Hierarchical Bayesian model](bayesian-statistics.md#hierarchical-bayesian-model)
    - [Conditional exchangeability of hospital risks](bayesian-statistics.md#conditional-exchangeability-of-hospital-risks)
    - [Non-centered Gaussian random-effect parameterization](bayesian-statistics.md#non-centered-gaussian-random-effect-parameterization)
    - [Partial pooling](bayesian-statistics.md#partial-pooling)
    - [Gamma–Poisson hierarchical model](bayesian-statistics.md#gamma-poisson-hierarchical-model)
      - [Poisson–exponential posterior shrinkage formula](bayesian-statistics.md#poisson-exponential-posterior-shrinkage-formula)
      - [Gamma-integrated baseline Poisson likelihood](bayesian-statistics.md#gamma-integrated-baseline-poisson-likelihood)
    - [Gaussian–exponential hierarchical colour model](bayesian-statistics.md#gaussian-exponential-hierarchical-colour-model)
  - [Maximum a posteriori estimation](bayesian-statistics.md#maximum-a-posteriori-estimation)
    - [Maximum a posteriori estimate](bayesian-statistics.md#maximum-a-posteriori-estimate)
  - [Credible interval](bayesian-statistics.md#credible-interval)
    - [Equal-tailed credible interval](bayesian-statistics.md#equal-tailed-credible-interval)
    - [One-sided credible interval](bayesian-statistics.md#one-sided-credible-interval)
  - [Empirical Bayes method](bayesian-statistics.md#empirical-bayes-method)
    - [Maximum marginal likelihood estimator](bayesian-statistics.md#maximum-marginal-likelihood-estimator)
    - [Hyperparameter](bayesian-statistics.md#hyperparameter)
  - [Dirichlet process](bayesian-statistics.md#dirichlet-process)
    - [Dirichlet-multinomial conjugacy](bayesian-statistics.md#dirichlet-multinomial-conjugacy)
  - [Prior probability](bayesian-statistics.md#prior-probability)
    - [Prior mean](bayesian-statistics.md#prior-mean)
    - [Prior elicitation](bayesian-statistics.md#prior-elicitation)
    - [Prior odds](bayesian-statistics.md#prior-odds)
    - [Prior density](bayesian-statistics.md#prior-density)
    - [Continuous spike-and-slab prior](bayesian-statistics.md#continuous-spike-and-slab-prior)
    - [Uniform prior](bayesian-statistics.md#uniform-prior)
  - [Bayesian posterior](bayesian-statistics.md#bayesian-posterior)
    - [Normal mean posterior with an exponential prior](bayesian-statistics.md#normal-mean-posterior-with-an-exponential-prior)
    - [Posterior moment](bayesian-statistics.md#posterior-moment)
    - [Exponential posterior for a uniform endpoint](bayesian-statistics.md#exponential-posterior-for-a-uniform-endpoint)
    - [Bounded uniform-location posterior](bayesian-statistics.md#bounded-uniform-location-posterior)
    - [Discrete uniform endpoint posterior](bayesian-statistics.md#discrete-uniform-endpoint-posterior)
    - [Posterior rank distribution](bayesian-statistics.md#posterior-rank-distribution)
    - [Posterior variance](bayesian-statistics.md#posterior-variance)
      - [Posterior covariance matrix](bayesian-statistics.md#posterior-covariance-matrix)
    - [Posterior predictive distribution](bayesian-statistics.md#posterior-predictive-distribution)
      - [Posterior predictive check](bayesian-statistics.md#posterior-predictive-check)
        - [Conditional versus marginal posterior predictive checks](bayesian-statistics.md#conditional-versus-marginal-posterior-predictive-checks)
    - [Flat-prior elimination of a Gaussian common mean](bayesian-statistics.md#flat-prior-elimination-of-a-gaussian-common-mean)
    - [Posterior predictive probability](bayesian-statistics.md#posterior-predictive-probability)
    - [Posterior density](bayesian-statistics.md#posterior-density)
      - [Log-posterior](bayesian-statistics.md#log-posterior)
    - [Posterior mean](bayesian-statistics.md#posterior-mean)
      - [Posterior expectation by Laplace approximation](bayesian-statistics.md#posterior-expectation-by-laplace-approximation)
    - [Posterior probability](bayesian-statistics.md#posterior-probability)
      - [Posterior odds](bayesian-statistics.md#posterior-odds)
        - [Base-rate effect in a positive study](bayesian-statistics.md#base-rate-effect-in-a-positive-study)
    - [Point-null mixture prior](bayesian-statistics.md#point-null-mixture-prior)
      - [Marginal likelihood for a Gaussian point-null mixture](bayesian-statistics.md#marginal-likelihood-for-a-gaussian-point-null-mixture)
        - [Posterior probability of a Gaussian point null](bayesian-statistics.md#posterior-probability-of-a-gaussian-point-null)
          - [Jeffreys-Lindley paradox for a Gaussian point null](bayesian-statistics.md#jeffreys-lindley-paradox-for-a-gaussian-point-null)
    - [Improper prior](bayesian-statistics.md#improper-prior)
      - [Haldane prior](bayesian-statistics.md#haldane-prior)
      - [Scale-invariant prior](bayesian-statistics.md#scale-invariant-prior)
      - [Improper posterior from a log-uniform random-effect scale prior](bayesian-statistics.md#improper-posterior-from-a-log-uniform-random-effect-scale-prior)
      - [Posterior propriety](bayesian-statistics.md#posterior-propriety)
        - [Empty component under an improper prior](bayesian-statistics.md#empty-component-under-an-improper-prior)
    - [Poisson-gamma conjugacy](bayesian-statistics.md#poisson-gamma-conjugacy)
      - [Log-gamma prior for a Poisson log-intercept](bayesian-statistics.md#log-gamma-prior-for-a-poisson-log-intercept)
      - [Poisson-gamma conjugacy with unequal exposures](bayesian-statistics.md#poisson-gamma-conjugacy-with-unequal-exposures)
    - [Gamma-exponential conjugacy](bayesian-statistics.md#gamma-exponential-conjugacy)
    - [Beta-binomial conjugacy](bayesian-statistics.md#beta-binomial-conjugacy)
      - [Beta-geometric conjugacy](bayesian-statistics.md#beta-geometric-conjugacy)
      - [Beta-binomial distribution](bayesian-statistics.md#beta-binomial-distribution)
        - [Uniform-count predictive property](bayesian-statistics.md#uniform-count-predictive-property)
          - [Hypergeometric allocation of exchangeable Bernoulli counts](bayesian-statistics.md#hypergeometric-allocation-of-exchangeable-bernoulli-counts)
      - [Beta-binomial exchangeable coupling](bayesian-statistics.md#beta-binomial-exchangeable-coupling)
  - [Bayes estimator](bayesian-statistics.md#bayes-estimator)
    - [Bayes estimator under weighted absolute loss](bayesian-statistics.md#bayes-estimator-under-weighted-absolute-loss)
    - [Bayes decision rule](bayesian-statistics.md#bayes-decision-rule)
      - [Extended Bayes rule](bayesian-statistics.md#extended-bayes-rule)
    - [Bayes estimator under squared error loss](bayesian-statistics.md#bayes-estimator-under-squared-error-loss)
      - [Proper-prior obstruction to homogeneous variance Bayes rules](bayesian-statistics.md#proper-prior-obstruction-to-homogeneous-variance-bayes-rules)
      - [Gaussian normal-mean shrinkage Bayes estimator](bayesian-statistics.md#gaussian-normal-mean-shrinkage-bayes-estimator)
    - [Bayes estimator under parameter-weighted squared error](bayesian-statistics.md#bayes-estimator-under-parameter-weighted-squared-error)
    - [Bayes estimator under reciprocal weighted quadratic loss](bayesian-statistics.md#bayes-estimator-under-reciprocal-weighted-quadratic-loss)
    - [Posterior expected loss](bayesian-statistics.md#posterior-expected-loss)
  - [Markov chain Monte Carlo](bayesian-statistics.md#markov-chain-monte-carlo)
    - [Autocorrelation time](bayesian-statistics.md#autocorrelation-time)
    - [Burn-in](bayesian-statistics.md#burn-in)
    - [MCMC trace diagnosis and proposal tuning](bayesian-statistics.md#mcmc-trace-diagnosis-and-proposal-tuning)
    - [Coupling from the past](bayesian-statistics.md#coupling-from-the-past)
      - [Monotone coupling from the past](bayesian-statistics.md#monotone-coupling-from-the-past)
    - [Reversible-jump Markov chain Monte Carlo](bayesian-statistics.md#reversible-jump-markov-chain-monte-carlo)
      - [Trans-dimensional annealing for penalized likelihood](bayesian-statistics.md#trans-dimensional-annealing-for-penalized-likelihood)
        - [Binomial-normal reversible-jump annealing](bayesian-statistics.md#binomial-normal-reversible-jump-annealing)
      - [Birth and death moves for Bayesian variable selection](bayesian-statistics.md#birth-and-death-moves-for-bayesian-variable-selection)
      - [Centered polynomial birth move in reversible-jump sampling](bayesian-statistics.md#centered-polynomial-birth-move-in-reversible-jump-sampling)
      - [Pseudo-prior](bayesian-statistics.md#pseudo-prior)
        - [Pseudo-prior augmentation for model comparison](bayesian-statistics.md#pseudo-prior-augmentation-for-model-comparison)
          - [Poisson mean equality model comparison](bayesian-statistics.md#poisson-mean-equality-model-comparison)
      - [Equal-dimension reversible-jump acceptance probability](bayesian-statistics.md#equal-dimension-reversible-jump-acceptance-probability)
    - [Hit-and-run sampler](bayesian-statistics.md#hit-and-run-sampler)
      - [Hit-and-run kernel density](bayesian-statistics.md#hit-and-run-kernel-density)
    - [Markov chain Monte Carlo convergence diagnostics](bayesian-statistics.md#markov-chain-monte-carlo-convergence-diagnostics)
      - [Potential scale reduction factor](bayesian-statistics.md#potential-scale-reduction-factor)
      - [Trace plot](bayesian-statistics.md#trace-plot)
    - [Thinning of a Markov chain](bayesian-statistics.md#thinning-of-a-markov-chain)
    - [Geometric ergodicity](bayesian-statistics.md#geometric-ergodicity)
      - [Central limit theorem for a geometrically ergodic Markov chain](bayesian-statistics.md#central-limit-theorem-for-a-geometrically-ergodic-markov-chain)
      - [Uniform geometric ergodicity](bayesian-statistics.md#uniform-geometric-ergodicity)
      - [Burn-in total variation comparison](bayesian-statistics.md#burn-in-total-variation-comparison)
      - [Absolute L2 spectral gap of a reversible Markov chain](bayesian-statistics.md#absolute-l2-spectral-gap-of-a-reversible-markov-chain)
        - [Stationary covariance bound for reversible Markov chains](bayesian-statistics.md#stationary-covariance-bound-for-reversible-markov-chains)
      - [Markov-chain law of large numbers](bayesian-statistics.md#markov-chain-law-of-large-numbers)
      - [Minorization condition](bayesian-statistics.md#minorization-condition)
        - [Doeblin's condition](bayesian-statistics.md#doeblin-s-condition)
      - [Small set](bayesian-statistics.md#small-set)
      - [Drift-minorisation condition](bayesian-statistics.md#drift-minorisation-condition)
        - [Geometric drift condition](bayesian-statistics.md#geometric-drift-condition)
          - [Bounded conditional moments imply a geometric drift](bayesian-statistics.md#bounded-conditional-moments-imply-a-geometric-drift)
    - [Markov chain Monte Carlo asymptotic variance](bayesian-statistics.md#markov-chain-monte-carlo-asymptotic-variance)
    - [Discrete-time Poincaré inequality for a Markov kernel](bayesian-statistics.md#discrete-time-poincare-inequality-for-a-markov-kernel)
    - [Peskun ordering](bayesian-statistics.md#peskun-ordering)
    - [Hamiltonian Monte Carlo](bayesian-statistics.md#hamiltonian-monte-carlo)
      - [Surrogate Hamiltonian Monte Carlo](bayesian-statistics.md#surrogate-hamiltonian-monte-carlo)
    - [Metropolis–Hastings algorithm](bayesian-statistics.md#metropolis-hastings-algorithm)
      - [Metropolis-within-Gibbs algorithm](bayesian-statistics.md#metropolis-within-gibbs-algorithm)
      - [Pseudo-marginal Metropolis–Hastings algorithm](bayesian-statistics.md#pseudo-marginal-metropolis-hastings-algorithm)
        - [Unbiased likelihood estimator](bayesian-statistics.md#unbiased-likelihood-estimator)
      - [Metropolis–Hastings acceptance probability](bayesian-statistics.md#metropolis-hastings-acceptance-probability)
      - [Proposal distribution](bayesian-statistics.md#proposal-distribution)
        - [Involutive Metropolis proposal](bayesian-statistics.md#involutive-metropolis-proposal)
        - [Orthogonal-mixture Metropolis proposal](bayesian-statistics.md#orthogonal-mixture-metropolis-proposal)
        - [Gaussian autoregressive proposal reversible with respect to a standard normal distribution](bayesian-statistics.md#gaussian-autoregressive-proposal-reversible-with-respect-to-a-standard-normal-distribution)
          - [Preconditioned Crank–Nicolson algorithm](bayesian-statistics.md#preconditioned-crank-nicolson-algorithm)
      - [Random-walk Metropolis algorithm](bayesian-statistics.md#random-walk-metropolis-algorithm)
        - [Positive-parameter random walk with boundary rejection](bayesian-statistics.md#positive-parameter-random-walk-with-boundary-rejection)
        - [Proposal scale and random-walk Metropolis efficiency](bayesian-statistics.md#proposal-scale-and-random-walk-metropolis-efficiency)
      - [Independence Metropolis–Hastings algorithm](bayesian-statistics.md#independence-metropolis-hastings-algorithm)
    - [Effective sample size of a Markov chain](bayesian-statistics.md#effective-sample-size-of-a-markov-chain)
      - [Integrated autocorrelation time](bayesian-statistics.md#integrated-autocorrelation-time)
    - [Gibbs sampler](bayesian-statistics.md#gibbs-sampler)
      - [Gaussian Gibbs sweep autocorrelation](bayesian-statistics.md#gaussian-gibbs-sweep-autocorrelation)
      - [Gaussian two-coordinate Gibbs recursion](bayesian-statistics.md#gaussian-two-coordinate-gibbs-recursion)
      - [WinBUGS](bayesian-statistics.md#winbugs)
      - [Linear contraction of a two-coordinate Gaussian Gibbs sweep](bayesian-statistics.md#linear-contraction-of-a-two-coordinate-gaussian-gibbs-sweep)
      - [Gibbs sampling for a finite hidden spin field](bayesian-statistics.md#gibbs-sampling-for-a-finite-hidden-spin-field)
        - [Local likelihood factors in a hidden spin field](bayesian-statistics.md#local-likelihood-factors-in-a-hidden-spin-field)
      - [Systematic Gibbs sampling need not be reversible](bayesian-statistics.md#systematic-gibbs-sampling-need-not-be-reversible)
      - [Blocked Gibbs sampler](bayesian-statistics.md#blocked-gibbs-sampler)
        - [Checkerboard Gibbs sampling](bayesian-statistics.md#checkerboard-gibbs-sampling)
      - [Random-scan Gibbs sampler](bayesian-statistics.md#random-scan-gibbs-sampler)
        - [Detailed balance of a random-scan Gibbs sampler](bayesian-statistics.md#detailed-balance-of-a-random-scan-gibbs-sampler)
      - [Tempered Gibbs sampler](bayesian-statistics.md#tempered-gibbs-sampler)
      - [Stationarity of the two-coordinate Gibbs sampler](bayesian-statistics.md#stationarity-of-the-two-coordinate-gibbs-sampler)
      - [Normal mean-precision Gibbs sampler](bayesian-statistics.md#normal-mean-precision-gibbs-sampler)
  - [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence)
    - [Evidence averaging under an interval prior](bayesian-statistics.md#evidence-averaging-under-an-interval-prior)
      - [Laplace-likelihood interval evidence](bayesian-statistics.md#laplace-likelihood-interval-evidence)
    - [Prior predictive check](bayesian-statistics.md#prior-predictive-check)
    - [Harmonic mean estimator of Bayesian model evidence](bayesian-statistics.md#harmonic-mean-estimator-of-bayesian-model-evidence)
    - [Bayes factor](bayesian-statistics.md#bayes-factor)
      - [Uniform-alternative binomial Bayes factor](bayesian-statistics.md#uniform-alternative-binomial-bayes-factor)
      - [Gaussian practical-null mixture](bayesian-statistics.md#gaussian-practical-null-mixture)
      - [Savage-Dickey density ratio](bayesian-statistics.md#savage-dickey-density-ratio)
  - [Bayesian model averaging](bayesian-statistics.md#bayesian-model-averaging)
  - [Evidence lower bound](bayesian-statistics.md#evidence-lower-bound)
- [Jackknife bias correction](#jackknife-bias-correction)
  - [Sample variance](#sample-variance)
    - [Empirical variance](#empirical-variance)
    - [Pooled sample variance](#pooled-sample-variance)
- [Estimating equation](#estimating-equation)
  - [Generalized estimating equation](#generalized-estimating-equation)
    - [Working correlation matrix](#working-correlation-matrix)
    - [Population-averaged logistic model for repeated binary outcomes](#population-averaged-logistic-model-for-repeated-binary-outcomes)
      - [Inverse-observation-weighted estimating equations for longitudinal dropout](#inverse-observation-weighted-estimating-equations-for-longitudinal-dropout)
    - [Marginal incidence trend with clustered observations](#marginal-incidence-trend-with-clustered-observations)
  - [Z-estimator](#z-estimator)
    - [Consistency of a uniquely bracketed zero](#consistency-of-a-uniquely-bracketed-zero)
- [Asymptotic normality](#asymptotic-normality)
  - [Slutsky theorem](#slutsky-theorem)
  - [Sandwich covariance matrix](#sandwich-covariance-matrix)
  - [Delta method](#delta-method)
    - [Variance-stabilizing transformation](#variance-stabilizing-transformation)
      - [Log absolute value stabilization of a normal scale family](#log-absolute-value-stabilization-of-a-normal-scale-family)
    - [Functional delta method](#functional-delta-method)
    - [Asymptotic distribution of the Gaussian sample correlation](#asymptotic-distribution-of-the-gaussian-sample-correlation)
  - [Endpoint asymptotics of the symmetric-uniform maximum likelihood estimator](#endpoint-asymptotics-of-the-symmetric-uniform-maximum-likelihood-estimator)
- [Asymptotic relative efficiency](#asymptotic-relative-efficiency)
- [Wald confidence interval](#wald-confidence-interval)
- [Heteroskedasticity-consistent standard errors](#heteroskedasticity-consistent-standard-errors)

## Blind analysis

↑ **Parent:** [Statistical inference](statistical-inference.md)

An analysis in which data capable of revealing the sought result are hidden while selection and inference procedures are chosen. It reduces result-dependent tuning. [calibration](differential-geometry.md#calibration-differential-geometry) samples and predefined validation samples remain necessary; blinding does not itself correct a defective background model.

## Pseudolikelihood

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudolikelihood)

A [pseudolikelihood](#pseudolikelihood) multiplies conditional probabilities rather than the full joint [likelihood function](maximum-likelihood-estimation.md#likelihood-function). It can be useful for fitting a [Markov random field](statistical-model.md#markov-random-field), but using the product itself as a probability density defines a different model unless an additional equivalence is established.

<h2 id="winner-s-curse">Winner's curse</h2>

↑ **Parent:** [Statistical inference](statistical-inference.md)

Overestimation of effect magnitude when noisy discoveries are selected for unusually strong apparent effects. Independent replication and explicit modeling of the selection process help correct the bias.

## Frequency estimation

↑ **Parent:** [Statistical inference](statistical-inference.md)

[Frequency estimation](#frequency-estimation) infers a periodic signal's [frequency](wave.md#frequency) from observed samples. It may use a peak of the [discrete Fourier transform](discrete-fourier-transform.md), or fit a sinusoidal model with amplitude, [phase](wave.md#phase-waves), and [frequency](wave.md#frequency) as unknown parameters. Its attainable precision depends on noise, observation duration, [sampling rate](wave-equation.md#sampling-rate), and the estimator. [Fourier frequency resolution](discrete-fourier-transform.md#fourier-frequency-resolution) alone does not specify that precision.

## Effect size

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Effect_size)

An [effect size](#effect-size) measures the magnitude of an observed or modeled relationship. A [standardized mean difference](causal-inference.md#standardized-mean-difference) expresses a mean contrast in standard-deviation units; other [effect sizes](#effect-size) include a [correlation coefficient](variance.md#pearson-correlation-coefficient) or [odds ratio](statistical-modelling.md#odds-ratio). Magnitude is distinct from the evidence against a [null hypothesis](statistical-hypothesis-test.md#null-hypothesis) supplied by a [p-value](statistical-hypothesis-test.md#p-value): a small [effect size](#effect-size) can have a small [p-value](statistical-hypothesis-test.md#p-value) in a sufficiently large sample.

## Statistical process control

↑ **Parent:** [Statistical inference](statistical-inference.md)

Statistical process control compares observed process outcomes with a stable reference model and [control limits](#control-limits) reflecting expected sampling variation. An observation outside those limits is a signal to investigate, not proof of a specific cause. Varying sample volumes require varying limits, and [multiple testing](statistical-hypothesis-test.md#multiple-hypothesis-testing) changes the chance of a chance signal somewhere in the display.

### CUSUM

↑ **Parent:** [Statistical process control](#statistical-process-control)

A [CUSUM](#cusum) accumulates evidence for a change in a monitored [probability distribution](probability-distribution.md). With $W_t$ a [log-likelihood ratio](statistical-hypothesis-test.md#log-likelihood-ratio) increment favoring a specified changed distribution, reset the accumulated score at zero and signal when it exceeds a chosen boundary $h$. For $C_0=0$, $C_t$ is the largest nonnegative sum of successive increments ending at $t$. This permits repeated detection of a change with an unknown onset, rather than a single fixed-start test.

#### Poisson likelihood-ratio CUSUM

↑ **Parent:** [CUSUM](#cusum)

For independent [Poisson](discrete-probability-distribution.md#poisson-distribution) observations, comparing mean $\lambda_{0t}$ with $\theta\lambda_{0t}$ gives the displayed [log-likelihood ratio](statistical-hypothesis-test.md#log-likelihood-ratio). Updating a [CUSUM](#cusum) with these scores targets the specified multiplicative increase. Its expected score is negative under the null and positive under the alternative when $\theta>1$, so resetting at zero discards earlier evidence against an increase.

#### Average run length

↑ **Parent:** [CUSUM](#cusum)

The average run length of a [CUSUM](#cusum) is the [expectation](expected-value.md) of its first signalling time under a specified data model and initial chart state. A large in-control average run length discourages false alarms; a small out-of-control value indicates rapid detection. The mean alone does not give a finite-horizon [Type I error](information-theory.md#type-i-and-type-ii-errors) probability or the complete detection-delay distribution.

#### Fast initial response CUSUM

↑ **Parent:** [CUSUM](#cusum)

A [fast initial response CUSUM](#fast-initial-response-cusum) starts a [CUSUM](#cusum) with a positive head start below its signalling boundary. Before its first reset, it accumulates a fixed-start [log-likelihood ratio](statistical-hypothesis-test.md#log-likelihood-ratio) like a [sequential probability ratio test](statistical-hypothesis-test.md#sequential-probability-ratio-test); after resetting to zero it behaves as an ordinary [CUSUM](#cusum). It gives faster initial detection when the process may already be out of control, at the cost of changed initial false-alarm behavior.

### Hospital mortality funnel plot

↑ **Parent:** [Statistical process control](#statistical-process-control)

A hospital mortality funnel plot places each hospital's observed mortality proportion against its case volume. Under an independent [binomial distribution](discrete-probability-distribution.md#binomial-distribution) model with common target p, the [standard error](#standard-error) is $\sqrt{p(1-p)/n_i}$, so uncertainty bands contract as volume grows. This is a provider-performance plot, distinct in purpose and axes from a meta-analysis funnel plot. A signal requires investigation of data quality and patient case mix before drawing a causal conclusion.

#### Binomial funnel control limits

↑ **Parent:** [Hospital mortality funnel plot](#hospital-mortality-funnel-plot)

The displayed pointwise [control limits](#control-limits) follow from the [normal approximation](convergence-of-random-variables.md#normal-approximation) to an observed [binomial proportion](discrete-probability-distribution.md#binomial-proportion). Clip plotted limits to the probability range. Their nominal coverage is approximate and can be poor for small expected counts; exact binomial tails give a discrete alternative. Pointwise coverage does not provide simultaneous coverage of all hospitals; use [Bonferroni correction](statistical-hypothesis-test.md#bonferroni-correction) or another [familywise error rate](statistical-hypothesis-test.md#familywise-error-rate) procedure when that is the required guarantee.

### Control limits

↑ **Parent:** [Statistical process control](#statistical-process-control)

Control limits bound the sampling outcomes expected under a specified reference process. An observation outside a limit is a [statistical hypothesis testing](statistical-hypothesis-test.md) signal to investigate the reference model. These are limits for observations under that model, rather than a [confidence interval](#confidence-interval) constructed around each observed estimate. Their calibration may be pointwise, simultaneous or sequential.

## Jackknife resampling

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jackknife_resampling)

The delete-one form of [jackknife resampling](#jackknife-resampling) recalculates a [statistic](#statistic) after deleting each observation in turn. It uses one observed [statistical sample](#statistical-sample) to investigate how sensitive an [estimator](statistical-modelling.md#estimator) is to its individual observations, and supplies both a [jackknife variance estimator](#jackknife-variance-estimator) and [jackknife bias correction](#jackknife-bias-correction). The calculations are deterministic once the data are fixed: no random draws are needed.

In the basic setting, $X_1,\ldots,X_n$ are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), with [sample size](probability-and-statistics.md#sample-size) $n>1$. Let $x_1,\ldots,x_n$ be the observed values and $\widehat\theta_n=t_n(x_1,\ldots,x_n)$ a scalar [estimator](statistical-modelling.md#estimator) of an [estimand](#estimand) $\theta$. Apply the same estimation rule to each reduced [statistical sample](#statistical-sample), using its new [sample size](probability-and-statistics.md#sample-size) $n-1$ wherever the rule requires it:

$$
\widehat\theta_{(-i)}=t_{n-1}(x_1,\ldots,x_{i-1},x_{i+1},\ldots,x_n),\qquad
i=1,\ldots,n,\qquad
\overline\theta_J=\frac1n\sum_{i=1}^n\widehat\theta_{(-i)}.
$$

Every index is deleted exactly once; an unusual value is treated by the same rule as every other value. The [mean](expected-value.md) $\overline\theta_J$ summarizes the deletion estimates. They overlap in $n-2$ observations, so they are generally not [independent random variables](random-variable.md#independent-random-variables) representing fresh repetitions of the original experiment. Cosma Shalizi's [Carnegie Mellon jackknife notes, Sections 1–3 and 5](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) explain this construction and its scaling.

For a concrete [sample mean](variance.md#sample-mean), use the data $(1,2,3,4,10)$, whose full [sample mean](variance.md#sample-mean) is $\overline x=4$. The five deletion [sample means](variance.md#sample-mean), in observation order, are

$$
(\widehat\theta_{(-1)},\ldots,\widehat\theta_{(-5)})
=(4.75,4.5,4.25,4,2.5),\qquad \overline\theta_J=4.
$$

Deleting $1$ raises the [sample mean](variance.md#sample-mean) by $0.75$, while deleting $10$ lowers the [sample mean](variance.md#sample-mean) by $1.5$. Thus $10$ has the largest deletion effect in this [statistical sample](#statistical-sample). This is a descriptive sensitivity calculation, not a rule for removing that observation: the full [sample mean](variance.md#sample-mean) remains $4$.

<a id="image-delete-each-observation-once-and-recompute-the-sample-mean"></a>
![](jackknife-leave-one-out.png)

**[Figure 1](#image-delete-each-observation-once-and-recompute-the-sample-mean). Delete each observation once and recompute the sample mean**. The left panel shows all five reduced [statistical samples](#statistical-sample) from $(1,2,3,4,10)$; each crossed entry is omitted only for that row. The right panel shows their [sample means](variance.md#sample-mean) against the full [sample mean](variance.md#sample-mean) $4$. The orange row makes the deletion effect of $10$ visible.

Early literature includes M. H. Quenouille's [Approximate Tests of Correlation in Time-Series, JRSS B 11(1), 68–84 (1949)](https://academic.oup.com/jrsssb/article/11/1/68/7026551) and John W. Tukey's one-paragraph abstract [Bias and Confidence in Not-Quite Large Samples, Annals of Mathematical Statistics 29(2), 614 (1958)](https://www.jstor.org/stable/2237363), within the issue's collected abstracts. Shalizi's [historical notes and bibliography](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) discuss the later development of [jackknife bias correction](#jackknife-bias-correction) and the [jackknife variance estimator](#jackknife-variance-estimator).

### Jackknife variance estimator

↑ **Parent:** [Jackknife resampling](#jackknife-resampling)

The [jackknife variance estimator](#jackknife-variance-estimator) estimates the [sampling variance](statistical-modelling.md#variance-of-an-estimator) of the full-data [estimator](statistical-modelling.md#estimator), using the deletion estimates and their [mean](expected-value.md) from [jackknife resampling](#jackknife-resampling):

$$
\widehat V_J=\frac{n-1}{n}\sum_{i=1}^n
(\widehat\theta_{(-i)}-\overline\theta_J)^2,\qquad
\widehat{\operatorname{SE}}_J=\sqrt{\widehat V_J}.
$$

The square root is the estimated [standard error](#standard-error). The factor $n-1$ multiplies the divisor-$n$ [variance](variance.md) of the deletion estimates: those estimates vary less than estimates from new [independent](random-variable.md#independent-random-variables) experiments because almost all their observations are shared. Ryan Tibshirani's [Carnegie Mellon notes on computing jackknife standard errors](https://www.stat.cmu.edu/~ryantibs/statcomp-F15/lectures/design.html) give the same scaling in terms of the divisor-$(n-1)$ [sample variance](#sample-variance) of the deletion estimates.

For the [sample mean](variance.md#sample-mean), this formula has an exact algebraic simplification. With $s_n^2$ denoting the usual [sample variance](#sample-variance),

$$
\widehat\theta_{(-i)}=\frac{n\overline x-x_i}{n-1},\qquad
\overline\theta_J=\overline x,\qquad
\widehat\theta_{(-i)}-\overline\theta_J
=-\frac{x_i-\overline x}{n-1},
$$

and therefore

$$
\widehat V_J=\frac{1}{n(n-1)}\sum_{i=1}^n(x_i-\overline x)^2
=\frac{s_n^2}{n}.
$$

Under the [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) assumption and a finite second [moment](expected-value.md#moment), $s_n^2$ is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the population [variance](variance.md) $\sigma^2$. Consequently $\widehat V_J$ is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the [sample mean](variance.md#sample-mean)'s [sampling variance](statistical-modelling.md#variance-of-an-estimator) $\sigma^2/n$. The equality $\widehat V_J=s_n^2/n$ itself holds for any observed data with $n>1$; its sampling interpretation uses the stated assumptions.

For $(1,2,3,4,10)$, the sum of squared deviations from the [sample mean](variance.md#sample-mean) is $50$, giving [sample variance](#sample-variance) $s_5^2=50/4=12.5$. The deletion [sample means](variance.md#sample-mean) have squared deviations totaling $3.125$, so

$$
\widehat V_J=\frac45(3.125)=2.5=\frac{12.5}{5},\qquad
\widehat{\operatorname{SE}}_J=\sqrt{2.5}\approx1.58114.
$$

Here $12.5$ estimates the [variance](variance.md) of individual observations, while $2.5$ estimates the [sampling variance](statistical-modelling.md#variance-of-an-estimator) of their [sample mean](variance.md#sample-mean). These answer different questions.

For more general [statistics](#statistic), validity requires regularity beyond the deletion formula, such as a sufficiently [smooth function](analysis.md#smooth-function) of [sample means](variance.md#sample-mean) with suitable [moments](expected-value.md#moment). Ordinary delete-one [jackknife resampling](#jackknife-resampling) can fail for nonsmooth [quantiles](probability-distribution.md#quantile-function), including the [median](probability-distribution.md#median); see Larry Wasserman's [All of Nonparametric Statistics, Section 3.1](https://www.stat.cmu.edu/~brian/valerie/617-2022/0%20-%20books/2006%20-%20Wasserman%20All%20Of%20Nonparametric%20Statistics.pdf). With [statistical dependence](random-variable.md#statistical-dependence), deleting individual observations need not reproduce the relevant [sampling variance](statistical-modelling.md#variance-of-an-estimator); the deletion scheme must reflect that [statistical dependence](random-variable.md#statistical-dependence). Shalizi's [jackknife notes, Sections 4 and 7](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) distinguish the basic [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) case from extensions.

#### Jackknife and bootstrap variance of a sample second moment

↑ **Parent:** [Jackknife variance estimator](#jackknife-variance-estimator)

For independent identically distributed observations with finite fourth [moment](expected-value.md#moment), the [sample mean](variance.md#sample-mean) of their squares has [sampling variance](statistical-modelling.md#variance-of-an-estimator) $\operatorname{Var}(X^2)/n$. Its [jackknife variance estimator](#jackknife-variance-estimator) is exactly the displayed unbiased estimator, since its leave-one-out values differ from their average by $-(x_i^2-\overline{x^2})/(n-1)$. The [conditional bootstrap variance of a sample mean](statistical-modelling.md#conditional-bootstrap-variance-of-a-sample-mean) is $\widehat v_B=n^{-2}\sum_i(x_i^2-\overline{x^2})^2=(n-1)\widehat v_J/n$. Thus the two methods have a known finite-sample scaling difference, despite sharing the same large-sample target.

## Fisherian conditional inference

↑ **Parent:** [Statistical inference](statistical-inference.md)

In a [parametric statistical model](statistical-model.md#parametric-statistical-model), the [likelihood function](maximum-likelihood-estimation.md#likelihood-function) compares parameter values, while sampling distributions calibrate tests and [confidence intervals](#confidence-interval). A [sufficient statistic](probability-and-statistics.md#sufficient-statistic) retains the parameter information. Conditioning on an observed [ancillary statistic](probability-and-statistics.md#ancillary-statistic) restricts that calibration to experiments with the same ancillary configuration, instead of averaging over configurations whose distribution is unrelated to the parameter. Since the ancillary's marginal law is parameter-free, conditional and unconditional likelihoods have the same parameter-dependent factor. With a [nuisance parameter](statistical-model.md#nuisance-parameter), a conditional law or [pivotal quantity](probability-and-statistics.md#pivotal-quantity) must remove it before inference for the parameter of interest can use a nuisance-free reference law.

### Conditionality principle

↑ **Parent:** [Fisherian conditional inference](#fisherian-conditional-inference)

When an experiment's configuration is observed, inference conditions on the experiment actually performed rather than averaging over its possible configurations. Conditioning on an [ancillary statistic](probability-and-statistics.md#ancillary-statistic) is a central application; freedom from a [nuisance parameter](statistical-model.md#nuisance-parameter) must still be checked in the resulting [conditional distribution](probability-theory.md#conditional-distribution).

## Kolmogorov-Smirnov test

↑ **Parent:** [Statistical inference](statistical-inference.md)

The one-sample [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test) checks [goodness of fit](statistical-modelling.md#goodness-of-fit) by comparing an [empirical distribution function](probability-distribution.md#empirical-distribution-function) $F_n$ with a specified [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) $F_0$. Its [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) $D_n$ is the largest vertical gap anywhere between the two curves. Every threshold asks the same concrete question: what proportion of the observations are at or below it, and what [probability](probability-theory.md#probability) does the proposed [probability distribution](probability-distribution.md) assign there? A large discrepancy supplies evidence against the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis).

For example, four stipulated observations $(1/10,2/5,4/5,9/10)$ compared with the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$ give $D_4=3/10$. Just before $4/5$, only two observations have been counted, so the [empirical distribution function](probability-distribution.md#empirical-distribution-function) approaches $1/2$, while $F_0$ approaches $4/5$. The [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) section calculates every jump-side gap. These are exact illustrative numbers, not experimental measurements or a claim of [statistical significance](statistical-hypothesis-test.md#statistical-significance).

The ordinary one-sample calibration assumes [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) real observations and a [simple hypothesis](statistical-hypothesis-test.md#simple-hypothesis) $H_0:F=F_0$, with $F_0$ a [continuous function](calculus.md#continuous-function) fixed before inspecting these observations. All [statistical parameters](statistical-model.md#statistical-parameter) of $F_0$ must be specified.[1.3.5.16. Kolmogorov-Smirnov Goodness-of-Fit Test](mathematics-bibliography.md#nist-and-sematech-e-handbook-of-statistical-methods/1-3-5-16-kolmogorov-smirnov-goodness-of-fit-test) Under that [null hypothesis](statistical-hypothesis-test.md#null-hypothesis), the [probability integral transform](probability-distribution.md#probability-integral-transform) gives $U_i=F_0(X_i)$ with the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$, retaining [independence](random-variable.md#independent-random-variables). Consequently the [sampling distribution](statistical-modelling.md#sampling-distribution) of $D_n$ depends on the [sample size](probability-and-statistics.md#sample-size) $n$, but not on the particular [continuous](calculus.md#continuous-function) $F_0$. This is the useful sense in which the calibration is distribution-free.

For the [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate one, $F_0(x)=1-e^{-x}$ for $x\geq0$. Take $x_i=-\log(1-u_i)$ for the four stipulated $u_i$ above. The [probability integral transform](probability-distribution.md#probability-integral-transform) changes the horizontal coordinates but preserves both the [order statistics](probability-theory.md#order-statistic) and their cumulative heights, so the same [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) $3/10$ appears on both scales. More generally, for [continuous](calculus.md#continuous-function) $F_0$, the jump-side formulas depend only on $F_0(X_{(i)})$. Strict increase everywhere is unnecessary: intervals on which $F_0$ is constant have [probability](probability-theory.md#probability) zero under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis). This explains the invariance without assuming a strictly positive [probability density function](continuous-probability-distribution.md#probability-density-function).

<a id="image-the-probability-integral-transform-preserves-the-kolmogorov-smirnov-gap-on-exponential-and-uniform-scales"></a>
![](kolmogorov-smirnov-probability-integral-transform.png)

**[Figure 2](#image-the-probability-integral-transform-preserves-the-kolmogorov-smirnov-gap-on-exponential-and-uniform-scales). The probability integral transform preserves the Kolmogorov-Smirnov gap on exponential and uniform scales**. The same four stipulated points are shown as $x_i=-\log(1-u_i)$ on the left and $u_i\in\{1/10,2/5,4/5,9/10\}$ on the right. Open circles indicate left limits of the [empirical distribution function](probability-distribution.md#empirical-distribution-function), filled circles its values. The gap $3/10$ is approached from below the third observation on both scales.

The observed [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) is a discrepancy, whereas its [p-value](statistical-hypothesis-test.md#p-value) is a tail [probability](probability-theory.md#probability) under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis):

$$
p=\Pr_{H_0}(D_n^{\mathrm{new}}\geq d_{\mathrm{obs}}).
$$

Here $D_n^{\mathrm{new}}$ is computed from a fresh sample of the same [sample size](probability-and-statistics.md#sample-size). Choose a [significance level](statistical-hypothesis-test.md#significance-level) $\alpha$ before the test and reject when the calibrated [p-value](statistical-hypothesis-test.md#p-value) is at most $\alpha$. The value $D_4=3/10$ alone supplies neither a [p-value](statistical-hypothesis-test.md#p-value) nor a rejection decision. Failure to reject does not establish that the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis) is true. A finite-sample calibration and the asymptotic [Kolmogorov-Smirnov theorem](#kolmogorov-smirnov-theorem) are distinct; a cutoff for $D_n$ must be rescaled before use with $\sqrt nD_n$.[1.3.5.16. Kolmogorov-Smirnov Goodness-of-Fit Test](mathematics-bibliography.md#nist-and-sematech-e-handbook-of-statistical-methods/1-3-5-16-kolmogorov-smirnov-goodness-of-fit-test)

Fitting [statistical parameters](statistical-model.md#statistical-parameter) on the tested observations replaces $F_0$ by the random $F_{\widehat\theta}$. The resulting transformed observations need not be [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) uniforms, so the ordinary reference law fails. The [Lilliefors test](#lilliefors-test) addresses a particular fitted [normal distribution](probability-distribution.md#normal-distribution). More general [parametric bootstrap](statistical-modelling.md#parametric-bootstrap) calibration must simulate from the fitted [statistical model](statistical-model.md) and repeat the fitting in every replicate; holding the fitted [statistical parameters](statistical-model.md#statistical-parameter) fixed during those comparisons calibrates a different procedure. Such a [parametric bootstrap](statistical-modelling.md#parametric-bootstrap) requires its own validity justification rather than inheriting exactness from the simple-null test.

For a [discrete probability distribution](discrete-probability-distribution.md), $F_0(X)$ is generally not uniform. Equal observations also arise from rounding, so tied data require a calibration that accounts for the [discrete probability distribution](discrete-probability-distribution.md) or the rounding rule. The discrepancy remains meaningful, but continuous-null [p-values](statistical-hypothesis-test.md#p-value) are not automatically valid. [Statistical dependence](random-variable.md#statistical-dependence) likewise changes the reference law. The [two-sample Kolmogorov-Smirnov test](#two-sample-kolmogorov-smirnov-test) compares two [empirical distribution functions](probability-distribution.md#empirical-distribution-function) and has a different calibration.[Kolmogorov-Smirnov Tests (ks.test, R stats documentation)](mathematics-bibliography.md#kolmogorov-smirnov-tests-ks-test-r-stats-documentation)

### Kolmogorov-Smirnov statistic

↑ **Parent:** [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test)

For an [empirical distribution function](probability-distribution.md#empirical-distribution-function) $F_n$ and a specified [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) $F_0$, the one-sample [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) is their [Kolmogorov distance](probability-distribution.md#kolmogorov-distance):

$$
F_n(x)=\frac1n\sum_{j=1}^n\mathbf1_{\{X_j\leq x\}},\qquad
D_n=\sup_{x\in\mathbb R}|F_n(x)-F_0(x)|.
$$

The displayed sum uses an [indicator function](measure-theory.md#indicator-function). With this convention, $F_n$ is [right-continuous](calculus.md#right-continuous-function). For distinct observations, its value and its left [one-sided limit](calculus.md#one-sided-limit) at the $i$th [order statistic](probability-theory.md#order-statistic) are $F_n(X_{(i)})=i/n$ and $F_n(X_{(i)}^-)=(i-1)/n$.

For [continuous](calculus.md#continuous-function) $F_0$, both jump sides matter. Define the two directional discrepancies by

$$
D_n^+=\sup_x(F_n(x)-F_0(x))
=\max_{1\leq i\leq n}\left\{\frac{i}{n}-F_0(X_{(i)})\right\},
$$



$$
D_n^-=\sup_x(F_0(x)-F_n(x))
=\max_{1\leq i\leq n}\left\{F_0(X_{(i)})-\frac{i-1}{n}\right\},\qquad
D_n=\max(D_n^+,D_n^-).
$$

Thus $D_n^+$ uses the [empirical distribution function](probability-distribution.md#empirical-distribution-function) immediately after a jump, and $D_n^-$ uses its left [one-sided limit](calculus.md#one-sided-limit).[1.3.5.16. Kolmogorov-Smirnov Goodness-of-Fit Test](mathematics-bibliography.md#nist-and-sematech-e-handbook-of-statistical-methods/1-3-5-16-kolmogorov-smirnov-goodness-of-fit-test) A [supremum](real-analysis.md#supremum) need not be attained.

For $n=4$, $F_0(x)=x$ on $[0,1]$, and the stipulated [order statistics](probability-theory.md#order-statistic) $(1/10,2/5,4/5,9/10)$, the complete calculation is

$$
\begin{array}{c|c|c|c|c|c}
i&X_{(i)}&F_4(X_{(i)}^-)&F_4(X_{(i)})&i/4-F_0(X_{(i)})&F_0(X_{(i)})-(i-1)/4\\\hline
1&1/10&0&1/4&3/20&1/10\\
2&2/5&1/4&1/2&1/10&3/20\\
3&4/5&1/2&3/4&-1/20&3/10\\
4&9/10&3/4&1&1/10&3/20
\end{array}
$$

The last two columns give the signed directional gaps: $D_4^+=3/20$, $D_4^-=3/10$, and $D_4=3/10$. In contrast, checking only $|F_4(X_{(i)})-F_0(X_{(i)})|$ gives $3/20$ and misses the largest gap approached as $x\uparrow4/5$. At $x=4/5$ itself, the gap has already fallen to $1/20$.

<a id="image-both-jump-sides-determine-the-exact-kolmogorov-smirnov-statistic"></a>
![](kolmogorov-smirnov-ecdf-jump-gaps.png)

**[Figure 3](#image-both-jump-sides-determine-the-exact-kolmogorov-smirnov-statistic). Both jump sides determine the exact Kolmogorov-Smirnov statistic**. The [empirical distribution function](probability-distribution.md#empirical-distribution-function) for four stipulated rational observations is compared with the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$. Open circles show left [one-sided limits](calculus.md#one-sided-limit); filled circles show values at jumps. The green gap is $D_4^+=3/20$ and the magenta gap is the limiting $D_4^-=3/10$.

The finite formula follows from the behavior between jumps: the [empirical distribution function](probability-distribution.md#empirical-distribution-function) $F_n$ is constant and the [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) $F_0$ is [monotone](calculus.md#monotonic-function), so the largest directional gaps occur at the two interval ends, possibly as [one-sided limits](calculus.md#one-sided-limit). The two tails introduce no larger gap. Checking every jump side therefore gives the exact [supremum](real-analysis.md#supremum).

A common normalized [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) is $\sqrt nD_n$, which equals $3/5$ in this example. Its large-sample reference law comes from the [Kolmogorov-Smirnov theorem](#kolmogorov-smirnov-theorem). The unscaled $D_n$ remains the largest difference of cumulative [probabilities](probability-theory.md#probability), not a [p-value](statistical-hypothesis-test.md#p-value).

There is a useful exact exception to the usual warning about fitting [statistical parameters](statistical-model.md#statistical-parameter). Suppose $n\geq2$ [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) observations have the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,\theta)$ with unknown $\theta>0$. Let $M=\max_iX_i$ and let $J$ be the label of its almost surely unique maximizing observation. Conditional on $M=m$ and $J=j$, the surviving labelled observations $(X_i)_{i\ne j}$ are [independent](random-variable.md#independent-random-variables) with the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,m)$; after division by $m$ they are [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) uniforms on $(0,1)$. These are [conditional distributions](probability-theory.md#conditional-distribution) defined by [probability density functions](continuous-probability-distribution.md#probability-density-function), since the event $M=m$ has [probability](probability-theory.md#probability) zero.

To check this, the joint [probability density function](continuous-probability-distribution.md#probability-density-function) of $M$ and $J=j$ is $m^{n-1}/\theta^n$ for $0<m<\theta$. Dividing the original joint [probability density function](continuous-probability-distribution.md#probability-density-function) $\theta^{-n}$ by this factor gives the conditional survivor [probability density function](continuous-probability-distribution.md#probability-density-function)

$$
m^{-(n-1)}\prod_{i\ne j}\mathbf1_{\{0<x_i<m\}}.
$$

This factorization proves the claimed [conditional independence](random-variable.md#conditional-independence); scaling removes $m$. Keep the surviving labels in a fixed order, or apply an [independent](random-variable.md#independent-random-variables) random [permutation](combinatorics.md#permutation). The sorted survivors instead have the joint law of [uniform order statistics](probability-theory.md#uniform-order-statistic) and exhibit [statistical dependence](random-variable.md#statistical-dependence); sorting does not affect their [empirical distribution function](probability-distribution.md#empirical-distribution-function). Delete the maximum itself, which would otherwise become a forced value $1$, and compute the [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) using [sample size](probability-and-statistics.md#sample-size) $n-1$ and jump heights $i/(n-1)$. This gives an exact conditional [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test) under the uniform-endpoint [statistical model](statistical-model.md). It does not justify fitting an arbitrary endpoint or other [statistical parameters](statistical-model.md#statistical-parameter) and using the ordinary $n$-sample calibration.

### Lilliefors test

↑ **Parent:** [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lilliefors_test)

The [Lilliefors test](#lilliefors-test) calibrates the [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) against a [normal distribution](probability-distribution.md#normal-distribution) whose [mean](expected-value.md) and [variance](variance.md) are estimated from the tested observations. In the original procedure, $s^2$ is the [sample variance](#sample-variance) with denominator $n-1$, and $\Phi$ is the [standard normal distribution function](probability-distribution.md#standard-normal-distribution-function). Its reference law includes this fitting step. The original paper's opening procedure and Table 1 explain the changed calibration.[pp. 399-400: opening procedure and Table 1 of the original article; inspected mirrored text](mathematics-bibliography.md#on-the-kolmogorov-smirnov-test-for-normality-with-mean-and-variance-unknown-by-hubert-w-lilliefors)

### Two-sample Kolmogorov-Smirnov test

↑ **Parent:** [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test)

The [two-sample Kolmogorov-Smirnov test](#two-sample-kolmogorov-smirnov-test) compares two [empirical distribution functions](probability-distribution.md#empirical-distribution-function) from [independent](random-variable.md#independent-random-variables) samples, each internally [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables), under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis) that their underlying [probability distributions](probability-distribution.md) coincide. Both curves are estimated from data, so calibration depends on both [sample sizes](probability-and-statistics.md#sample-size); the usual asymptotic scaling is $\sqrt{nm/(n+m)}D_{n,m}$. Tied data can be handled by an appropriate [permutation test](statistical-hypothesis-test.md#permutation-test) under the required [exchangeability](probability-distribution.md#exchangeable-random-variables), rather than by assuming the untied continuous-null law.[Kolmogorov-Smirnov Tests (ks.test, R stats documentation)](mathematics-bibliography.md#kolmogorov-smirnov-tests-ks-test-r-stats-documentation)

## Likelihood principle

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Likelihood_principle)

All evidence in observed data about a parameter is contained in its [likelihood function](maximum-likelihood-estimation.md#likelihood-function); proportional likelihoods carry the same evidence. If a stopping rule contributes only a positive factor independent of the parameter to the complete observed-sample likelihood, that factor does not change likelihood-based inference. Recording only a coarsened part of the sample produces a different likelihood and is not covered by the same invariance claim.

### Exponential sampling stopped by a data-dependent coin

↑ **Parent:** [Likelihood principle](#likelihood-principle)

For independent exponential observations of rate $\theta$, stopping after observation $x$ with known probability $\alpha(x)\in(0,1)$ gives a complete-data likelihood proportional to $\theta^Ne^{-\theta S}$. Its minimal sufficient statistic is $(N,S)$ by the parameter-free likelihood-ratio criterion. If only the last value $Y$ is recorded, its density instead is $\alpha(y)e^{-\theta y}/\int_0^\infty\alpha(x)e^{-\theta x}\,dx$. The stopping rule therefore changes the coarsened-data inference even though it adds no complete-data likelihood factor involving $\theta$.

## Estimand

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Estimand)

An estimand is the population quantity an analysis seeks to learn, as distinct from an [estimator](statistical-modelling.md#estimator) calculated from a sample. In a [randomized controlled trial](causal-inference.md#randomized-controlled-trial), the [causal effect](causal-inference.md#causal-effect) of treatment assignment and the effect of actual treatment receipt are different estimands when adherence is imperfect.

## Efficiency (statistics)

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Efficiency_(statistics))

Statistical efficiency compares the precision of procedures estimating the same [estimand](#estimand). For unbiased [estimators](statistical-modelling.md#estimator), relative efficiency is commonly a ratio of their [variances](variance.md); lower variance means more information from the same sample size. An [efficient estimator](statistical-modelling.md#efficient-estimator) attains a relevant information lower bound. A baseline-adjusted [linear regression](linear-regression.md) can improve precision in a [randomized controlled trial](causal-inference.md#randomized-controlled-trial) by removing prognostic variation.

## Statistical functional

↑ **Parent:** [Statistical inference](statistical-inference.md)

A statistical functional assigns a target value to each [probability measure](probability-space.md#probability-measure) in a [statistical model](statistical-model.md). Examples include an [expected value](expected-value.md), a [quantile](probability-distribution.md#quantile-function), and an [integral](integral.md) of a power of a [probability density function](continuous-probability-distribution.md#probability-density-function). Its behavior along [statistical paths](statistical-model.md#statistical-path) determines whether first-order [influence-function representers](#influence-function-representer) are available.

### Functional statistic

↑ **Parent:** [Statistical functional](#statistical-functional)

A functional statistic evaluates a [statistical functional](#statistical-functional) $T$ at the [empirical distribution](information-theory.md#type-information-theory) $F_n=n^{-1}\sum_i\delta_{X_i}$. The map $T$ acts on distributions, whereas $T(F_n)$ is a [statistic](#statistic). If $T$ has an [asymptotic linear representation](robust-statistics.md#asymptotic-linear-representation), then

$$
T(F_n)-T(F)=\frac1n\sum_i\operatorname{IF}(X_i;T,F)+o_p(n^{-1/2}).
$$

A square-integrable [influence function](robust-statistics.md#influence-function) with mean zero consequently gives [asymptotic variance](statistical-modelling.md#asymptotic-variance) $n^{-1}\int\operatorname{IF}(x;T,F)^2\,dF(x)$ by the [central limit theorem](convergence-of-random-variables.md#central-limit-theorem).

### Density fourth-power functional

↑ **Parent:** [Statistical functional](#statistical-functional)

Along [bounded density tilts](statistical-model.md#bounded-density-tilt), this functional has [derivative](calculus.md#derivative) $4\int f^4g=P_f(4f^3g)$. At a bounded baseline density its [canonical gradient](#canonical-gradient), relative to these regular paths, is $4(f^3-\int f^4)$. A common local bound on nearby densities suffices to obtain the same [derivative](calculus.md#derivative) along arbitrary [differentiable-in-quadratic-mean paths](statistical-model.md#differentiability-in-quadratic-mean) in that bounded neighborhood. A bounded baseline alone is insufficient, because of the [spike obstruction to density-power differentiability](#spike-obstruction-to-density-power-differentiability).

#### Spike obstruction to density-power differentiability

↑ **Parent:** [Density fourth-power functional](#density-fourth-power-functional)

A perturbation can have negligible [Hellinger distance](f-divergence.md#hellinger-distance) but a large [integral](integral.md) of its density's fourth power. At the uniform density on $[0,1]$, let $b(s)=6s(1-s)$ on $[0,1]$ and zero elsewhere, and let $f_t(u)=1-t^4+t^{-2}b(u/t^6)$. Then $\int f_t=1$ and $\int(\sqrt{f_t}-1)^2\leq2t^4=o(t^2)$, so the [score function](statistical-modelling.md#informant-function) is zero. However $\int f_t^4\geq72/(35t^2)$. Thus the [density fourth-power functional](#density-fourth-power-functional) is not continuous along this [differentiable-in-quadratic-mean path](statistical-model.md#differentiability-in-quadratic-mean), despite a bounded baseline and individually bounded nearby densities.

### Pathwise differentiability of a statistical functional

↑ **Parent:** [Statistical functional](#statistical-functional)

A statistical functional is pathwise differentiable relative to chosen [statistical paths](statistical-model.md#statistical-path) if its [derivative](calculus.md#derivative) along every path depends only on that path's [score function](statistical-modelling.md#informant-function) and defines a [bounded linear functional](topological-vector-space.md#continuous-linear-functional) on their [statistical tangent space](statistical-model.md#statistical-tangent-space). The [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) expresses this [derivative](calculus.md#derivative) as an [L2 inner product](measure-theory.md#l2-inner-product) with a unique element of the [statistical tangent space](statistical-model.md#statistical-tangent-space), the [canonical gradient](#canonical-gradient). A path family and the associated [derivative](calculus.md#derivative) remainder conditions must both be specified; a formal [derivative](calculus.md#derivative) along one convenient family does not establish differentiability along all paths.

#### Influence-function representer

↑ **Parent:** [Pathwise differentiability of a statistical functional](#pathwise-differentiability-of-a-statistical-functional)

An influence-function representer is a centered [square-integrable function](measure-theory.md#square-integrable-function) representing [derivatives](calculus.md#derivative) of a [statistical functional](#statistical-functional) along all admissible [score functions](statistical-modelling.md#informant-function). Representers may differ by a [function](function.md) orthogonal to the [statistical tangent space](statistical-model.md#statistical-tangent-space). This pathwise definition is distinct from defining an [influence function](robust-statistics.md#influence-function) solely by point-mass contamination paths.

##### Canonical gradient

↑ **Parent:** [Influence-function representer](#influence-function-representer)

The canonical gradient is the [influence-function representer](#influence-function-representer) in the [statistical tangent space](statistical-model.md#statistical-tangent-space) $\mathcal T$. It equals the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto $\mathcal T$ of any representer. Every other representer differs from it by an element of $\mathcal T^\perp$, so the [Pythagorean theorem in an inner-product space](inner-product.md#pythagorean-theorem-in-an-inner-product-space) gives it minimum [variance](variance.md). For $\psi(P)=Pa$ in an unrestricted density model with bounded $a$, it is $a-Pa$.

## Statistical estimation

↑ **Parent:** [Statistical inference](statistical-inference.md)

Statistical estimation uses observed data to infer numerical properties of a population or model. A point [estimator](statistical-modelling.md#estimator) gives a value, while a [confidence interval](#confidence-interval) describes uncertainty with a specified coverage property. [Maximum likelihood estimation](maximum-likelihood-estimation.md) is one approach; bias, variance, identifiability and the sampling or selection mechanism all affect an estimate's interpretation.

### Ratio estimator

↑ **Parent:** [Statistical estimation](#statistical-estimation)

A ratio estimator divides one statistic by another, for example an estimated joint moment by an estimated marginal probability. Its definition must specify what happens when the denominator is zero. A denominator bounded away from zero permits direct error bounds through $U_n-\theta V_n$.

#### Absolute error bound for a ratio estimator with a controlled denominator

↑ **Parent:** [Ratio estimator](#ratio-estimator)

Set $G_n=U_n-\theta V_n$, and define the estimator on zero-denominator events as part of the model. On $V_n>\delta>0$, its error is at most $|G_n|/\delta$. Centering $G_n$ and applying the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives the displayed bound, where $r_n$ is the expected error on $V_n\le\delta$. This controls a [ratio estimator](#ratio-estimator) without falsely assuming that its numerator and denominator are independent.

## Probability sampling

↑ **Parent:** [Statistical inference](statistical-inference.md)

Probability sampling chooses observational units by a specified random mechanism with known inclusion [probabilities](probability-theory.md#probability). This separates design-based representativeness from the convenience of obtaining particular observations. [Simple random sampling](#simple-random-sampling), [stratified sampling](#stratified-sampling) and [cluster sampling](#cluster-sampling) are different designs with different precision and cost properties.

### Sampling with replacement

↑ **Parent:** [Probability sampling](#probability-sampling)

[Sampling with replacement](#sampling-with-replacement) returns each selected label to the available population before the next draw. Independent uniform draws from a fixed population are [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables); a label can recur. Replacement by itself does not imply uniformity or [independence](random-variable.md#independent-random-variables).

### Inclusion probability

↑ **Parent:** [Probability sampling](#probability-sampling)

An [inclusion probability](#inclusion-probability) is the [probability](probability-theory.md#probability) that a particular unit belongs to the selected sample. For [sample size](probability-and-statistics.md#sample-size) $n$ in [simple random sampling](#simple-random-sampling) from $N$ labels it is $n/N$. It differs from the selection [probability](probability-theory.md#probability) at a particular draw position.

### Unequal probability sampling

↑ **Parent:** [Probability sampling](#probability-sampling)

[Unequal probability sampling](#unequal-probability-sampling) assigns different [inclusion probabilities](#inclusion-probability) to different population units. Estimating an unweighted population summary generally requires accounting for these differences in the [estimator](statistical-modelling.md#estimator).

### Finite population mean

↑ **Parent:** [Probability sampling](#probability-sampling)

The [finite population mean](#finite-population-mean) for $N\geq1$ is the [arithmetic mean](arithmetic.md#arithmetic-mean) of all fixed values in the target population. Under [simple random sampling](#simple-random-sampling), the [sample mean](variance.md#sample-mean) is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of it.

### Finite population variance

↑ **Parent:** [Probability sampling](#probability-sampling)

For $N>1$, the [finite population variance](#finite-population-variance) measures spread about the [finite population mean](#finite-population-mean). Survey-sampling formulas commonly use denominator $N-1$; the denominator-$N$ version is $\sigma_N^2=(N-1)S^2/N$. The normalization must be specified when using a [finite population correction](discrete-probability-distribution.md#finite-population-correction).

### Sampling without replacement

↑ **Parent:** [Probability sampling](#probability-sampling)

[Sampling without replacement](#sampling-without-replacement) selects distinct labelled units: after a unit is selected it is unavailable for the remaining draws. Distinct labels can carry equal numerical values, so repeated values do not necessarily imply a repeated unit. The rule alone does not specify selection [probabilities](probability-theory.md#probability); a procedure favoring particular units is still [sampling without replacement](#sampling-without-replacement) but need not be [simple random sampling](#simple-random-sampling).

In uniform sequential [sampling without replacement](#sampling-without-replacement), the next label is chosen uniformly among those remaining. For a population of $N$ labels, any ordered sequence of $n$ distinct labels has [probability](probability-theory.md#probability) $1/[N(N-1)\cdots(N-n+1)]$. Each size-$n$ [subset](set.md#subset) has $n!$ possible orders, so its [probability](probability-theory.md#probability) is $\binom Nn^{-1}$. This gives the fixed-size [simple random sampling](#simple-random-sampling) design. Equivalently, take the first $n$ labels of a uniformly random [permutation](combinatorics.md#permutation). Restricting a uniformly random [permutation](combinatorics.md#permutation) to a specified label set preserves uniformity; biased modulo mappings should not replace uniform selection.

The draw positions have identical marginal [probability distributions](probability-distribution.md), but exhibit [statistical dependence](random-variable.md#statistical-dependence). If the first label is $i$, the [conditional probability](probability-theory.md#conditional-probability) that the second label is $i$ is zero, whereas its marginal [probability](probability-theory.md#probability) is $1/N$. Thus these draws are not [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) when $N>1$ and $n>1$. For a marked subset of labels, counting size-$n$ [subsets](set.md#subset) with [binomial coefficients](binomial-coefficient.md) gives the [hypergeometric distribution](discrete-probability-distribution.md#hypergeometric-distribution). The resulting negative [covariance](variance.md#covariance) explains the [finite population correction](discrete-probability-distribution.md#finite-population-correction) for both counts and [sample means](variance.md#sample-mean).

#### Marginal and pair probabilities in sampling without replacement

↑ **Parent:** [Sampling without replacement](#sampling-without-replacement)

Take a uniformly random [permutation](combinatorics.md#permutation) of $N>1$ distinguishable objects, of which $K$ are marked. Let $B_i$ mean that position $i$ is marked. Every object is equally likely at a specified position, so $\mathbb P(B_i)=K/N$. For distinct positions $i,j$, their ordered pair is uniform among $N(N-1)$ distinct-object pairs, of which $K(K-1)$ are marked pairs. This proves the second formula. For $K>0$, the [conditional probability](probability-theory.md#conditional-probability) is $\mathbb P(B_i\mid B_j)=(K-1)/(N-1)$.

For the count $M_m$ of marked objects among the first $m$ positions, [indicator random variables](expected-value.md#indicator-random-variable) and [linearity of expectation](expected-value.md#linearity-of-expectation) give $\mathbb E[M_m]=mK/N$. These draws are [exchangeable](probability-distribution.md#exchangeable-random-variables) but generally dependent; equal marginal [probabilities](probability-theory.md#probability) do not imply [independence](random-variable.md#independent-random-variables).

#### First return to equal counts in sampling without replacement

↑ **Parent:** [Sampling without replacement](#sampling-without-replacement)

Draw balls sequentially without replacement from $g$ green and $r$ red balls. Let $T$ be the first positive draw count at which the numbers of drawn green and red balls agree. For $1\leq m\leq\min(g,r)$,

$$
\mathbb P(T=2m)=2C_{m-1}\frac{(g)_m(r)_m}{(g+r)_{2m}},
\qquad C_k=\frac1{k+1}\binom{2k}{k},
$$

where $(q)_j=q(q-1)\cdots(q-j+1)$ denotes the [falling factorial](combinatorics.md#falling-factorial) and $C_k$ is a [Catalan number](combinatorics.md#catalan-number). Odd [first return times](markov-chain.md#first-return-time) are impossible because equality requires an even total number of draws.

To count the successful colour orders, encode green by a step $+1$ and red by a step $-1$. If the first step is positive, a [first return time](markov-chain.md#first-return-time) $2m$ means that the [partial sums](sequence-and-series.md#partial-sum) remain strictly positive until the last step. Delete the first positive step and the last negative step, and shift the remaining heights down by one. The result is a [Dyck path](combinatorics.md#dyck-path) of length $2m-2$, of which there are $C_{m-1}$. Interchanging the colours doubles this count. Every such colour order has the same [probability](probability-theory.md#probability) under [sampling without replacement](#sampling-without-replacement), namely $(g)_m(r)_m/(g+r)_{2m}$, proving the formula. In particular, the numbers of successful colour orders at lengths two, four and six are two, two and four; balanced orders with an earlier return must not be counted.

#### First marked item in a random permutation

↑ **Parent:** [Sampling without replacement](#sampling-without-replacement)

When $m\ge1$ items among $N$ are marked, inspect a uniformly random permutation until the first marked item. For its first position to be $k$, the other $m-1$ marked positions must lie among the last $N-k$ slots. This yields the displayed law with support $1\le k\le N-m+1$. It is the first-success form of [sampling without replacement](#sampling-without-replacement). For one marked item the position is uniform, while its conditional success chance after $r$ failures increases to $1/(N-r)$.

### Cluster sampling

↑ **Parent:** [Probability sampling](#probability-sampling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cluster_sampling)

Cluster sampling chooses groups of observational units, such as production days, rather than dispersed individual units. Testing every unit in a selected group is a one-stage cluster sample. Positive within-cluster [intraclass correlation](variance.md#intraclass-correlation-coefficient) reduces the information supplied by a fixed number of sampled units, although collecting clustered observations can be cheaper.

#### Design effect

↑ **Parent:** [Cluster sampling](#cluster-sampling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Design_effect)

The [design effect](#design-effect) is a sampling [variance](variance.md) under a complex design divided by the corresponding simple-random-sampling [variance](variance.md). For independent equal-size clusters of size $m$ with exchangeable [intraclass correlation](variance.md#intraclass-correlation-coefficient) $\rho$, a common mean-[estimation](#statistical-estimation) approximation is $1+(m-1)\rho$. It expresses the loss of effective [sample size](probability-and-statistics.md#sample-size) from positive correlation; finite-population and unequal-cluster-size designs require their own calculation.

### Stratified sampling

↑ **Parent:** [Probability sampling](#probability-sampling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stratified_sampling)

Stratified sampling partitions a population into strata and samples separately within each. It guarantees specified representation and can improve precision when the strata describe population variation. Equal sampling fractions give equal unit inclusion [probabilities](probability-theory.md#probability); unequal fractions require appropriate weighting for population summaries.

#### Optimal cost-constrained stratified sampling allocation

↑ **Parent:** [Stratified sampling](#stratified-sampling)

Suppose the [variance](variance.md) is $\sum_i v_i/x_i$ and the sampling cost is $\sum_i a_ix_i\leq b$, with positive costs, variance coefficients and budget. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $A^2\leq(\sum_i v_i/x_i)(\sum_i a_ix_i)\leq b\sum_i v_i/x_i$. Equality forces $x_i$ proportional to $\sqrt{v_i/a_i}$ and a tight budget, proving the displayed unique optimum. The minimal variance is $A^2/b$. For the [optimization Lagrangian](mathematical-optimization.md#optimization-lagrangian) $f-\lambda(\sum_i a_ix_i-b)$, the multiplier and budget derivative both equal $-A^2/b^2$. Therefore a small resource change $\delta b$ changes the optimum by $\lambda\delta b+O((\delta b)^2)$. This is a continuous allocation; integer sample-size restrictions define a separate optimization problem.

### Simple random sampling

↑ **Parent:** [Probability sampling](#probability-sampling)

Here [simple random sampling](#simple-random-sampling) means a random unordered [subset](set.md#subset) $A$ of exactly $n$ distinct labels from $\{1,\ldots,N\}$, with every size-$n$ [subset](set.md#subset) equally likely. The [sample size](probability-and-statistics.md#sample-size) is fixed in advance, $1\leq n\leq N$, and [sampling without replacement](#sampling-without-replacement) prevents duplicate units. This is [SRSWOR](#simple-random-sampling); some texts also use "simple random sampling" for independent uniform draws with replacement, which is a different design.[Sampling Theory, Chapter 2, Simple Random Sampling, PDF pp. 1–4: replacement conventions and ordered versus unordered sample probabilities](mathematics-bibliography.md#sampling-theory/chapter-2-simple-random-sampling)

Every label has [inclusion probability](#inclusion-probability) $n/N$, but equal [inclusion probabilities](#inclusion-probability) alone are insufficient. For example, from six labels choose either $\{1,2,3\}$ or $\{4,5,6\}$ with [probability](probability-theory.md#probability) $1/2$. Each label is included with [probability](probability-theory.md#probability) $1/2$, yet eighteen of the twenty size-three [subsets](set.md#subset) are impossible: this is a two-group [cluster sampling](#cluster-sampling) design. [Unequal probability sampling](#unequal-probability-sampling) deliberately changes inclusion [probabilities](probability-theory.md#probability), often to improve precision for a particular [estimand](#estimand), and generally requires an appropriately weighted [estimator](statistical-modelling.md#estimator) rather than the plain [sample mean](variance.md#sample-mean).

Consider the original mathematical population with labelled values $(2,4,6,8,10,12)$, and let $n=2$. The fifteen equiprobable [subsets](set.md#subset), followed by their [sample means](variance.md#sample-mean), are

$$
\begin{array}{c|rrrrr}
\text{first value }2&\{2,4\}:3&\{2,6\}:4&\{2,8\}:5&\{2,10\}:6&\{2,12\}:7\\
4&\{4,6\}:5&\{4,8\}:6&\{4,10\}:7&\{4,12\}:8&\\
6&\{6,8\}:7&\{6,10\}:8&\{6,12\}:9&&\\
8&\{8,10\}:9&\{8,12\}:10&&&\\
10&\{10,12\}:11&&&&
\end{array}
$$

Their [sample means](variance.md#sample-mean) sum to $105$, giving [expected value](expected-value.md) $105/15=7$. Their squared deviations from $7$ sum to $70$, giving [variance](variance.md) $70/15=14/3$. This is an enumeration over hypothetical selections from six stipulated numbers, not measured survey data.

<a id="image-all-fifteen-size-two-subsets-and-all-thirty-six-ordered-replacement-outcomes-from-six-labelled-values"></a>
![](simple-random-sampling-subsets-and-replacement.png)

**[Figure 4](#image-all-fifteen-size-two-subsets-and-all-thirty-six-ordered-replacement-outcomes-from-six-labelled-values). All fifteen size-two subsets and all thirty-six ordered replacement outcomes from six labelled values**.

With independent uniform [sampling with replacement](#sampling-with-replacement), the $6^2=36$ ordered outcomes each have [probability](probability-theory.md#probability) $1/36$. The two orders $(2,4)$ and $(4,2)$ are distinct outcomes, and $(2,2)$ is now possible. Forgetting order does not make the resulting unordered multisets equiprobable: $\{2,4\}$ has [probability](probability-theory.md#probability) $2/36$ but $\{2,2\}$ has [probability](probability-theory.md#probability) $1/36$. The thirty-six [sample means](variance.md#sample-mean) still have [expected value](expected-value.md) $7$, but their squared deviations sum to $210$, giving [variance](variance.md) $210/36=35/6$. Avoiding duplicate labels improves precision for this fixed population.

#### Sample mean under simple random sampling

↑ **Parent:** [Simple random sampling](#simple-random-sampling)

Fix $N>1$ real population values $y_1,\ldots,y_N$. Define the [finite population mean](#finite-population-mean) and two normalizations of the [finite population variance](#finite-population-variance) by

$$
\bar Y=\frac1N\sum_{i=1}^Ny_i,\qquad
S^2=\frac1{N-1}\sum_{i=1}^N(y_i-\bar Y)^2,\qquad
\sigma_N^2=\frac1N\sum_{i=1}^N(y_i-\bar Y)^2=\frac{N-1}{N}S^2.
$$

The values are fixed; only the selected [subset](set.md#subset) $A$ is random. For its [sample mean](variance.md#sample-mean) $\bar y_A=n^{-1}\sum_{i\in A}y_i$, the exact design [expectation](expected-value.md) and [variance](variance.md) are

$$
\mathbb E[\bar y_A]=\bar Y,\qquad
\operatorname{Var}(\bar y_A)=\left(1-\frac nN\right)\frac{S^2}{n}
=\frac{N-n}{N-1}\frac{\sigma_N^2}{n}.
$$

The [sample mean](variance.md#sample-mean) is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the [finite population mean](#finite-population-mean). At $n=N$, every unit is observed and $\bar y_A=\bar Y$ exactly, so the [variance](variance.md) is zero. The $N=1$ case is deterministic and is handled directly, since $S^2$ is undefined then.[Sampling Theory, Chapter 2, PDF pp. 2, 6–9: variance normalizations, unbiasedness, covariance derivation and finite population correction](mathematics-bibliography.md#sampling-theory/chapter-2-simple-random-sampling)

The [finite population correction](discrete-probability-distribution.md#finite-population-correction) depends on the baseline. With the $N-1$ normalization it is $1-n/N$ multiplying $S^2/n$. With the $N$ normalization it is $(N-n)/(N-1)$ multiplying $\sigma_N^2/n$, the exact [variance](variance.md) for independent uniform [sampling with replacement](#sampling-with-replacement). The [standard error](#standard-error) uses the square root of the relevant [variance](variance.md) factor. Mixing the two normalizations gives a wrong answer even at $n=1$, when replacement cannot matter. For the six-value example, $\bar Y=7$, $\sum_i(y_i-7)^2=70$, $S^2=14$ and $\sigma_N^2=35/3$, reproducing $14/3$ without replacement and $35/6$ with replacement.

A short proof exposes the [statistical dependence](random-variable.md#statistical-dependence). Let $X_r$ be the value at position $r$ in uniform sequential [sampling without replacement](#sampling-without-replacement), so each $X_r$ has [expected value](expected-value.md) $\bar Y$ and [variance](variance.md) $\sigma_N^2$. Write $d_i=y_i-\bar Y$. Every ordered pair of distinct labels is equally likely, and $\sum_i d_i=0$, hence for $r\ne s$,

$$
\operatorname{Cov}(X_r,X_s)=\frac{\sum_{i\ne j}d_id_j}{N(N-1)}
=\frac{(\sum_i d_i)^2-\sum_i d_i^2}{N(N-1)}
=-\frac{\sigma_N^2}{N-1}=-\frac{S^2}{N}.
$$

[Linearity of expectation](expected-value.md#linearity-of-expectation) proves unbiasedness without requiring [independence](random-variable.md#independent-random-variables). The [variance of a sum](variance.md#variance-of-a-sum) includes all $n(n-1)$ ordered [covariance](variance.md#covariance) terms, giving

$$
\operatorname{Var}\left(\frac1n\sum_{r=1}^nX_r\right)
=\frac{n\sigma_N^2-n(n-1)\sigma_N^2/(N-1)}{n^2}.
$$

For the original population, each pair of distinct draw positions has [covariance](variance.md#covariance) $-7/3$. Drawing a high value leaves a lower [mean](expected-value.md) among the remaining values, balancing subsequent draws. Equal marginal [probability distributions](probability-distribution.md) therefore coexist with negative [covariance](variance.md#covariance).

When $2\leq n\leq N$, the [sample variance](#sample-variance) $s_A^2=(n-1)^{-1}\sum_{i\in A}(y_i-\bar y_A)^2$ is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of $S^2$. To check this independently, use $\sum_{i\in A}(y_i-\bar y_A)^2=\sum_{i\in A}(y_i-\bar Y)^2-n(\bar y_A-\bar Y)^2$: its [expected value](expected-value.md) is $n\sigma_N^2-n\operatorname{Var}(\bar y_A)=(n-1)S^2$. Thus $(1-n/N)s_A^2/n$ unbiasedly estimates the [variance](variance.md) of the [sample mean](variance.md#sample-mean); its square root estimates the [standard error](#standard-error), but need not be unbiased.[Sampling Theory, Chapter 2, PDF pp. 10–12: sample-variance and standard-error estimation](mathematics-bibliography.md#sampling-theory/chapter-2-simple-random-sampling)

<a id="image-exact-mean-variance-and-expected-distinct-unit-coverage-as-sample-size-grows-in-the-six-value-population"></a>
![](simple-random-sampling-variance-and-population-coverage.png)

**[Figure 5](#image-exact-mean-variance-and-expected-distinct-unit-coverage-as-sample-size-grows-in-the-six-value-population). Exact mean variance and expected distinct-unit coverage as sample size grows in the six-value population**.

The diagram compares [variance](variance.md) with the expected fraction of distinct population labels observed. Without replacement this fraction is exactly $n/N$; with independent uniform [sampling with replacement](#sampling-with-replacement), a label is missed with [probability](probability-theory.md#probability) $(1-1/N)^n$, so [linearity of expectation](expected-value.md#linearity-of-expectation) gives expected fraction $1-(1-1/N)^n$. At six draws, replacement covers only about $66.5\%$ of labels on average and retains [sample mean](variance.md#sample-mean) [variance](variance.md) $35/18$; sampling all six distinct labels covers the population completely and removes selection uncertainty. This population coverage is distinct from [confidence interval](#confidence-interval) [coverage probability](#coverage-probability).

The correction matters when the [sampling fraction](#sampling-fraction) is appreciable. It calibrates uncertainty about this fixed population under the specified selection mechanism. It does not correct unequal selection weights, missing observations or measurement errors; observing every label also does not eliminate uncertainty about a larger unobserved population. Moreover, an exact [variance](variance.md) alone does not guarantee the [coverage probability](#coverage-probability) of a proposed [confidence interval](#confidence-interval): a small discrete [sampling distribution](statistical-modelling.md#sampling-distribution) can make a [normal approximation](convergence-of-random-variables.md#normal-approximation) inaccurate.

##### Sampling fraction

↑ **Parent:** [Sample mean under simple random sampling](#sample-mean-under-simple-random-sampling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sampling_fraction)

The [sampling fraction](#sampling-fraction) is the [sample size](probability-and-statistics.md#sample-size) divided by the finite population size. In [simple random sampling](#simple-random-sampling), it determines how much the [finite population correction](discrete-probability-distribution.md#finite-population-correction) reduces the [variance](variance.md) relative to $S^2/n$.

## Scoring rule

↑ **Parent:** [Statistical inference](statistical-inference.md)

A [scoring rule](#scoring-rule) turns a [probability distribution](probability-distribution.md) forecast and an observed outcome into a number. For example, a forecast of rain with [probability](probability-theory.md#probability) $0.7$ should express uncertainty more usefully than a bare prediction of rain. A [scoring rule](#scoring-rule) lets us compare such forecasts after observations arrive, and its choice determines whether exaggerating confidence pays. A [proper scoring rule](#proper-scoring-rule) rewards an honest account of uncertainty in [expected value](expected-value.md).

There are two sign conventions. A reward $S(P,x)$ is maximized; a [loss function](foundations-of-mathematics.md#loss-function) $L(P,x)$ is minimized. The conversion $L=-S$ reverses every comparison. Here the [linear probability score](#linear-probability-score) is a reward, while the binary [Brier score](#brier-score) and the negative [logarithmic scoring rule](#logarithmic-scoring-rule) are losses. Calling all three a "score" without specifying the direction would hide the central difference.

Throughout the binary examples, the [random variable](random-variable.md) $Y$ has a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with actual success [probability](probability-theory.md#probability) $q=0.7$, and the report $p\in[0,1]$ assigns [probability](probability-theory.md#probability) $p$ to $Y=1$ and $1-p$ to $Y=0$. The value $q=0.7$ is stipulated by this [statistical model](statistical-model.md); it is not inferred from data or a claim that a forecasting system is calibrated. In practice the true [predictive distribution](probability-distribution.md#predictive-distribution) is unknown, and the relevant $q$ is the [conditional probability](probability-theory.md#conditional-probability) of success given the information available when the forecast is issued. [Propriety](#proper-scoring-rule) evaluates incentives for reporting that [predictive distribution](probability-distribution.md#predictive-distribution); it does not supply the unknown [probabilities](probability-theory.md#probability).

### Linear probability score

↑ **Parent:** [Scoring rule](#scoring-rule)

The [linear probability score](#linear-probability-score) pays the reported [probability](probability-theory.md#probability) of whichever binary outcome occurs. With report $p$ and observed $y\in\{0,1\}$, its reward is

$$
S_{\rm lin}(p,y)=yp+(1-y)(1-p).
$$

It looks sensible: assign more [probability](probability-theory.md#probability) to what happens and receive more reward. But the [expected value](expected-value.md) under a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with true success [probability](probability-theory.md#probability) $q$ is

$$
\mathbb E_q[S_{\rm lin}(p,Y)]=qp+(1-q)(1-p)=1-q+(2q-1)p.
$$

This is an [affine function](vector-space.md#affine-function) of the report. When $q>1/2$, the maximum over $[0,1]$ is at $p=1$; when $q<1/2$, it is at $p=0$. At $q=1/2$, every report ties. Thus the [linear probability score](#linear-probability-score) encourages reporting certainty about the more likely outcome and is not a [proper scoring rule](#proper-scoring-rule).

For the stipulated $q=0.7$, the [expected value](expected-value.md) of the reward is $0.3+0.4p$. Honest reporting $p=0.7$ earns $0.58$ in [expectation](expected-value.md), whereas $p=1$ earns $0.7$. The forecaster improves expected reward by replacing a 70% forecast with a 100% forecast. The [Brier score](#brier-score) and [logarithmic scoring rule](#logarithmic-scoring-rule) avoid this incentive, as the expected-score diagram under [proper scoring rule](#proper-scoring-rule) shows.

### Proper scoring rule

↑ **Parent:** [Scoring rule](#scoring-rule)

A [proper scoring rule](#proper-scoring-rule) makes reporting the true [probability distribution](probability-distribution.md) optimal in [expected value](expected-value.md), for every true [probability distribution](probability-distribution.md) in the allowed class of forecasts. In the reward convention, the inequality in the title holds for every report $P$ and true law $Q$. The [expected value](expected-value.md) is always taken under $Q$, because the report does not change how the outcome is generated. In the loss convention the same definition reads

$$
\mathbb E_Q[L(Q,X)]\leq\mathbb E_Q[L(P,X)]\qquad\text{for every admissible }P,Q.
$$

This requirement makes a [proper scoring rule](#proper-scoring-rule) useful for eliciting [probabilities](probability-theory.md#probability) and comparing [predictive distributions](probability-distribution.md#predictive-distribution): deliberately distorting a known forecast cannot improve its expected reward or expected loss. The reward convention and its strict version are set out in [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others) (Section 1).

For the [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with $q=0.7$, the [Brier score](#brier-score) has expected loss $(p-0.7)^2+0.21$, and the negative [logarithmic scoring rule](#logarithmic-scoring-rule) has expected loss $-0.7\ln p-0.3\ln(1-p)$. Both are minimized at the honest report $p=0.7$. The [linear probability score](#linear-probability-score), by contrast, maximizes its expected reward at $p=1$. These are statements about averaging over both possible outcomes with their actual [probabilities](probability-theory.md#probability).

<a id="image-expected-losses-of-the-brier-score-and-logarithmic-scoring-rule-favor-p-q-0-7-the-linear-probability-score-rewards-p-1"></a>
![](proper-score-expected-losses.png)

**[Figure 6](#image-expected-losses-of-the-brier-score-and-logarithmic-scoring-rule-favor-p-q-0-7-the-linear-probability-score-rewards-p-1). Expected losses of the Brier score and logarithmic scoring rule favor $p=q=0.7$; the linear probability score rewards $p=1$**.

The left panel displays each excess expected loss divided by that rule's expected loss at $p=q$: $0.21$ for the [Brier score](#brier-score) and approximately $0.610864$ for the [logarithmic scoring rule](#logarithmic-scoring-rule). This normalization permits comparison of curve shapes and preserves the minimizing report, since it subtracts a constant and divides by a positive constant independent of $p$. Zero means no excess expected loss. The right panel shows the unmodified [linear probability score](#linear-probability-score) reward, with its maximizing direction labeled explicitly.

#### Strictly proper scoring rule

↑ **Parent:** [Proper scoring rule](#proper-scoring-rule)

A [strictly proper scoring rule](#strictly-proper-scoring-rule) is a [proper scoring rule](#proper-scoring-rule) for which the true [probability distribution](probability-distribution.md) is the unique optimizer of the [expected value](expected-value.md). Equivalently, any different admissible [probability distribution](probability-distribution.md) gives strictly larger expected loss. For [probability density functions](continuous-probability-distribution.md#probability-density-function), two densities that agree [almost everywhere](measure-theory.md#almost-everywhere) represent the same [probability distribution](probability-distribution.md). Ordinary [propriety](#proper-scoring-rule) permits ties: the constant reward $S(P,x)=0$ is a [proper scoring rule](#proper-scoring-rule), because every report ties, but it is not a [strictly proper scoring rule](#strictly-proper-scoring-rule) and elicits no information.

[Strict propriety](#strictly-proper-scoring-rule) concerns [expectation](expected-value.md), not guaranteed success on each observation or each realized dataset. With the stipulated [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) $q=0.7$, suppose the outcome is $Y=0$. The honest report $p=0.7$ then has [Brier score](#brier-score) loss $0.49$, while $p=0.2$ has loss $0.04$. The [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss) similarly gives losses $-\ln(0.3)\approx1.203973$ and $-\ln(0.8)\approx0.223144$. The honest forecast loses this comparison on that draw, which occurs with [probability](probability-theory.md#probability) $0.3$ in the stipulated [statistical model](statistical-model.md).

<a id="image-individual-outcomes-can-favor-a-different-report-even-though-the-expected-brier-score-and-logarithmic-loss-are-uniquely-minimized-at-p-0-7"></a>
![](proper-score-realized-outcomes.png)

**[Figure 7](#image-individual-outcomes-can-favor-a-different-report-even-though-the-expected-brier-score-and-logarithmic-loss-are-uniquely-minimized-at-p-0-7). Individual outcomes can favor a different report even though the expected Brier score and logarithmic loss are uniquely minimized at $p=0.7$**.

The $Y=0$ loss curves favor $p=0$, and the $Y=1$ loss curves favor $p=1$. Their weighted average, with weights $0.3$ and $0.7$, favors $p=0.7$. Choosing a report after observing $Y$ would use information unavailable at forecast time. Even an average loss on a finite dataset can rank an honest forecast below a competing forecast through outcome variation; [strict propriety](#strictly-proper-scoring-rule) guarantees the ranking in [expected value](expected-value.md) under the specified information and true [predictive distribution](probability-distribution.md#predictive-distribution).

##### Brier score

↑ **Parent:** [Strictly proper scoring rule](#strictly-proper-scoring-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brier_score)

The binary [Brier score](#brier-score) applies [squared-error loss](#squared-error-loss) to a reported success [probability](probability-theory.md#probability) $p$ and the observed indicator $y\in\{0,1\}$. It is a loss, so smaller is better. Its values lie in $[0,1]$: predicting the outcome with certainty gives zero, while assigning it zero [probability](probability-theory.md#probability) gives one. Unlike the [logarithmic scoring rule](#logarithmic-scoring-rule) loss, the binary [Brier score](#brier-score) remains bounded even for a confidently wrong forecast.

For a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with true success [probability](probability-theory.md#probability) $q$, averaging the two squared losses gives

$$
\mathbb E_q[(p-Y)^2]=q(p-1)^2+(1-q)p^2=(p-q)^2+q(1-q).
$$

The report controls only $(p-q)^2$; the remaining term is the [variance](variance.md) of the [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution). Consequently the [Brier score](#brier-score) is a [strictly proper scoring rule](#strictly-proper-scoring-rule). At $q=0.7$, the expected loss is $(p-0.7)^2+0.21$, with unique minimum $0.21$ at $p=0.7$. Reporting $p=0.2$ instead gives expected loss $0.46$, despite its better loss on the particular outcome $Y=0$ above.

For several possible categories, the [Brier score](#brier-score) sums the squared differences between reported [probabilities](probability-theory.md#probability) and observed category indicators. With two categories that sum is $2(p-y)^2$, so its numerical values are twice the binary convention used here, with the same optimizing report. Brier's original [Verification of Forecasts Expressed in Terms of Probability (1950), equation (2)](https://www.u-cursos.cl/ingenieria/2025/1/CI71C/1/material_docente/bajar?bajar=1&id=8745481) averages these category-sum losses over forecasts. [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others) (Section 3.1, Example 1, and Table 1) gives the category-sum and binary forms as negative rewards; negating them gives the losses described here.

##### Logarithmic scoring rule

↑ **Parent:** [Strictly proper scoring rule](#strictly-proper-scoring-rule)

The [logarithmic scoring rule](#logarithmic-scoring-rule) rewards the [natural logarithm](calculus.md#natural-logarithm) of the reported [probability mass](probability-distribution.md#probability-mass) or [probability density](wave-function.md#probability-density) at the observed outcome. The title uses the reward convention. For a binary report $p$, its negative is the [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss):

$$
L_{\log}(p,y)=-y\ln p-(1-y)\ln(1-p),\qquad 0<p<1.
$$

For $y=1$ this is $-\ln p$; for $y=0$ it is $-\ln(1-p)$. At an endpoint, use these outcome-specific forms: assigning zero [probability](probability-theory.md#probability) to the outcome incurs infinite loss, while assigning it [probability](probability-theory.md#probability) one gives zero. The [natural logarithm](calculus.md#natural-logarithm) therefore makes a confidently wrong binary forecast far more costly than the bounded [Brier score](#brier-score) does.

Under the stipulated [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with $q=0.7$, the expected logarithmic loss is

$$
\mathbb E_{0.7}[L_{\log}(p,Y)]=-0.7\ln p-0.3\ln(1-p).
$$

Its unique minimum is at $p=0.7$, where the expected loss is approximately $0.610864$. At $p=0.2$ it is approximately $1.193550$. More generally, the excess expected logarithmic loss over truthful reporting is the [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) in the order true law first, reported law second:

$$
\mathbb E_q[L_{\log}(p,Y)]-\mathbb E_q[L_{\log}(q,Y)]
=q\ln\frac qp+(1-q)\ln\frac{1-q}{1-p}
=D_{\rm KL}\!\left(\operatorname{Bernoulli}(q)\Vert\operatorname{Bernoulli}(p)\right).
$$

For $0<q<1$, this [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) is nonnegative and vanishes only at $p=q$, explaining why the [logarithmic scoring rule](#logarithmic-scoring-rule) is a [strictly proper scoring rule](#strictly-proper-scoring-rule). The same [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) identity applies to [probability density functions](continuous-probability-distribution.md#probability-density-function) relative to a common [measure](measure.md) when the truthful expected [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss) is finite and the comparison [expected value](expected-value.md) is well defined.[Section 3.1, Example 3, and Section 4.1](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others) For sequential forecasts, the existing [prequential log score identity](#prequential-log-score-identity) explains how logarithmic rewards add over observations.

###### Prequential log score identity

↑ **Parent:** [Logarithmic scoring rule](#logarithmic-scoring-rule)

The probability chain rule makes a sum of sequential predictive log scores equal the log [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence) when the forecasts are coherent Bayesian one-step predictions under proper priors. Differences of total scores are therefore log [Bayes factors](bayesian-statistics.md#bayes-factor).

## Statistical degrees of freedom

↑ **Parent:** [Statistical inference](statistical-inference.md)

The number of free dimensions remaining after specified constraints often determines a reference [sampling distribution](statistical-modelling.md#sampling-distribution). In a full-rank [normal linear model](normal-linear-model.md) with $n$ observations and $p$ mean coefficients, the residual space has dimension $n-p$. A regular nested [likelihood-ratio test](statistical-hypothesis-test.md#likelihood-ratio-test) instead uses the difference in free [statistical parameter](statistical-model.md#statistical-parameter) dimensions. Boundary constraints may invalidate this regular calibration.

## Statistic

↑ **Parent:** [Statistical inference](statistical-inference.md)

A statistic is a measurable function of observed data whose definition does not involve an unknown parameter. It may be scalar or vector valued. [Sufficient statistics](probability-and-statistics.md#sufficient-statistic) summarize all information about a parameter in the conditional-distribution sense.

### Complete statistic

↑ **Parent:** [Statistic](#statistic)

A statistic is complete for a parameter family if the displayed implication holds for every measurable $g$ integrable under all parameter values. This property does not itself assert sufficiency; a [complete sufficient statistic](probability-and-statistics.md#complete-sufficient-statistic) has both properties. A nonconstant unbiased estimator of a known constant provides a direct obstruction to completeness.

#### Boundedly complete statistic

↑ **Parent:** [Complete statistic](#complete-statistic)

Bounded completeness requires the defining implication for a [complete statistic](#complete-statistic) only for bounded measurable functions. Completeness implies it, but the converse need not hold. If a [sufficient statistic](probability-and-statistics.md#sufficient-statistic) $T$ gives a parameter-independent event probability $c$ and the conditional probability $S(T)$ of that event is nonconstant, then $S-c$ is a bounded zero-mean obstruction to bounded completeness.

## Meta-analysis

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meta-analysis)

A meta-analysis combines statistical evidence from several studies addressing a common estimand. It may assume a shared effect or use a [random-effects meta-analysis](#random-effects-meta-analysis) to represent between-study variation. [Inverse-variance weighted means](statistical-modelling.md#inverse-variance-weighted-mean) combine [independent](random-variable.md#independent-random-variables) effect estimates when their [variances](variance.md) are known or estimated; differences in study validity and [effect modifiers](causal-inference.md#effect-modifier) require substantive assessment, not just weighting.

### Subgroup analysis in meta-analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

Divide studies by a specified characteristic and estimate an effect in each subgroup, then test the difference using an [independent subgroup contrast in meta-analysis](#independent-subgroup-contrast-in-meta-analysis) or an appropriate interaction model. The test of a between-group difference is distinct from separate tests against no effect within each group. Exploratory splits can be affected by [multiple testing](statistical-hypothesis-test.md#multiple-hypothesis-testing) and by [confounding](causal-inference.md#confounding) between study characteristics.

### Forest plot

↑ **Parent:** [Meta-analysis](#meta-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forest_plot)

A forest plot shows each study's effect estimate and [confidence interval](#confidence-interval), together with a pooled estimate when appropriate. A vertical null-effect line allows comparison on a common scale. For an [odds ratio](statistical-modelling.md#odds-ratio) the null is one and a logarithmic axis treats reciprocal ratios symmetrically; marker areas commonly encode study weights.

### Funnel plot

↑ **Parent:** [Meta-analysis](#meta-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Funnel_plot)

A [funnel plot](#funnel-plot) displays study effect estimates against a measure of their precision, often [standard error](#standard-error) increasing down the vertical axis. Under a common-effect model, imprecise estimates spread more widely around the effect. Asymmetry is evidence of a [small-study effect](#small-study-effect) and can be consistent with [publication bias](#publication-bias), but it has other possible explanations.

#### Small-study effect

↑ **Parent:** [Funnel plot](#funnel-plot)

A [small-study effect](#small-study-effect) is a systematic relationship between study precision or size and estimated effect. It may result from selective publication, design differences, effect modification or other heterogeneity. A regression of effect on its [standard error](#standard-error) tests one such relationship; it does not by itself determine which mechanism generated it.

### Publication bias

↑ **Parent:** [Meta-analysis](#meta-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Publication_bias)

Publication bias arises when the availability of studies depends on the results, such as their significance, magnitude or direction. A [meta-analysis](#meta-analysis) of the available studies can then differ systematically from one including all eligible evidence. [Funnel plot](#funnel-plot) asymmetry can motivate investigation but does not establish this mechanism; heterogeneity and other [small-study effects](#small-study-effect) can also cause asymmetry.

#### Selection model for publication bias

↑ **Parent:** [Publication bias](#publication-bias)

A selection model combines a distribution for all study results with a [probability](probability-theory.md#probability) $\pi(y)$ that a result becomes available. The observed distribution is reweighted by this [probability](probability-theory.md#probability) and renormalized. Assumed or estimated selection mechanisms permit [sensitivity analysis](probability-and-statistics.md#sensitivity-analysis) of a [meta-analysis](#meta-analysis), but unavailable results generally prevent a fully assumption-free correction.

##### Odds under at-least-one-positive selection

↑ **Parent:** [Selection model for publication bias](#selection-model-for-publication-bias)

For $n$ studies conditionally independent given the truth of one relationship, the event that at least one is positive has probability $1-\beta^n$ under the alternative and $1-(1-\alpha)^n$ under the null. Its [Bayes factor](bayesian-statistics.md#bayes-factor) therefore gives the displayed [posterior odds](bayesian-statistics.md#posterior-odds). For interior error probabilities these tend back to the [prior odds](bayesian-statistics.md#prior-odds) $R$. If power exceeds size, the Bayes factor decreases to one: the quotient of geometric sums is a weighted average of decreasing powers $[\beta/(1-\alpha)]^k$.

This result concerns the coarsened selection event. Full observed results instead multiply their individual [Bayes factors](bayesian-statistics.md#bayes-factor), and concordant evidence can accumulate without this bound. It is a useful example of information discarded by [publication bias](#publication-bias).

#### Trim and fill

↑ **Parent:** [Publication bias](#publication-bias)

Trim and fill estimates missing studies from [funnel plot](#funnel-plot) asymmetry by trimming extreme studies to locate a centre and filling in counterparts on the less represented side. The adjusted [meta-analysis](#meta-analysis) includes these imputed estimates. Its interpretation depends on a symmetry model for missing evidence; it is not a guarantee that genuine [publication bias](#publication-bias) has been removed.

### Independent subgroup contrast in meta-analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

For [independent](random-variable.md#independent-random-variables) subgroup estimates $\widehat\mu_1,\widehat\mu_2$ with [variances](variance.md) $v_1,v_2$, the null contrast has [Wald statistic](statistical-hypothesis-test.md#wald-test) $Z=(\widehat\mu_1-\widehat\mu_2)/\sqrt{v_1+v_2}$. If evidence overlaps, include minus twice the [covariance](variance.md#covariance) in the contrast variance. A nonsignificant comparison is not proof of equivalence.

### Within-study bias

↑ **Parent:** [Meta-analysis](#meta-analysis)

Systematic displacement of an individual study estimate caused by design, conduct, analysis or selective reporting. Combining estimates can reduce random error without reducing this bias. [Bias-adjusted meta-analysis](#bias-adjusted-meta-analysis) and analyses restricted or stratified by relevant bias domains can assess its impact.

#### Bias-adjusted meta-analysis

↑ **Parent:** [Within-study bias](#within-study-bias)

Model study estimates as noisy versions of the target effects plus study-specific biases. External information or sensitivity parameters describe those biases and their uncertainty. Removing an assumed bias without propagating its uncertainty overstates precision; observed study data alone generally do not identify the adjustment.

### Fixed-effect meta-analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

A common-effect synthesis treats study estimates as estimates of one shared effect. For [independent](random-variable.md#independent-random-variables) approximately unbiased estimates $y_i$ with [variances](variance.md) $v_i$, use $\widehat\mu=\sum_iw_iy_i/\sum_iw_i$ with $w_i=v_i^{-1}$. This model does not accommodate additional [between-study heterogeneity](#between-study-heterogeneity).

<h4 id="mantel-haenszel-pooled-odds-ratio">Mantel–Haenszel pooled odds ratio</h4>

↑ **Parent:** [Fixed-effect meta-analysis](#fixed-effect-meta-analysis)

For independent two-by-two tables with counts $a_i,b_i,c_i,d_i$ and total $n_i$, the Mantel–Haenszel pooled [odds ratio](statistical-modelling.md#odds-ratio) is the displayed ratio of sums. When all $b_ic_i>0$, it is also the weighted arithmetic mean of study odds ratios with weights $b_ic_i/n_i$. These differ from inverse estimated [variance](variance.md) weights for [log odds ratios](statistical-modelling.md#log-odds-ratio). Both constructions can represent a [fixed-effect meta-analysis](#fixed-effect-meta-analysis), but they should not be silently interchanged when interpreting a supplied plot.

### Leave-one-study-out influence analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

Refit a [meta-analysis](#meta-analysis) after deleting each study, comparing fitted effects, uncertainty and heterogeneity to the full fit. For fixed weights $w_i>0$, total weight $W$ and weighted effect $\widehat\mu$, direct subtraction of the two weighted means gives $\widehat\mu-\widehat\mu_{(-i)}=w_i(y_i-\widehat\mu)/(W-w_i)$. Re-estimating heterogeneity additionally measures influence through the weights. This is a sensitivity diagnostic, not an automatic rule for removing discordant studies.

### Random-effects meta-analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

For [independent](random-variable.md#independent-random-variables) study estimates $y_i$ with within-study [variances](variance.md) $v_i$, a usual approximate model is $y_i\mid\delta_i\sim N(\delta_i,v_i)$ and $\delta_i\sim N(\mu,\tau^2)$. Its [marginal distribution](probability-distribution.md#marginal-distribution) is $N(\mu,v_i+\tau^2)$, so for fixed heterogeneity $\tau^2$ the [inverse-variance weighted mean](statistical-modelling.md#inverse-variance-weighted-mean) uses weights $(v_i+\tau^2)^{-1}$. Here $\mu$ describes the mean effect across comparable studies; $\tau^2$ represents between-study variation. Estimation and uncertainty for heterogeneity are essential, especially with few studies.

#### Student t random-effect model

↑ **Parent:** [Random-effects meta-analysis](#random-effects-meta-analysis)

A [Student t random-effect model](#student-t-random-effect-model) assigns [Student's t-distributions](continuous-probability-distribution.md#student-s-t-distribution) to exchangeable study effects, allowing heavier tails than a [normal distribution](probability-distribution.md#normal-distribution) hierarchy. An equivalent [Gaussian scale mixture](statistical-modelling.md#gaussian-scale-mixture) is $\lambda_j\sim\chi^2_\nu$, $\beta_j\mid\lambda_j,\mu,\psi\sim N(\mu,\nu\psi^2/\lambda_j)$, with independent latent draws. For $\nu>2$ the [variance](variance.md) is $\nu\psi^2/(\nu-2)$, so $\psi$ is a scale rather than a [standard deviation](variance.md#standard-deviation). Small latent precisions weaken shrinkage for atypical studies while retaining [partial pooling](bayesian-statistics.md#partial-pooling) for the rest.

#### Between-study heterogeneity

↑ **Parent:** [Random-effects meta-analysis](#random-effects-meta-analysis)

Variation in the underlying study effects, additional to sampling error. The usual normal [random-effects meta-analysis](#random-effects-meta-analysis) models it by a between-study [variance](variance.md) $\tau^2$. It can reflect effect modification, design differences or [within-study bias](#within-study-bias); it is not automatically a biological treatment difference.

##### Meta-regression

↑ **Parent:** [Between-study heterogeneity](#between-study-heterogeneity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meta-regression)

Meta-regression relates study effect estimates to study-level explanatory variables. A common [random-effects meta-analysis](#random-effects-meta-analysis) extension is $y_i=\alpha+\beta x_i+u_i+\varepsilon_i$, where $\operatorname{Var}(u_i)=\tau^2$ and $\operatorname{Var}(\varepsilon_i)=v_i$. For [log odds ratios](statistical-modelling.md#log-odds-ratio), $e^\beta$ is a ratio of underlying odds ratios per unit of $x$. Few studies, correlated design changes and exploratory variable selection limit interpretation; a study-level association does not identify an individual-level [causal effect](causal-inference.md#causal-effect). The interpretation of study-level predictors is also discussed in [the Cochrane methods handbook, section 10.11](https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10).

##### Prior calibration for normal random-effect range

↑ **Parent:** [Between-study heterogeneity](#between-study-heterogeneity)

For $J\ge2$ conditionally independent effects $\beta_j\sim N(\mu,\tau^2)$, each pair difference has [normal distribution](probability-distribution.md#normal-distribution) $N(0,2\tau^2)$. With $m=\binom J2$, an upper bound $A=R/[\sqrt2\,\Phi^{-1}(1-\varepsilon/(2m))]$ on $\tau$ ensures, by the [union bound](probability-inequality.md#boole-s-inequality), that $\mathbb P(\max_j\beta_j-\min_j\beta_j>R)\le\varepsilon$. Any proper scale [prior distribution](bayesian-statistics.md#prior-probability) supported on $(0,A)$ preserves this bound after averaging. This is conservative simultaneous calibration, rather than the weaker statement about one selected pair. For [log odds ratios](statistical-modelling.md#log-odds-ratio), a bound $R$ corresponds to a ratio-of-odds-ratios bound $e^R$.

##### I-squared statistic

↑ **Parent:** [Between-study heterogeneity](#between-study-heterogeneity)

For $Q>0$ and $m$ studies, $I^2=\max\{0,[Q-(m-1)]/Q\}$. Usually reported as a percentage, it describes excess variation relative to the observed variation on this heterogeneity scale. It is not a proportion of studies with different effects or a proportion of an individual clinical outcome.

<h5 id="dersimonian-laird-estimator">DerSimonian–Laird estimator</h5>

↑ **Parent:** [Between-study heterogeneity](#between-study-heterogeneity)

For $m$ studies let $w_i=v_i^{-1}$, $W=\sum_iw_i$, $C=W-\sum_iw_i^2/W$, and let $Q$ be [Cochran's Q statistic](#cochran-s-q-statistic). The moment estimate is $\widehat\tau^2=\max\{0,[Q-(m-1)]/C\}$ when $C>0$. It estimates the [variance](variance.md) of underlying study effects, not their sampling variance.

<h5 id="cochran-s-q-statistic">Cochran's Q statistic</h5>

↑ **Parent:** [Between-study heterogeneity](#between-study-heterogeneity)

With fixed inverse-variance weights and weighted mean $\widehat\mu$, $Q=\sum_iw_i(y_i-\widehat\mu)^2$. Under a common-effect normal model with $m$ independent estimates and known variances it has a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $m-1$ degrees of freedom. Estimated variances make this calibration approximate.

### Network meta-analysis

↑ **Parent:** [Meta-analysis](#meta-analysis)

A network meta-analysis jointly compares several treatments using a [graph](graph.md) of direct [randomized controlled trials](causal-inference.md#randomized-controlled-trial) and [indirect treatment comparisons](#indirect-treatment-comparison). If effects are measured relative to a reference treatment, consistency means $\delta_{ij}=\delta_{i0}-\delta_{j0}$. A connected [graph](graph.md) identifies all relative effects under that model. [Transitivity in network meta-analysis](#transitivity-in-network-meta-analysis) is the substantive comparability assumption supporting these relations; inconsistency can be assessed when the network has loops.

#### Indirect treatment comparison

↑ **Parent:** [Network meta-analysis](#network-meta-analysis)

For [independent](random-variable.md#independent-random-variables) studies comparing treatments $A$ and $B$ to common control $C$, a consistent [log odds ratio](statistical-modelling.md#log-odds-ratio) comparison uses $\widehat\delta_{AB}=\widehat\delta_{AC}-\widehat\delta_{BC}$, with [variance](variance.md) $v_{AC}+v_{BC}$. This follows from subtracting two estimates of additive effects relative to the same reference. With overlapping evidence, subtract twice their [covariance](variance.md#covariance). Causal comparability across the studies is supplied by [transitivity in network meta-analysis](#transitivity-in-network-meta-analysis), not by the [variance](variance.md) calculation.

##### Transitivity in network meta-analysis

↑ **Parent:** [Indirect treatment comparison](#indirect-treatment-comparison)

Transitivity requires the studies of different treatment comparisons to be sufficiently comparable in distributions of [effect modifiers](causal-inference.md#effect-modifier), outcome definitions and other design features to support an [indirect treatment comparison](#indirect-treatment-comparison) in one target population. For example, a treatment that works differently by disease severity cannot safely be compared indirectly across trials with systematically different severity distributions. Statistical consistency is an implication of suitable transitivity and modeling assumptions, not a substitute for assessing them.

## Confidence region

↑ **Parent:** [Statistical inference](statistical-inference.md)

A random set of parameter values with specified repeated-sampling coverage: $\mathbb P_\theta\{\theta\in C(X)\}\geq1-\alpha$ for every permitted $\theta$. Exact coverage, asymptotic coverage and pointwise versus uniform validity must be distinguished. A [confidence interval](#confidence-interval) is the scalar interval case.

### Confidence band

↑ **Parent:** [Confidence region](#confidence-region)

A confidence band provides simultaneous bounds on an unknown function over its entire index set. Its coverage event is the intersection over all indices, unlike separate pointwise [confidence intervals](#confidence-interval). For a continuous [cumulative distribution function](probability-distribution.md#cumulative-distribution-function), the [Kolmogorov-Smirnov theorem](#kolmogorov-smirnov-theorem) gives an asymptotic band $F_n\pm c_\alpha/\sqrt n$, clipped to $[0,1]$, where $c_\alpha$ is a $(1-\alpha)$-quantile of the absolute [Brownian bridge](brownian-motion.md#brownian-bridge) maximum. The simultaneous event equals $\sqrt n\|F_n-F\|_\infty\leq c_\alpha$, so [convergence in distribution](convergence-of-random-variables.md#convergence-in-distribution) at this continuity point proves coverage tending to $1-\alpha$.

#### Kolmogorov-Smirnov confidence band

↑ **Parent:** [Confidence band](#confidence-band)

For independent observations from a continuous distribution function, the [probability integral transform](probability-distribution.md#probability-integral-transform) makes the [Kolmogorov-Smirnov statistic](#kolmogorov-smirnov-statistic) distribution-free. Choose $c_{n,\alpha}$ from its uniform-sample distribution to have probability $1-\alpha$ of not exceeding that critical value. Clipping the empirical distribution plus/minus this value to the unit interval gives simultaneous coverage at every argument. This is a band for the entire distribution, rather than separate pointwise intervals.

// Target: statistical-modelling.bigb

### Confidence ellipsoid

↑ **Parent:** [Confidence region](#confidence-region)

An ellipsoidal [confidence region](#confidence-region) defined by a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) $A$ and a calibrated threshold $c$. For a known-covariance [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) sample, $A=n\Sigma^{-1}$ and the $1-\alpha$ quantile of the [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $d$ [degrees of freedom](classical-mechanics.md#degree-of-freedom) give exact coverage for the $d$-dimensional mean.

## Statistical sample

↑ **Parent:** [Statistical inference](statistical-inference.md)

A collection of observed random variables used to infer a [statistical model](statistical-model.md) or its parameters. A common assumption is that the observations are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables); dependence must otherwise be included in the model. Its randomness induces the [sampling distribution](statistical-modelling.md#sampling-distribution) of a statistic.

### Normal sample

↑ **Parent:** [Statistical sample](#statistical-sample)

A collection of independent identically distributed [normal random variables](probability-distribution.md#gaussian-random-variable). Orthogonal coordinates in the standardized [Gaussian vector](probability-and-statistics.md#gaussian-random-vector) separate the [sample mean](variance.md#sample-mean) from the residual sum of squares, proving their independence and giving the normal and [chi-squared distributions](probability-distribution.md#chi-squared-distribution) used for exact inference.

## Semiparametric statistics

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semiparametric_statistics)

Semiparametric statistics studies models with a finite-dimensional target parameter and an infinite-dimensional nuisance component.

### Adaptivity to an unknown covariate distribution

↑ **Parent:** [Semiparametric statistics](#semiparametric-statistics)

If the parametric [score function](statistical-modelling.md#informant-function) has zero [conditional expectation](measure-theory.md#conditional-expectation) given a [covariate](statistical-model.md#covariate) $X$, it is orthogonal to the centered [functions](function.md) of $X$ that form the covariate-density [nuisance tangent space](#nuisance-tangent-space). Its [efficient score](#efficient-score) then equals its parametric [score function](statistical-modelling.md#informant-function), and the unknown covariate distribution causes no loss of [Fisher information](statistical-modelling.md#fisher-information-matrix). This applies to [Gaussian regression scores](statistical-modelling.md#gaussian-regression-score) and more generally to regular conditional models with unrestricted covariate distribution and no additional nuisance components.

### Nuisance tangent space

↑ **Parent:** [Semiparametric statistics](#semiparametric-statistics)

The nuisance tangent space is the closed linear span of [score functions](statistical-modelling.md#informant-function) from [statistical paths](statistical-model.md#statistical-path) that vary the [nuisance parameter](statistical-model.md#nuisance-parameter) while fixing the target [statistical parameter](statistical-model.md#statistical-parameter). It is a [closed subspace of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space) inside $L^2_0(P)$. Removing its component from a parametric [score function](statistical-modelling.md#informant-function) leaves the information that nuisance variation cannot imitate.

#### Mean-preserving error tangent space

↑ **Parent:** [Nuisance tangent space](#nuisance-tangent-space)

For independent-error regression with a zero-mean error, bounded density paths $f_t=f(1+t\gamma)$ must preserve both normalization and the first [moment](expected-value.md#moment). Their [score functions](statistical-modelling.md#informant-function) therefore satisfy two constraints. When $0<E_f\varepsilon^2<\infty$, truncation followed by two small bounded moment corrections shows these scores are dense in the displayed [closed subspace of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space). By [independence](random-variable.md#independent-random-variables), they are orthogonal to every $\varepsilon\psi(X)$ with $\psi\in L^2(v)$. The same constraints apply to other paths only under regularity permitting differentiation of the first [moment](expected-value.md#moment).

#### Efficient score

↑ **Parent:** [Nuisance tangent space](#nuisance-tangent-space)

The efficient score is the residual after [orthogonal projection](hilbert-space.md#orthogonal-projection) of the parametric [score function](statistical-modelling.md#informant-function) onto the [nuisance tangent space](#nuisance-tangent-space). It is centered and orthogonal to every nuisance direction. Its squared [L2 norm](real-analysis.md#l2-norm) is the [efficient information](#efficient-information).

##### Efficient score in independent-error regression

↑ **Parent:** [Efficient score](#efficient-score)

With unknown independent covariate and centered error distributions, take the regular [mean-preserving error tangent space](#mean-preserving-error-tangent-space), let $h=\partial_\theta g_\theta$, $\rho=-f'/f$ and $\tau^2=E_f\varepsilon^2>0$. Under $E_f\rho=0$, $E_f(\varepsilon\rho)=1$ and finite second [moments](expected-value.md#moment), [orthogonal projection](hilbert-space.md#orthogonal-projection) removes $(E_vh)(\rho-\varepsilon/\tau^2)$ from $h\rho$. Thus the [efficient score](#efficient-score) and [efficient information](#efficient-information) are $\widetilde\ell=(h-E_vh)\rho+(E_vh)\varepsilon/\tau^2$ and $\widetilde I=\operatorname{Var}_v(h)E_f\rho^2+(E_vh)^2/\tau^2$. The reduction to $h\varepsilon/\tau^2$ is valid for a [normal distribution](probability-distribution.md#normal-distribution) of errors or for constant $h$, but need not hold otherwise. Centered covariates and [logistic distribution](statistical-modelling.md#logistic-distribution) errors give the counterexample $\widetilde\ell=X\tanh(\varepsilon/2)$.

##### Efficient-score projection identity

↑ **Parent:** [Efficient score](#efficient-score)

The decomposition $\dot\ell=\Pi_{\mathcal N}\dot\ell+\widetilde\ell$ is orthogonal. Taking the [inner product](inner-product.md) with the [efficient score](#efficient-score) gives $P(\dot\ell\widetilde\ell)=\widetilde I$. Centering of the [efficient score](#efficient-score) follows because the [nuisance tangent space](#nuisance-tangent-space) and the parametric [score function](statistical-modelling.md#informant-function) lie in the closed [mean-zero L2 space](measure-theory.md#mean-zero-l2-space).

##### Efficient information

↑ **Parent:** [Efficient score](#efficient-score)

The efficient information for a scalar target [statistical parameter](statistical-model.md#statistical-parameter) is the squared [L2 norm](real-analysis.md#l2-norm) of its [efficient score](#efficient-score). It cannot exceed the parametric [Fisher information](statistical-modelling.md#fisher-information-matrix), by the [Pythagorean theorem in an inner-product space](inner-product.md#pythagorean-theorem-in-an-inner-product-space). It can vanish when first-order target variation can be reproduced by nuisance variation.

### Semiparametric estimator

↑ **Parent:** [Semiparametric statistics](#semiparametric-statistics)

A semiparametric estimator targets a finite-dimensional parameter while estimating or otherwise accommodating an infinite-dimensional nuisance component.

### Partially linear model

↑ **Parent:** [Semiparametric statistics](#semiparametric-statistics)

A partially linear model combines a linear coefficient with an unrestricted nuisance function, for example $\mathbb E[Y\mid A,X]=\beta A+g(X)$.

## Fisher consistency

↑ **Parent:** [Statistical inference](statistical-inference.md)

A statistical functional is Fisher-consistent for a parameter when evaluating it at the model distribution returns that parameter.

## Scale estimator

↑ **Parent:** [Statistical inference](statistical-inference.md)

A scale estimator measures the spread of a distribution and transforms proportionally when all observations are multiplied by a positive constant.

## Consistency (statistics)

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Consistency_(statistics))

A statistical estimator is consistent when it converges in probability to the target parameter as the sample size tends to infinity.

## Plug-in estimator

↑ **Parent:** [Statistical inference](statistical-inference.md)

A plug-in estimator replaces unknown components of a statistical functional by estimators and evaluates the same functional at those fitted components.

<h2 id="assouad-s-lemma">Assouad's lemma</h2>

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Assouad's_lemma)

Assouad's lemma lower-bounds minimax risk by embedding a Hamming hypercube of separated parameters whose neighboring statistical experiments are difficult to distinguish.

### Assouad hypercube

↑ **Parent:** [Assouad's lemma](#assouad-s-lemma)

An Assouad hypercube is a family $(P_\omega,\theta_\omega)_{\omega\in\{0,1\}^k}$ in which loss separates proportionally to Hamming distance while distributions at neighboring vertices remain close in total variation.

## Nonparametric statistics

↑ **Parent:** [Statistical inference](statistical-inference.md)

[This section is present in another page, follow this link to view it.](nonparametric-statistics.md)

## Robust statistics

↑ **Parent:** [Statistical inference](statistical-inference.md)

[This section is present in another page, follow this link to view it.](robust-statistics.md)

## Kolmogorov-Smirnov theorem

↑ **Parent:** [Statistical inference](statistical-inference.md)

For an empirical distribution function based on an independent sample from a continuous distribution $F$,

$$
\sqrt n\sup_x|\widehat F_n(x)-F(x)|
\xrightarrow{d}\sup_{0\leq t\leq1}|B(t)|,
$$

where $B$ is a [Brownian bridge](brownian-motion.md#brownian-bridge).

This limit calibrates the [Kolmogorov-Smirnov test](#kolmogorov-smirnov-test); the test compares an empirical distribution with its null distribution using the supremum discrepancy.

## Standard error

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_error)

The standard error of an estimator is the standard deviation of its sampling distribution, or an estimate of that standard deviation.

## Efficient unbiased estimator implies exponential family

↑ **Parent:** [Statistical inference](statistical-inference.md)

In a regular one-parameter statistical model, equality in the [Cramér-Rao lower bound](statistical-modelling.md#cramer-rao-bound) for an unbiased estimator $T$ implies the [score function](statistical-modelling.md#informant-function) $\partial_\theta\log f(x;\theta)=I(\theta)(T(x)-\theta)$. Integrating in the parameter on a regular connected interval gives $f(x;\theta)=h(x)\exp(A(\theta)T(x)-B(\theta))$, with $A'=I$ and $B'=\theta I$. Thus efficiency for every parameter value forces an [exponential family](exponential-family.md) structure, under the usual common-support and differentiation assumptions.

## Wilks theorem

↑ **Parent:** [Statistical inference](statistical-inference.md)

Under regularity conditions, minus twice the logarithm of a generalized likelihood ratio converges under the null hypothesis to a chi-squared distribution whose degrees of freedom equal the difference in parameter dimensions.

## Chi-squared test

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chi-squared_test)

A [chi-squared test](#chi-squared-test) rejects a null hypothesis for a statistic whose null distribution is a chi-squared law, exactly or asymptotically. Pearson tests compare observed and expected counts; both goodness-of-fit and [chi-squared tests of independence](#chi-squared-test-of-independence) are instances.

### Chi-squared comparison of a calibrated attenuation model

↑ **Parent:** [Chi-squared test](#chi-squared-test)

Suppose $N_0$ is independently calibrated and counts $y_i$ have predicted means $\mu_i=t_iN_0e^{-bn_i}$ under a specified candidate $b$. For independent sufficiently large Poisson counts, the [Pearson chi-squared statistic](generalized-linear-model.md#pearson-chi-squared-statistic) is $Q=\sum_i(y_i-\mu_i)^2/\mu_i$. With no parameters fitted to these test counts, its approximate reference [chi-squared distribution](probability-distribution.md#chi-squared-distribution) has one degree of freedom per observation. Fitting a continuous $b$ to the same data instead removes one residual degree of freedom. Replacing the denominators by observed counts is a common estimated-error approximation but can behave badly at small counts.

Calibration uncertainty $\sigma_0$ also induces correlated prediction errors. First-order [propagation of uncertainty](wave-equation.md#propagation-of-uncertainty) gives

$$
\operatorname{Cov}(y_i-\mu_i,y_j-\mu_j)\simeq\delta_{ij}\mu_i+t_it_j e^{-b(n_i+n_j)}\sigma_0^2.
$$

A generalized quadratic form uses this [covariance matrix](variance.md#covariance-matrix). For sparse counts use the [Poisson deviance](generalized-linear-model.md#poisson-deviance) or the full count likelihood, with simulation if a calibrated goodness-of-fit probability is required. Choosing a range after inspecting residuals also affects formal test calibration; a physically specified signal-dominated range is preferable when applying a pure attenuation model.

### Compatibility of independent lifetime measurements

↑ **Parent:** [Chi-squared test](#chi-squared-test)

If two independent approximately Gaussian [mean lifetime](relativistic-quantum-field.md#mean-lifetime-physics) estimates have known [standard deviations](variance.md#standard-deviation) $s_1,s_2$, equality of their true lifetimes implies that their difference has mean zero and [variance](variance.md) $s_1^2+s_2^2$. Its squared standardized difference therefore has a one-degree-of-freedom [chi-squared distribution](probability-distribution.md#chi-squared-distribution), giving the statistic in the title. A chosen significance threshold converts its upper-tail [P-value](statistical-hypothesis-test.md#p-value) into a compatibility decision.

Testing a fitted decay curve against a fixed numerical lifetime is a different question: that test does not include the external measurement uncertainty. Comparing the two experiments requires both uncertainties or a joint likelihood with a common lifetime. Correlated estimates replace the denominator by $s_1^2+s_2^2-2\operatorname{Cov}(\widehat\tau_1,\widehat\tau_2)$.

### Chi-squared test of independence

↑ **Parent:** [Chi-squared test](#chi-squared-test)

For an $r$ by $c$ contingency table, Pearson's sum of squared observed-minus-fitted counts divided by fitted counts is asymptotically $\chi^2_{(r-1)(c-1)}$ under independence.

## Statistical decision theory

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_decision_theory)

Statistical decision theory compares decision rules through the expected loss they incur under each parameter value.

### Statistical invariance principle

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

If sample transformations preserve the model and both hypotheses, the invariance principle restricts attention to tests whose decisions are unchanged by those transformations. Such tests are functions of a [maximal invariant](statistical-model.md#maximal-invariant). In estimation, the analogous requirement is [equivariance](group-action.md#equivariant-map), accompanied by an invariant [loss function](foundations-of-mathematics.md#loss-function) so that risks transform compatibly. The principle respects symmetries; it does not by itself prove optimality among all unrestricted procedures.

### Cost-effectiveness analysis

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cost-effectiveness_analysis)

[Cost-effectiveness analysis](#cost-effectiveness-analysis) compares interventions through their costs and effects measured in a common outcome unit. Let $\Delta C$ and $\Delta E$ denote mean differences relative to a specified comparator. A positive effect increment with nonpositive cost increment gives dominance; the reverse signs give a dominated intervention. A tradeoff in the positive-positive quadrant requires a willingness-to-pay threshold per outcome unit. [Randomized controlled trials](causal-inference.md#randomized-controlled-trial) can estimate these differences, but their joint [sampling distribution](statistical-modelling.md#sampling-distribution) is needed to express uncertainty. Outcome units, time horizon and costing perspective must be specified; a survival-day increment is not automatically a quality-adjusted outcome.

#### Incremental net monetary benefit

↑ **Parent:** [Cost-effectiveness analysis](#cost-effectiveness-analysis)

At a specified willingness-to-pay threshold $\lambda$, the [incremental net monetary benefit](#incremental-net-monetary-benefit) is the value of the effect increment minus the cost increment. It avoids dividing by a potentially near-zero or negative effect estimate. For estimates with [variances](variance.md) $v_E,v_C$ and [covariance](variance.md#covariance) $v_{CE}$, its estimated [variance](variance.md) is $\lambda^2v_E+v_C-2\lambda v_{CE}$. A [normal approximation](convergence-of-random-variables.md#normal-approximation) therefore gives a [confidence interval](#confidence-interval) directly on the net-benefit scale. The economic sign criterion does not require a positive effect increment.

##### Cost-effectiveness acceptability curve

↑ **Parent:** [Incremental net monetary benefit](#incremental-net-monetary-benefit)

A [cost-effectiveness acceptability curve](#cost-effectiveness-acceptability-curve) displays the probability of positive [incremental net monetary benefit](#incremental-net-monetary-benefit) as a function of the willingness-to-pay threshold. Under a [posterior distribution](bayesian-statistics.md#bayesian-posterior) this is a posterior probability. A frequentist paired [bootstrap](statistical-modelling.md#bootstrapping-statistics) version displays the fraction of replicates for which the net benefit is positive, a resampling measure of uncertainty rather than literally a probability that a fixed true parameter is positive. Using the sign of net benefit handles all quadrants of the [cost-effectiveness plane](#cost-effectiveness-plane); counting only replicates whose ratio is below the threshold does not.

#### Cost-effectiveness plane

↑ **Parent:** [Cost-effectiveness analysis](#cost-effectiveness-analysis)

The [cost-effectiveness plane](#cost-effectiveness-plane) plots an effect increment horizontally and a cost increment vertically. The southeast quadrant represents greater effectiveness at lower cost, while the northwest quadrant represents lower effectiveness at greater cost. A threshold $\lambda$ corresponds to the line $\Delta C=\lambda\Delta E$; points below the line have positive [incremental net monetary benefit](#incremental-net-monetary-benefit), in every quadrant. A joint confidence region or paired [bootstrap](statistical-modelling.md#bootstrapping-statistics) cloud reveals uncertainty and preserves the dependence between cost and effect estimates.

#### Incremental cost-effectiveness ratio

↑ **Parent:** [Cost-effectiveness analysis](#cost-effectiveness-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incremental_cost-effectiveness_ratio)

The [incremental cost-effectiveness ratio](#incremental-cost-effectiveness-ratio) divides an intervention's additional mean cost by its additional mean effect relative to a comparator. Its units are cost per outcome unit. When both increments are positive, comparison with a threshold $\lambda$ is equivalent to checking whether the [incremental net monetary benefit](#incremental-net-monetary-benefit) $\lambda\Delta E-\Delta C$ is positive. When $\Delta E<0$ the inequality reverses on division, and when $\Delta E=0$ the ratio is undefined. A ratio alone cannot identify the quadrant of the [cost-effectiveness plane](#cost-effectiveness-plane).

### Bayesian decision problem

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

A prior on a parameter, a conditional observation distribution, an action space and a loss specify a Bayesian decision problem. The normal form minimizes prior expected loss over [decision rules](#decision-rule); the extensive form minimizes posterior expected loss after each observation. Conditional expectation gives the same [Bayes risk](#bayes-risk) for these formulations, provided measurable optimal or approximate choices can be made.

### Decision rule

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_rule)

A measurable choice of an action from observed data, with a randomized rule allowing a conditional distribution of actions. Its performance under a loss function is the [risk function](statistical-modelling.md#risk-function) $R(\theta,\delta)=\mathbb E_\theta L(\theta,\delta(X))$. Admissibility compares risks pointwise, Bayes optimality integrates risk under a prior, and minimax optimality minimizes the worst-case risk.

### Absolute-error loss

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

The loss $|a-\theta|$ for estimating a real parameter $\theta$ by $a$. Its [risk of a decision rule](#risk-of-a-decision-rule) is the corresponding [expected value](expected-value.md). Unlike [squared-error loss](#squared-error-loss), its pointwise size is a [metric](topological-analysis.md#metric), so the triangle inequality gives a direct overlap version of the [Le Cam two-point lemma](#le-cam-two-point-lemma).

#### Asymmetric absolute-error loss

↑ **Parent:** [Absolute-error loss](#absolute-error-loss)

This loss assigns different positive costs to underestimation and overestimation of a scalar parameter. Here $\gamma$ penalizes estimates below the parameter and $\delta$ estimates above it. Equal costs give a multiple of [absolute-error loss](#absolute-error-loss).

##### Bayes quantile under asymmetric absolute-error loss

↑ **Parent:** [Asymmetric absolute-error loss](#asymmetric-absolute-error-loss)

For a [posterior distribution](bayesian-statistics.md#bayesian-posterior) with finite first moment, the [posterior](bayesian-statistics.md#bayesian-posterior) risk [derivative](calculus.md#derivative) at continuity points is $(\gamma+\delta)F(a)-\gamma$. [Convexity](real-analysis.md#convex-function) therefore makes a [posterior](bayesian-statistics.md#bayesian-posterior) $\gamma/(\gamma+\delta)$-quantile a [Bayes estimator](bayesian-statistics.md#bayes-estimator). With atoms, the condition is $F(a^-)\leq\gamma/(\gamma+\delta)\leq F(a)$. Increasing the cost of underestimation moves the optimal estimate upward.

### Squared-error loss

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

Quadratic loss penalizes an estimate $a$ of a vector parameter $\theta$ by $\lVert a-\theta\rVert^2$. Its posterior expected value is minimized by the posterior mean.

#### Quadratic risk

↑ **Parent:** [Squared-error loss](#squared-error-loss)

The risk of an estimator under squared Euclidean error is its expected squared distance from the true parameter. Pointwise risk domination can be strict even when the supremum risk agrees, because the supremum can be approached at parameters tending to infinity.

##### Mean-vector prediction risk

↑ **Parent:** [Quadratic risk](#quadratic-risk)

The mean-vector prediction risk measures squared [Euclidean norm](normed-vector-space.md#euclidean-norm) error in estimating the deterministic response mean. For [independent](random-variable.md#independent-random-variables) future noise with [covariance matrix](variance.md#covariance-matrix) $\sigma^2I_n$, prediction of a new noisy response adds $n\sigma^2$ to this risk. A Gaussian [orthogonal projection matrix](inner-product.md#orthogonal-projection-matrix) $P$ of rank $k$ has risk $\|(I-P)\mu\|^2+k\sigma^2$.

###### Unbiased Gaussian projection risk estimate

↑ **Parent:** [Mean-vector prediction risk](#mean-vector-prediction-risk)

For $Y\sim N_n(\mu,\sigma^2I)$ and a fixed [orthogonal projection matrix](inner-product.md#orthogonal-projection-matrix) $P$ of rank $k$, the displayed expression is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the [mean-vector prediction risk](#mean-vector-prediction-risk) whenever $\widehat\sigma^2$ is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of $\sigma^2$. [Independence](random-variable.md#independent-random-variables) of its two terms is unnecessary. Comparing fixed models yields the [Mallows Cp](statistical-modelling.md#mallows-s-cp) penalty, but minimizing unbiased estimates does not preserve unbiasedness after selection.

###### Unknown-variance risk estimation in a saturated Gaussian model

↑ **Parent:** [Unbiased Gaussian projection risk estimate](#unbiased-gaussian-projection-risk-estimate)

For a [normal distribution](probability-distribution.md#normal-distribution) $N_n(\mu,\sigma^2I)$ with unrestricted $\mu\in\mathbb R^n$ and unknown $\sigma^2$, an integrable data-only [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the [mean-vector prediction risk](#mean-vector-prediction-risk) of a fixed rank-$k$ [orthogonal projection matrix](inner-product.md#orthogonal-projection-matrix) exists exactly when $2k=n$. To prove necessity, randomize the mean by [independent](random-variable.md#independent-random-variables) Gaussian [variance](variance.md) $v$: conditioning adds $(n-k)v$ to the squared bias term, whereas the marginal [variance](variance.md) identity would add $kv$. When $2k=n$, the [residual sum of squares](linear-regression.md#residual-sum-of-squares) itself is unbiased.

### Le Cam two-point lemma

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

Le Cam's two-point lemma lower-bounds minimax risk by reducing estimation to testing two separated parameter values. Under squared loss, one form is

$$
\inf_{\widehat\theta}\max_{j=0,1}\mathbb E_j(\widehat\theta-\theta_j)^2
\geq\frac{(\theta_1-\theta_0)^2}{8}
\left(1-\operatorname{TV}(P_0,P_1)\right).
$$

#### Metric two-point risk bound

↑ **Parent:** [Le Cam two-point lemma](#le-cam-two-point-lemma)

If two parameters are separated by at least $2r$ in a [metric](topological-analysis.md#metric), any [estimator](statistical-modelling.md#estimator) gives a test by deciding whether its distance from the first parameter is below $r$. For $0<\eta<1$, the event $|Z-1|\le\eta$ and [Markov inequality](probability-inequality.md#markov-s-inequality) give the displayed [minimax risk](statistical-modelling.md#minimax-risk) bound, where $Z$ is the product [likelihood ratio](statistical-hypothesis-test.md#likelihood-ratio). The unrestricted claim for every positive $\eta$ is false when both factors on the right are negative.

#### Metric squared-loss two-point bound

↑ **Parent:** [Le Cam two-point lemma](#le-cam-two-point-lemma)

For any [estimator](statistical-modelling.md#estimator) $T$ in a [metric](topological-analysis.md#metric) parameter space, $d(T,f)^2+d(T,g)^2\geq d(f,g)^2/2$ by the [triangle inequality](topological-analysis.md#triangle-inequality). Average the two [risk functions](statistical-modelling.md#risk-function) and replace their [probability density functions](continuous-probability-distribution.md#probability-density-function) by their minimum. This proves $\max(R_f,R_g)\geq d(f,g)^2\int\min(p_f,p_g)/4$. The overlap equals one minus [total variation distance](probability-and-statistics.md#total-variation-distance). The same proof applies to squared error for a real-valued [statistical functional](#statistical-functional) of the parameter, without requiring that functional to be injective.

##### Mean-estimation minimax lower bound for continuous densities

↑ **Parent:** [Metric squared-loss two-point bound](#metric-squared-loss-two-point-bound)

For estimating the [expected value](expected-value.md) over all continuous [probability density functions](continuous-probability-distribution.md#probability-density-function) on $[0,1]$, compare $f=1$ and $g_n(u)=1+(u-1/2)/\sqrt n$. Their means differ by $1/(12\sqrt n)$, and $\chi^2(P_{g_n}\Vert P_f)=1/(12n)$. The [chi-squared divergence of product measures](f-divergence.md#chi-squared-divergence-of-product-measures) bounds joint [total variation distance](probability-and-statistics.md#total-variation-distance) by $1/2$. The [metric squared-loss two-point bound](#metric-squared-loss-two-point-bound) then gives the displayed uniform [minimax risk](statistical-modelling.md#minimax-risk) lower bound.

#### Chi-squared testing lower bound

↑ **Parent:** [Le Cam two-point lemma](#le-cam-two-point-lemma)

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|P-Q\|_{\mathrm{TV}}=\frac12\mathbb E_Q|dP/dQ-1|\leq\frac12\sqrt{\chi^2(P\Vert Q)}$. Every [statistical hypothesis testing](statistical-hypothesis-test.md) rule has sum of its [Type I error](information-theory.md#type-i-and-type-ii-errors) and [Type II error](information-theory.md#type-i-and-type-ii-errors) at least $1-\|P-Q\|_{\mathrm{TV}}$, proving the displayed bound. A [mixture model](statistical-modelling.md#mixture-model) of alternatives yields a lower bound on the worst alternative error because a maximum dominates an average.

#### Le Cam lower bound under absolute-error loss

↑ **Parent:** [Le Cam two-point lemma](#le-cam-two-point-lemma)

For two observation laws $P_0,P_1$ at real parameters separated by $\Delta$, every [estimator](statistical-modelling.md#estimator) $T$ satisfies $\max_j\mathbb E_j|T-\theta_j|\geq\Delta(1-\operatorname{TV}(P_0,P_1))/2$. With common densities, the sum of the two risks is at least $\int\min(p_0,p_1)(|T-\theta_0|+|T-\theta_1|)$, at least $\Delta\int\min(p_0,p_1)=\Delta(1-\operatorname{TV})$ by the [triangle inequality](topological-analysis.md#triangle-inequality). Divide by two. The same proof works for any [metric](topological-analysis.md#metric) loss.

##### Gaussian location minimax lower bound under absolute-error loss

↑ **Parent:** [Le Cam lower bound under absolute-error loss](#le-cam-lower-bound-under-absolute-error-loss)

For $n$ [independent](random-variable.md#independent-random-variables) observations with a [normal distribution](probability-distribution.md#normal-distribution) $N(\mu,\sigma^2)$, $\sigma>0$ fixed, every [estimator](statistical-modelling.md#estimator) has $\sup_\mu\mathbb E_\mu|T-\mu|\geq\sigma/(4\sqrt{2n})$. Compare $\mu_0=0$ and $\mu_1=\sigma/\sqrt{2n}$: the joint [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) is $1/4$, so the [total variation–Hellinger–relative entropy inequality](f-divergence.md#total-variation-hellinger-relative-entropy-inequality) bounds [total variation distance](probability-and-statistics.md#total-variation-distance) by $1/2$. Apply the [Le Cam lower bound under absolute-error loss](#le-cam-lower-bound-under-absolute-error-loss). Degenerate zero-noise laws do not satisfy a positive lower bound.

#### Two-point lower bound with a triangular bump

↑ **Parent:** [Le Cam two-point lemma](#le-cam-two-point-lemma)

For [fixed-design nonparametric regression](nonparametric-statistics.md#fixed-design-nonparametric-regression), compare $m_0=0$ with $m_1(x)=L(h-|x-x_0|)_+$. This pair has parameter separation $Lh$ at $x_0$, [Lipschitz bound](real-analysis.md#lipschitz-bound) $L$, and [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) at most $L^2h^2(2nh+1)/(2\sigma^2)$. Choosing $h\asymp(\sigma^2/(nL^2))^{1/3}$ controls [total variation distance](probability-and-statistics.md#total-variation-distance) by [Pinsker's inequality](probability-and-statistics.md#pinsker-s-inequality) and yields the [pointwise minimax rate for Lipschitz regression](nonparametric-statistics.md#pointwise-minimax-rate-for-lipschitz-regression) through the [Le Cam two-point lemma](#le-cam-two-point-lemma).

### Bayes classifier

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayes_classifier)

Under zero-one loss, a Bayes classifier assigns an observation to a class of greatest posterior probability. For two classes with prior probabilities $\pi_0,\pi_1$ and densities $f_0,f_1$, it chooses class one exactly when $\pi_1f_1(x)\geq\pi_0f_0(x)$.

#### Cost-sensitive Bayes classifier

↑ **Parent:** [Bayes classifier](#bayes-classifier)

With zero cost for correct classifications, assign class one when the displayed inequality holds and class two otherwise. It compares conditional expected losses; ties may be resolved arbitrarily. For positive costs and densities, the log likelihood ratio threshold is $\log(c(1\mid2)\pi_2/(c(2\mid1)\pi_1))$.

#### Minimum-integral decision region

↑ **Parent:** [Bayes classifier](#bayes-classifier)

For integrable real $g$, including points where $g<0$ decreases the integral and including points where $g>0$ increases it. Thus the negative set minimizes the integral, up to null sets and arbitrary choices where $g=0$. This elementary signed-integral fact derives the [Bayes classifier](#bayes-classifier) and [cost-sensitive Bayes classifier](#cost-sensitive-bayes-classifier).

#### Gaussian Bayes classifier

↑ **Parent:** [Bayes classifier](#bayes-classifier)

For two [multivariate normal densities](probability-and-statistics.md#multivariate-normal-density), the Bayes log posterior odds are a quadratic polynomial. Equal covariance matrices cancel the quadratic term and give [linear discriminant analysis](statistical-modelling.md#linear-discriminant-analysis); unequal covariance matrices give [quadratic discriminant analysis](statistical-modelling.md#quadratic-discriminant-analysis).

##### Prior-dependent Gaussian discriminant boundary

↑ **Parent:** [Gaussian Bayes classifier](#gaussian-bayes-classifier)

For two [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) classes with a common positive-definite [covariance matrix](variance.md#covariance-matrix), $L=\Sigma^{-1}(\mu_1-\mu_2)$ and the displayed score is the log posterior odds of class one against class two. With equal error costs, positive scores favor class one. Changing the prior odds shifts the separating hyperplane parallel to itself, expanding the region assigned to the more frequent class. On the boundary either decision has the same conditional risk.

##### Equal-covariance Gaussian classification error

↑ **Parent:** [Gaussian Bayes classifier](#gaussian-bayes-classifier)

For two [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) classes with equal priors and common [positive-definite](bilinear-form.md#positive-definite-bilinear-form) covariance, the optimal score is $(\mu_1-\mu_2)^T\Sigma^{-1}(x-(\mu_1+\mu_2)/2)$. Its distribution within either class is normal with [variance](variance.md) $D^2$ and mean respectively $D^2/2$ or $-D^2/2$. Both class error probabilities are therefore the displayed normal tail.

#### Uniqueness of a Bayes classifier

↑ **Parent:** [Bayes classifier](#bayes-classifier)

A binary Bayes classifier under zero-one loss is unique up to null sets when the posterior class probabilities tie only on a null set. For two distinct nonsingular Gaussian distributions, the tie set is the zero set of a nonzero quadratic polynomial and has Lebesgue measure zero.

### Risk of a decision rule

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)

For a model $\{P_\theta:\theta\in\Theta\}$, loss $L$, and decision rule $\delta$, the risk is

$$
R(\theta,\delta)=\mathbb E_\theta L(\delta(X),\theta).
$$

### Bayes risk

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayes_risk)

For a prior $\pi$, the integrated risk is $r(\pi,\delta)=\int R(\theta,\delta)\,\pi(d\theta)$. Its infimum over decision rules is the Bayes risk, attained by a Bayes rule when one exists.

#### Bayes act

↑ **Parent:** [Bayes risk](#bayes-risk)

A Bayes act minimizes $\int L(\theta,a)\Pi(d\theta)$ for a specified parameter distribution $\Pi$. Applying the same minimization to the posterior after observing data gives a [Bayes decision rule](bayesian-statistics.md#bayes-decision-rule). The optimal data-based [Bayes risk](#bayes-risk) is the expectation of the optimal posterior no-data loss.

##### Highest density region

↑ **Parent:** [Bayes act](#bayes-act)

For a probability density $\pi$ and threshold $c>0$, this region includes precisely the points at or above the threshold. It is a [Bayes act](#bayes-act) for loss $c|S|-\mathbf1_S(\theta)$, since expected loss is $\int_S(c-\pi(\theta))d\theta$. The minimal value is $-\int(\pi-c)_+d\theta$; adding or removing threshold-equality points does not change it.

#### Least favorable prior

↑ **Parent:** [Bayes risk](#bayes-risk)

A least favorable prior maximizes the Bayes risk over the allowed priors. If a Bayes rule has constant risk equal to the minimax value, its prior is least favorable.

### Minimax decision rule

↑ **Parent:** [Statistical decision theory](#statistical-decision-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimax_decision_rule)

A minimax rule minimizes the worst-case risk $\sup_{\theta\in\Theta}R(\theta,\delta)$.

#### Alpha-beta pruning

↑ **Parent:** [Minimax decision rule](#minimax-decision-rule)

#### Equalizer rule

↑ **Parent:** [Minimax decision rule](#minimax-decision-rule)

An equalizer rule has the same risk at every parameter value. A Bayes equalizer rule is minimax when its constant risk bounds from below the worst-case risk of every competing rule.

##### Minimax Gaussian Bayes classifier from equal class errors

↑ **Parent:** [Equalizer rule](#equalizer-rule)

For two distinct nonsingular Gaussian class distributions, vary the class-zero prior continuously. The class-zero and class-one error probabilities of the corresponding [Bayes classifier](#bayes-classifier) cross. At a crossing they are equal, making the classifier an [equalizer rule](#equalizer-rule), a [minimax decision rule](#minimax-decision-rule), and the associated prior a [least favorable prior](#least-favorable-prior).

#### Constant-risk limit-of-Bayes-risk criterion

↑ **Parent:** [Minimax decision rule](#minimax-decision-rule)

If a rule has constant risk $r$ and a sequence of priors has Bayes risks tending to $r$, then the rule is minimax. Every competing rule has worst-case risk at least every one of those Bayes risks.

#### Minimax sample mean for a nonnegative normal location

↑ **Parent:** [Minimax decision rule](#minimax-decision-rule)

For independent $X_i\sim N(\theta,1)$ with $\theta\ge0$, the sample mean has constant squared-error risk $1/n$ and is minimax. Smooth priors supported on $[0,L]$ whose prior Fisher information is $O(L^{-2})$ give, through the [Van Trees inequality](statistical-modelling.md#van-trees-inequality), a lower bound tending to $1/n$ for every rule's worst-case risk.

## Confidence interval

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Confidence_interval)

A [confidence interval](#confidence-interval) is a random interval constructed from a [statistical sample](#statistical-sample) to cover a fixed unknown [statistical parameter](statistical-model.md#statistical-parameter) with a prescribed [coverage probability](#coverage-probability). For a scalar target $\theta$, a procedure with nominal confidence $1-\alpha$ satisfies

$$
\mathbb P_\theta\{L(X)\leq\theta\leq U(X)\}\geq1-\alpha
\quad\text{for every admissible }\theta.
$$

The subscript records which [probability distribution](probability-distribution.md) generates the repeated samples. The endpoints are [statistics](#statistic), so they vary from sample to sample; the target is fixed. Equality gives exact nominal [coverage probability](#coverage-probability), while the inequality also permits conservative procedures. For a general [estimand](#estimand) $\psi(\theta)$, replace the target inside the interval by $\psi(\theta)$.

A realized [confidence interval](#confidence-interval) communicates the precision of an estimate in the target's own units. Reporting $1.2$ alone conceals the difference between an estimate with [standard error](#standard-error) $0.5$ and one with [standard error](#standard-error) $0.05$. A narrow [confidence interval](#confidence-interval) indicates greater precision for the stated [statistical model](statistical-model.md), rather than a guarantee that its assumptions describe the experiment correctly.

Once $x$ is observed, $C(x)$ either contains the fixed target or does not. The 95% statement concerns the random procedure $C(X)$, not a [posterior probability](bayesian-statistics.md#posterior-probability) of 0.95 that this particular interval contains $\theta$. A [credible interval](bayesian-statistics.md#credible-interval) instead assigns specified [posterior probability](bayesian-statistics.md#posterior-probability) to a region under [Bayesian inference](bayesian-statistics.md). These interpretations can differ even when the numerical endpoints agree. The repeated-sampling interpretation is explained in [NIST's confidence-limits teaching reference](https://www.itl.nist.gov/div898/handbook/eda/section3/eda352.htm).

Jerzy Neyman's 1937 paper formulates the fixed-target, random-endpoint construction in Section II, especially equation (20) on page 348. Its confidence coefficient must hold across the allowed [statistical parameters](statistical-model.md#statistical-parameter), rather than only at the value suggested by one sample. See [Neyman, Outline of a Theory of Statistical Estimation Based on the Classical Theory of Probability](https://doi.org/10.1098/rsta.1937.0005) and the [original paper scan](https://wwwusers.ts.infn.it/~milotti/Didattica/StatisticaAvanzata/Neyman_1937.pdf).

### Normal mean confidence interval with known variance

↑ **Parent:** [Confidence interval](#confidence-interval)

Suppose $X_1,\ldots,X_n$ are [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) with [normal distribution](probability-distribution.md#normal-distribution) $N(\mu,\sigma^2)$, where the [mean](expected-value.md) $\mu$ is unknown and the [standard deviation](variance.md#standard-deviation) $\sigma>0$ is known. The [sample mean](variance.md#sample-mean) $\bar X=n^{-1}\sum_iX_i$ has [normal distribution](probability-distribution.md#normal-distribution) $N(\mu,\sigma^2/n)$ and [standard error](#standard-error) $\sigma/\sqrt n$. With $z_q$ the [standard normal quantile](probability-distribution.md#standard-normal-quantile) at $q$, the displayed [confidence interval](#confidence-interval) has exact [coverage probability](#coverage-probability) $1-\alpha$ for every $\mu$ and every positive integer $n$. No [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) approximation is needed.

Take $\sigma=2$, $n=16$ and nominal confidence 95%. The [standard error](#standard-error) is $2/\sqrt{16}=0.5$, and $z_{0.975}=1.9599639845\ldots$. Therefore

$$
C(X)=[\bar X-0.9799819923\ldots,\ \bar X+0.9799819923\ldots].
$$

Rounded for reporting, this is $\bar x\pm0.98$. If $\bar x=1.2$, the realized [confidence interval](#confidence-interval) is approximately $[0.22,2.18]$. Exact 95% calibration refers to the unrounded [standard normal quantile](probability-distribution.md#standard-normal-quantile); using $1.96$ literally gives [coverage probability](#coverage-probability) $0.9500042097\ldots$, almost but not exactly 0.95.

The [confidence interval](#confidence-interval)'s width scales as $n^{-1/2}$: increasing [sample size](probability-and-statistics.md#sample-size) from 16 to 64 halves its half-width to $0.4899909961\ldots$. If $\sigma$ is unknown, merely substituting the square root of a [sample variance](#sample-variance) loses the displayed exact calibration; for the same [normal distribution](probability-distribution.md#normal-distribution) model, use a [Student t confidence interval](#student-t-confidence-interval).

The figure holds the true [mean](expected-value.md) at $\mu=0$ and independently generates 40 samples of 16 observations from the same [normal distribution](probability-distribution.md#normal-distribution). NumPy's PCG64 generator with seed 42 gives 39 covering [confidence intervals](#confidence-interval) and one miss, at sample 32: observed coverage is $39/40=97.5\%$. Every bar uses the unrounded [standard normal quantile](probability-distribution.md#standard-normal-quantile). This finite collection illustrates the moving endpoints; it does not establish the analytic [coverage probability](#coverage-probability) or require exactly two misses.

<a id="image-forty-normal-mean-confidence-intervals-and-their-exact-95-percent-coverage-event"></a>
![](confidence-interval-coverage.png)

**[Figure 8](#image-forty-normal-mean-confidence-intervals-and-their-exact-95-percent-coverage-event). Forty normal-mean confidence intervals and their exact 95% coverage event**.

The beauty of the construction is that a familiar [standard normal distribution](probability-distribution.md#standard-normal-distribution) calibrates every possible unknown [mean](expected-value.md) at once. For a short proof, the [pivotal quantity](probability-and-statistics.md#pivotal-quantity)

$$
Z=\frac{\bar X-\mu}{\sigma/\sqrt n}\sim N(0,1)
$$

has a [probability distribution](probability-distribution.md) independent of $\mu$. The event $|Z|\leq z_{1-\alpha/2}$ has [probability](probability-theory.md#probability) $1-\alpha$; rearranging it gives $\mu\in C(X)$. The right panel shows the equivalent event $|\bar X|\leq0.9799819923\ldots$ when $\mu=0$.

#### Normal mean confidence interval and hypothesis test duality

↑ **Parent:** [Normal mean confidence interval with known variance](#normal-mean-confidence-interval-with-known-variance)

For the same [normal distribution](probability-distribution.md#normal-distribution) model, a [two-sided test](statistical-hypothesis-test.md#two-sided-hypothesis-test) compares the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis) $H_0:\mu=\mu_0$ with the [alternative hypothesis](statistical-hypothesis-test.md#alternative-hypothesis) $H_1:\mu\ne\mu_0$. Under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis), the standardized [test statistic](statistical-hypothesis-test.md#test-statistic) has [standard normal distribution](probability-distribution.md#standard-normal-distribution). Write $\Phi$ for the [standard normal distribution function](probability-distribution.md#standard-normal-distribution-function). With $\bar x=1.2$, $\sigma=2$, $n=16$ and $\mu_0=0$, the observed [test statistic](statistical-hypothesis-test.md#test-statistic) is $z=1.2/0.5=2.4$. Its [p-value](statistical-hypothesis-test.md#p-value) is

$$
p=\mathbb P_{\mu_0}(|Z|\geq2.4)
=2[1-\Phi(2.4)]
=0.01639507185\ldots.
$$

Thus the [p-value](statistical-hypothesis-test.md#p-value) is a tail [probability](probability-theory.md#probability) computed under the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis), including departures in both directions. It is not $\mathbb P(H_0\mid x)$, the [posterior probability](bayesian-statistics.md#posterior-probability) of the [null hypothesis](statistical-hypothesis-test.md#null-hypothesis), nor the [probability](probability-theory.md#probability) that the observations arose "by chance". The [normal distribution](probability-distribution.md#normal-distribution) [test statistic](statistical-hypothesis-test.md#test-statistic) and its calibration appear in [NIST's teaching reference for testing a process mean](https://www.itl.nist.gov/div898/handbook/prc/section2/prc22.htm); the tail interpretation is stated in [Penn State's hypothesis-testing notes](https://online.stat.psu.edu/stat200/Lesson05).

Choose the [significance level](statistical-hypothesis-test.md#significance-level) $\alpha=0.05$ before observing the sample. The [rejection region](statistical-hypothesis-test.md#rejection-region) is $|Z|>z_{0.975}$, whose [probability](probability-theory.md#probability) under $H_0$ is exactly 0.05. Here $2.4>1.9599639845\ldots$, so reject $H_0$. This agrees with zero lying outside $[0.22,2.18]$. More generally, a proposed $\mu_0$ belongs to the unrounded 95% [confidence interval](#confidence-interval) precisely when its [two-sided test](statistical-hypothesis-test.md#two-sided-hypothesis-test) does not reject under this strict cutoff. The equality boundary has [probability](probability-theory.md#probability) zero in this continuous [statistical model](statistical-model.md).

<a id="image-the-chosen-5-percent-rejection-tails-and-the-observed-two-sided-p-value"></a>
![](hypothesis-test-normal-tails.png)

**[Figure 9](#image-the-chosen-5-percent-rejection-tails-and-the-observed-two-sided-p-value). The chosen 5% rejection tails and the observed two-sided p-value**.

The [significance level](statistical-hypothesis-test.md#significance-level) and [statistical power](probability-and-statistics.md#statistical-power) describe different repeated-experiment [probabilities](probability-theory.md#probability). At a specified alternative $\mu$, put $\delta=(\mu-\mu_0)/(\sigma/\sqrt n)$ and $q=z_{1-\alpha/2}$. Then

$$
\begin{aligned}
\mathbb P_{\mu_0}(\text{reject }H_0)&=\alpha,\\
\beta(\mu)=\mathbb P_\mu(\text{do not reject }H_0)&=\Phi(q-\delta)-\Phi(-q-\delta),\\
\mathbb P_\mu(\text{reject }H_0)&=1-\beta(\mu).
\end{aligned}
$$

The first is the [Type I error](information-theory.md#type-i-and-type-ii-errors) [probability](probability-theory.md#probability); the second is the [Type II error](information-theory.md#type-i-and-type-ii-errors) [probability](probability-theory.md#probability) at that alternative. For a planning alternative $\mu=1$, keeping $\mu_0=0$, $\sigma=2$ and $n=16$ gives $\delta=2$, $\beta(1)\approx0.483995$ and [statistical power](probability-and-statistics.md#statistical-power) $0.516005$. At $n=64$, $\delta=4$ and [statistical power](probability-and-statistics.md#statistical-power) rises to $0.979327$. These are model calculations for specified alternatives, not [posterior probabilities](bayesian-statistics.md#posterior-probability) inferred from a nonsignificant result. They explain why failure to reject cannot establish equality and why choosing [sample size](probability-and-statistics.md#sample-size) before an experiment is useful.

Historically, Ronald Fisher's 1925 book discusses the normal cutoff $1.96$ and tail [probability](probability-theory.md#probability) 0.05 as a convenient convention on page 47, rather than a mathematically compulsory threshold: [Fisher, Statistical Methods for Research Workers, first edition](https://books.google.com/books/about/Statistical_Methods_for_Research_Workers.html?id=I0NBAAAAIAAJ).

### Coverage probability

↑ **Parent:** [Confidence interval](#confidence-interval)

The [coverage probability](#coverage-probability) is the repeated-sampling [probability](probability-theory.md#probability) that a random [confidence interval](#confidence-interval) contains the fixed true [statistical parameter](statistical-model.md#statistical-parameter). A finite-sample level-$1-\alpha$ procedure has [coverage probability](#coverage-probability) at least $1-\alpha$ at every admissible [statistical parameter](statistical-model.md#statistical-parameter); exact nominal coverage means equality. An asymptotically calibrated procedure approaches the nominal value as [sample size](probability-and-statistics.md#sample-size) grows, under its stated assumptions. Higher-order [Edgeworth expansions](probability-distribution.md#edgeworth-series) can quantify the discrepancy from nominal [coverage probability](#coverage-probability) when their regularity conditions hold.

Observed coverage in finitely many repetitions is itself random. For $m$ independent repetitions of the exact [normal mean confidence interval with known variance](#normal-mean-confidence-interval-with-known-variance), the count $K$ of covering [confidence intervals](#confidence-interval) has [binomial distribution](discrete-probability-distribution.md#binomial-distribution) $\operatorname{Binomial}(m,0.95)$. At $m=40$, its [expectation](expected-value.md) is $38$, but

$$
\mathbb P(K=39)=\binom{40}{39}0.95^{39}0.05\approx0.270552.
$$

Consequently, the 39 successes in the figure are compatible with exact 95% [coverage probability](#coverage-probability). The guarantee follows from the [pivotal quantity](probability-and-statistics.md#pivotal-quantity)'s [probability distribution](probability-distribution.md); the finite observed fraction is an illustration. Also distinguish a [confidence interval](#confidence-interval) for a fixed [mean](expected-value.md) from a [prediction interval](#prediction-interval) for a future observation: the latter must accommodate the new observation's variation as well as estimation uncertainty.

### Extreme-order-statistic tolerance interval

↑ **Parent:** [Confidence interval](#confidence-interval)

The sample minimum and maximum enclose random population content given by the [uniformized sample range](probability-theory.md#uniformized-sample-range). The exact failure probability for content at least $1-\varepsilon$ is $(1-\varepsilon)^{n-1}[1+(n-1)\varepsilon]$. For small $\varepsilon$, setting $n\varepsilon\approx\vartheta$ gives the displayed sample-size approximation at confidence $1-\delta$. The positive solution is unique for $0<\delta<1$, since $(1+\vartheta)e^{-\vartheta}$ decreases from one to zero. A tolerance interval concerns population content, rather than a [confidence interval](#confidence-interval) for a fixed parameter; the exact inequality should select the final integer size.

### Exponential-mean confidence interval by pivot inversion

↑ **Parent:** [Confidence interval](#confidence-interval)

For an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) with mean $\theta$, the [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator) is $\bar Y$ and $\sqrt n(\bar Y-\theta)/\theta$ converges to a standard [normal distribution](probability-distribution.md#normal-distribution). Inverting the event that this pivot lies between $-z$ and $z$ gives the displayed [confidence interval](#confidence-interval), provided $n>z^2$. Its two-sided [coverage probability](#coverage-probability) has error $O(n^{-1})$, because the first [Edgeworth expansion](probability-distribution.md#edgeworth-series) term is even and cancels between the two tails.

<h3 id="fieller-s-theorem">Fieller's theorem</h3>

↑ **Parent:** [Confidence interval](#confidence-interval)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fieller's_theorem)

For jointly approximately [normal](probability-distribution.md#normal-distribution) estimates $(\widehat C,\widehat E)$ with estimated [variances](variance.md) $v_C,v_E$ and [covariance](variance.md#covariance) $v_{CE}$, a [confidence interval](#confidence-interval) for the ratio $C/E$, where $E\ne0$, can be obtained by inverting tests of $C-rE=0$. For each proposed ratio $r$, the contrast has estimate $\widehat C-r\widehat E$ and [variance](variance.md) $v_C-2rv_{CE}+r^2v_E$. Retain $r$ when its absolute standardized contrast is at most the chosen critical value $q$. This gives the displayed quadratic inequality, with coefficients $A=\widehat E^2-q^2v_E$, $B=-2(\widehat C\widehat E-q^2v_{CE})$, $D=\widehat C^2-q^2v_C$. When $A>0$ and the discriminant is positive, retain the interval between the roots. When $A<0$, a confidence set can instead be two unbounded rays or the entire real line. Degenerate linear cases are interpreted directly from the inequality. A bounded interval must not be forced when the denominator is poorly separated from zero. Known [covariance matrix](variance.md#covariance-matrix) and a joint [normal distribution](probability-distribution.md#normal-distribution) give exact normal critical values; estimated covariance usually gives approximate coverage, unless an appropriate exact common-scale pivot exists.

### Confidence bound

↑ **Parent:** [Confidence interval](#confidence-interval)

A lower confidence bound $L$ gives a one-sided [confidence interval](#confidence-interval) with the displayed coverage requirement for every admissible parameter. An upper bound $U$ instead satisfies $\Pr_\theta\{\theta\leq U\}\geq1-\alpha$. Coverage is a repeated-sampling property; it does not assign a posterior probability to the fixed parameter.

### Likelihood-ratio confidence interval

↑ **Parent:** [Confidence interval](#confidence-interval)

Invert a [likelihood-ratio test](statistical-hypothesis-test.md#likelihood-ratio-test) for a scalar parameter, maximizing over nuisance parameters for each fixed candidate value. Under regularity, a level $1-\alpha$ interval includes values whose profile [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is at most $\chi^2_{1,1-\alpha}/2$ below its maximum. This explains the horizontal cutoff on a [Box–Cox transformation](statistical-modelling.md#box-cox-transformation) likelihood plot.

### Confidence interval for a reciprocal rate

↑ **Parent:** [Confidence interval](#confidence-interval)

If a positive rate $q$ has a [confidence interval](#confidence-interval) $[L,U]$, monotonicity transforms it into $[1/U,1/L]$ for the reciprocal mean $1/q$. This preserves the coverage event exactly and reverses the endpoints. It applies directly to mean exponential [holding times](continuous-time-markov-chain.md#holding-time).

### Order-statistic confidence interval for a median

↑ **Parent:** [Confidence interval](#confidence-interval)

For a sample of size $n$ from a [continuous probability distribution](continuous-probability-distribution.md), this interval covers the [median](probability-distribution.md#median) $F^{-1}(1/2)$ with probability $1-2\sum_{r=0}^{j-1}\binom nr2^{-n}$, for $1\leq j<n/2$. Count observations below the [median](probability-distribution.md#median): their number has the [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with parameters $n,1/2$. No strict increase of the [distribution function](probability-distribution.md#cumulative-distribution-function) is needed.

### Support-restricted confidence interval for a uniform location parameter

↑ **Parent:** [Confidence interval](#confidence-interval)

For two independent observations uniform on $[\theta-a,\theta+a]$, the displayed interval of possible parameter values contains the true parameter almost surely. Intersecting any [confidence interval](#confidence-interval) with it preserves that interval's coverage, while excluding values inconsistent with the observations. The [order statistics](probability-theory.md#order-statistic) interval $[U_{(1)},U_{(2)}]$ has coverage $1/2$, since the observations straddle $\theta$ with probability $1/2$. If their separation exceeds $a$, the entire interval of possible parameters lies between the observations; this explains why the nominal one-half procedure can be unnecessarily wide on that event.

## Prediction interval

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prediction_interval)

A prediction interval is a random interval designed to contain a future observation with prescribed repeated-sampling probability. Unlike a [confidence interval](#confidence-interval) for a mean response, it includes both uncertainty in the fitted mean and the new observation's irreducible random variation.

### Normal prediction interval with maximum-likelihood variance

↑ **Parent:** [Prediction interval](#prediction-interval)

For independent [normal random variables](probability-distribution.md#gaussian-random-variable) with unknown common mean and variance, let $\widehat\sigma^2=n^{-1}\sum(X_i-\bar X)^2$ and $n\ge2$. The standardized future difference $X_0-\bar X$ is normal with variance $\sigma^2(1+1/n)$ and is independent of the residual sum of squares. Thus the ratio using the displayed standard error has [Student's t-distribution](continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom. This is unconditional repeated-sampling prediction coverage, not a confidence interval for the mean.

### Prediction interval in a normal linear model

↑ **Parent:** [Prediction interval](#prediction-interval)

For the full-rank [normal linear model](normal-linear-model.md) $Y=X\beta+\varepsilon$ and an independent future response $Y^*=x^{*T}\beta+\varepsilon^*$, put

$$
s^2=\frac{\operatorname{RSS}}{n-p},
\qquad
h^*=x^{*T}(X^TX)^{-1}x^*.
$$

Then an exact $(1-\alpha)$ prediction interval is

$$
x^{*T}\widehat\beta
\mathbin\pm t_{n-p,1-\alpha/2}s\sqrt{1+h^*}.
$$

The additional one inside the square root is the future observation's irreducible error variance; a confidence interval for its mean omits it.

#### Zero-residual degeneracy of regression prediction

↑ **Parent:** [Prediction interval in a normal linear model](#prediction-interval-in-a-normal-linear-model)

When a full-rank normal regression with positive residual degrees of freedom happens to fit all supplied observations exactly, its residual estimate of [variance](variance.md) is zero. The ordinary Studentized prediction-interval formula formally collapses, but the statistic divides by zero. Under positive true Gaussian [variance](variance.md) such samples form a null set; exact rounded or constructed data must not be treated as proof that future randomness vanishes.

### Prediction interval for a ratio of log-normal responses

↑ **Parent:** [Prediction interval](#prediction-interval)

Suppose independent future log responses satisfy $Z_j=x_j^T\beta+\varepsilon_j$, where the errors have variance $\sigma^2$. Conditional on a fitted [normal linear model](normal-linear-model.md), the predicted log ratio $Z_1-Z_2$ has estimated mean $(x_1-x_2)^T\widehat\beta$ and estimated variance

$$
(x_1-x_2)^T\widehat{\operatorname{Var}}(\widehat\beta)(x_1-x_2)+2\widehat\sigma^2.
$$

A [Student t interval](#student-t-confidence-interval) on this logarithmic scale can be exponentiated to obtain a prediction interval for the positive ratio.

## Student t confidence interval

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Student_t_confidence_interval)

A Student t confidence interval replaces unknown Gaussian scale by an independent residual estimate.

### Confidence interval for the difference of independent regression slopes

↑ **Parent:** [Student t confidence interval](#student-t-confidence-interval)

For two independent normal simple regressions with centered predictors, common unknown error variance and $m>2$ observations in each, let $S_u=\sum u_i^2$, $S_w=\sum w_i^2$. The estimated slope difference is normal with mean $b-d$ and variance $\sigma^2(S_u^{-1}+S_w^{-1})$. Pool the two [residual sums of squares](linear-regression.md#residual-sum-of-squares) and use $s^2=RSS/(2m-4)$. Independence from the estimates gives a [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution) pivot, yielding the displayed two-sided interval of confidence $1-\alpha$.

### Student t confidence interval for a centered regression intercept

↑ **Parent:** [Student t confidence interval](#student-t-confidence-interval)

In a two-parameter Gaussian simple linear regression centered at $\bar x$, the intercept estimator is $\bar Y$. With residual standard deviation $s$,

$$
\frac{\bar Y-\alpha'}{s/\sqrt n}\sim t_{n-2},
$$

which gives the usual two-sided interval from the corresponding quantiles.

## Bayesian statistics

↑ **Parent:** [Statistical inference](statistical-inference.md)

[This section is present in another page, follow this link to view it.](bayesian-statistics.md)

## Jackknife bias correction

↑ **Parent:** [Statistical inference](statistical-inference.md)

The [jackknife bias correction](#jackknife-bias-correction) uses [jackknife resampling](#jackknife-resampling) to estimate and subtract the [bias of an estimator](statistical-modelling.md#bias-of-an-estimator). Here $T_n$ denotes the original [estimator](statistical-modelling.md#estimator), $T_{(-i)}$ its version after deleting observation $i$, and $\overline T_J=n^{-1}\sum_{i=1}^nT_{(-i)}$ the [mean](expected-value.md) of those versions. For [sample size](probability-and-statistics.md#sample-size) $n>1$, define

$$
\widehat B_n=(n-1)(\overline T_J-T_n),\qquad
\widetilde T_J=T_n-\widehat B_n=nT_n-(n-1)\overline T_J.
$$

The sign matters: a negative estimated [bias](statistical-modelling.md#bias-of-an-estimator) increases the corrected value. The original [estimator](statistical-modelling.md#estimator) and all deletion versions must target the same [estimand](#estimand) and use the same estimation rule at their respective [sample sizes](probability-and-statistics.md#sample-size). The definition alone does not make $\widetilde T_J$ an [unbiased estimator](statistical-modelling.md#unbiased-estimator).

For an exact worked example, take the [empirical variance](#empirical-variance)

$$
T_n=\frac1n\sum_{i=1}^n(X_i-\overline X_n)^2.
$$

On $(1,2,3,4,10)$, the [sample mean](variance.md#sample-mean) is $4$ and $T_5=50/5=10$. Each deletion [empirical variance](#empirical-variance) is recomputed around its own deletion [sample mean](variance.md#sample-mean), with divisor $4$, giving

$$
(T_{(-1)},\ldots,T_{(-5)})
=(9.6875,11.25,12.1875,12.5,1.25),\qquad
\overline T_J=9.375.
$$

For instance, deleting $10$ leaves $(1,2,3,4)$, whose [sample mean](variance.md#sample-mean) is $2.5$ and whose [empirical variance](#empirical-variance) is $1.25$. The correction on the full [statistical sample](#statistical-sample) is

$$
\widehat B_5=4(9.375-10)=-2.5,\qquad
\widetilde T_J=10-(-2.5)=12.5.
$$

The same data thus give a [jackknife variance estimator](#jackknife-variance-estimator) of $2.5$ for the [sample mean](variance.md#sample-mean), and a corrected [empirical variance](#empirical-variance) of $12.5$; these are different [estimands](#estimand).

<a id="image-two-uses-of-the-same-deletions-sampling-variance-and-jackknife-bias-correction"></a>
![](jackknife-variance-bias.png)

**[Figure 10](#image-two-uses-of-the-same-deletions-sampling-variance-and-jackknife-bias-correction). Two uses of the same deletions: sampling variance and jackknife bias correction**. The left panel plots contributions to the [jackknife variance estimator](#jackknife-variance-estimator) of the [sample mean](variance.md#sample-mean), summing to $2.5$. The right panel plots the five deletion [empirical variances](#empirical-variance) and their [mean](expected-value.md) $9.375$, then compares the original [empirical variance](#empirical-variance) $10$ with the corrected [sample variance](#sample-variance) $12.5$.

The exact equality with the usual [sample variance](#sample-variance) is not an accident of these numbers. For any data with $n>1$, write $Q=\sum_i(x_i-\overline x)^2=nT_n$. Removing $x_i$ changes this sum to $Q-n(x_i-\overline x)^2/(n-1)$, so

$$
T_{(-i)}=\frac{Q}{n-1}-\frac{n(x_i-\overline x)^2}{(n-1)^2},\qquad
\overline T_J=\frac{n(n-2)}{(n-1)^2}T_n,\qquad
\widetilde T_J=\frac{n}{n-1}T_n=s_n^2.
$$

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with finite second [moment](expected-value.md#moment) and population [variance](variance.md) $\sigma^2$, the [expectation](expected-value.md) is $\mathbb E T_n=(1-1/n)\sigma^2$. Its [bias](statistical-modelling.md#bias-of-an-estimator) is exactly $-\sigma^2/n$; [jackknife bias correction](#jackknife-bias-correction) removes it exactly in this example. Thus $s_n^2$ is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of $\sigma^2$ under these assumptions, including $n=2$ where each deletion [empirical variance](#empirical-variance) is zero.

More generally, suppose the [bias](statistical-modelling.md#bias-of-an-estimator) has a regular expansion at both [sample sizes](probability-and-statistics.md#sample-size) $n$ and $n-1$, with coefficients $a,b$ independent of $n$:

$$
B_n=\mathbb E T_n-\theta=\frac an+\frac b{n^2}+O(n^{-3}).
$$

Under [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) sampling, each deletion [estimator](statistical-modelling.md#estimator) has the same [expectation](expected-value.md) as $T_{n-1}$. Hence the corrected [bias](statistical-modelling.md#bias-of-an-estimator) is

$$
\mathbb E\widetilde T_J-\theta=nB_n-(n-1)B_{n-1}=O(n^{-2}),
\qquad n\frac an-(n-1)\frac a{n-1}=0.
$$

The leading $O(n^{-1})$ term cancels; the remaining [bias](statistical-modelling.md#bias-of-an-estimator) need not vanish. The $O$ notation is [big O notation](real-analysis.md#big-o-notation). This argument presumes the expansion, rather than proving it for every [statistic](#statistic); the regularity conditions discussed for the [jackknife variance estimator](#jackknife-variance-estimator) and [statistical dependence](random-variable.md#statistical-dependence) still require care. Shalizi's [jackknife notes, Section 5.1](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) develop the cancellation argument and cite Quenouille's [Notes on Bias in Estimation, Biometrika 43(3–4), 353–360 (1956)](https://academic.oup.com/biomet/article-abstract/43/3-4/353/345190).

### Sample variance

↑ **Parent:** [Jackknife bias correction](#jackknife-bias-correction)

For observations $X_1,\ldots,X_n$, the unbiased sample variance is

$$
s_n^2=\frac1{n-1}\sum_{i=1}^n(X_i-\overline X_n)^2.
$$

For independent identically distributed observations with finite variance $\sigma^2$, it converges in probability to $\sigma^2$.

#### Empirical variance

↑ **Parent:** [Sample variance](#sample-variance)

The [empirical variance](#empirical-variance) is the [variance](variance.md) of the [empirical distribution](information-theory.md#type-information-theory), which puts [probability](probability-theory.md#probability) $1/n$ on each observation. It uses divisor $n$, whereas the usual [sample variance](#sample-variance) uses divisor $n-1$. For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with finite second [moment](expected-value.md#moment), [jackknife bias correction](#jackknife-bias-correction) converts the [empirical variance](#empirical-variance) into the [unbiased estimator](statistical-modelling.md#unbiased-estimator) $s_n^2$ exactly.

#### Pooled sample variance

↑ **Parent:** [Sample variance](#sample-variance)

For two independent normal samples of sizes $m,n$ with a common unknown variance, pooling their within-sample sums of squares gives the [unbiased estimator](statistical-modelling.md#unbiased-estimator) $S_p^2=(S_{XX}+S_{YY})/(m+n-2)$. The numerator divided by the common population variance has a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) with $m+n-2$ degrees of freedom and is independent of both sample means. Therefore $(\bar X-\bar Y-(\mu_X-\mu_Y))/(S_p\sqrt{1/m+1/n})$ has a [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution). This exact construction requires a positive residual number of degrees of freedom and the common-variance assumption.

## Estimating equation

↑ **Parent:** [Statistical inference](statistical-inference.md)

An estimating equation sets an empirical average $n^{-1}\sum_i\psi(X_i;\theta)$ equal to zero to define an estimator of $\theta$.

### Generalized estimating equation

↑ **Parent:** [Estimating equation](#estimating-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_estimating_equation)

For independent clusters with mean vector $m_i(\theta)$ and positive definite working [covariance matrix](variance.md#covariance-matrix) $V_i$, a [generalized estimating equation](#generalized-estimating-equation) solves

$$
\sum_iD_i^TV_i^{-1}(Y_i-m_i)=0,\qquad D_i=\partial m_i/\partial\theta^T.
$$

Correct mean specification and regularity can give a [consistent estimator](#consistency-statistics) of identifiable mean coefficients despite a misspecified working [covariance](variance.md#covariance). A [sandwich covariance matrix](#sandwich-covariance-matrix) accounts for actual cluster variation. Mean equations alone cannot identify two parameters that always enter through the same combination.

#### Working correlation matrix

↑ **Parent:** [Generalized estimating equation](#generalized-estimating-equation)

A [working correlation matrix](#working-correlation-matrix) $R_i(\alpha)$ is a positive-definite proposed correlation structure used to weight a [generalized estimating equation](#generalized-estimating-equation), with $A_i$ the diagonal matrix of marginal [variances](variance.md). It need not equal the actual correlation matrix. Correct marginal means and [independent](random-variable.md#independent-random-variables) sampling clusters keep the estimating equations unbiased; a cluster-level [sandwich covariance matrix](#sandwich-covariance-matrix) estimates their actual large-sample [covariance](variance.md#covariance). For three exchangeable observations, positive definiteness requires $-1/2<\rho<1$.

#### Population-averaged logistic model for repeated binary outcomes

↑ **Parent:** [Generalized estimating equation](#generalized-estimating-equation)

For independent subjects with repeated [Bernoulli](discrete-probability-distribution.md#bernoulli-distribution) observations, specify marginal means $m_{ij}=\operatorname{logit}^{-1}(w_{ij}^T\gamma)$. A [generalized estimating equation](#generalized-estimating-equation) uses their derivative matrix $D_i$ and working [covariance matrix](variance.md#covariance-matrix) $V_i$ to solve $\sum_iD_i^TV_i^{-1}(Y_i-m_i)=0$. Subject-level [sandwich covariance matrices](#sandwich-covariance-matrix) give robust uncertainty when the mean is correctly specified but the working correlation is not. The coefficients describe population [odds ratios](statistical-modelling.md#odds-ratio); this mean specification does not prescribe a complete joint distribution within a subject.

##### Inverse-observation-weighted estimating equations for longitudinal dropout

↑ **Parent:** [Population-averaged logistic model for repeated binary outcomes](#population-averaged-logistic-model-for-repeated-binary-outcomes)

For monotone [missing data](probability-and-statistics.md#missing-data), let $R_{ij}$ indicate observation and let $\rho_{ij}$ be the product of the conditional retention probabilities through visit $j$. Under sequential [missing at random](probability-and-statistics.md#missing-at-random), conditioning on the complete response history makes these retention probabilities depend only on the history already observed at each decision. Therefore $\mathbb E(R_{ij}/\rho_{ij}\mid Y_i,X_i)=1$. Weighting a working-independence [generalized estimating equation](#generalized-estimating-equation) by $R_{ij}/\rho_{ij}$ restores its mean-zero property. This needs correct retention probabilities, positivity and regularity; uncertainty must account for estimating the weights.

#### Marginal incidence trend with clustered observations

↑ **Parent:** [Generalized estimating equation](#generalized-estimating-equation)

A population-averaged log-rate model with exposure $P_{it}$ gives an annual [rate ratio](generalized-linear-model.md#rate-ratio) $e^{\beta_1}$. A [generalized estimating equation](#generalized-estimating-equation) can account for repeated observations within clusters through a working correlation and [sandwich covariance matrix](#sandwich-covariance-matrix). Independent Poisson standard errors do not account for clustering. An exposure-weighted population rate and an equally weighted average of cluster rates are different estimands.

### Z-estimator

↑ **Parent:** [Estimating equation](#estimating-equation)

A Z-estimator is a root of an estimating equation. Under differentiability, identification, and a central limit theorem, its first-order expansion has sandwich covariance.

#### Consistency of a uniquely bracketed zero

↑ **Parent:** [Z-estimator](#z-estimator)

Suppose random continuous real functions have unique zeros. If pointwise [convergence in probability](convergence-of-random-variables.md#convergence-in-probability) gives opposite strict limiting signs at the two ends of every sufficiently small interval about the target, the [intermediate value theorem](calculus.md#intermediate-value-theorem) traps their zeros in those intervals with [probability](probability-theory.md#probability) tending to one. The limiting function need not be continuous and the random functions need not be monotone.

## Asymptotic normality

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_normality)

An estimator is asymptotically normal when a rescaled estimation error converges in distribution to a normal law.

### Slutsky theorem

↑ **Parent:** [Asymptotic normality](#asymptotic-normality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slutsky_theorem)

Slutsky's theorem combines convergence in distribution with convergence in probability through continuous algebraic operations.

### Sandwich covariance matrix

↑ **Parent:** [Asymptotic normality](#asymptotic-normality)

For estimating equations, asymptotic covariance often has the form $A^{-1}BA^{-1}$, called a sandwich covariance.

Regression [heteroskedasticity-consistent standard errors](#heteroskedasticity-consistent-standard-errors) use a specific sandwich covariance estimate; general estimating equations can produce sandwich covariances outside regression.

### Delta method

↑ **Parent:** [Asymptotic normality](#asymptotic-normality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Delta_method)

If $\sqrt n(T_n-\theta)$ is asymptotically normal, differentiability gives $\sqrt n(g(T_n)-g(\theta))$ the variance multiplied by $g'(\theta)^2$.

#### Variance-stabilizing transformation

↑ **Parent:** [Delta method](#delta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variance-stabilizing_transformation)

If a response has mean $\mu$ and [variance](variance.md) $V(\mu)$, the [delta method](#delta-method) gives $\operatorname{Var}(g(Y))\approx g'(\mu)^2V(\mu)$. Choosing $g'(\mu)$ proportional to $V(\mu)^{-1/2}$ makes this first-order [variance](variance.md) independent of $\mu$. For $V(\mu)=k\mu^2$ on positive means, the resulting transformation is the [natural logarithm](calculus.md#natural-logarithm). This is a local approximation and requires the transformation to be defined on the observations; it does not make arbitrary normal responses positive or preserve an exact [normal distribution](probability-distribution.md#normal-distribution).

##### Log absolute value stabilization of a normal scale family

↑ **Parent:** [Variance-stabilizing transformation](#variance-stabilizing-transformation)

For $Y\sim N(\mu,k\mu^2)$ with $\mu\ne0$ and fixed $k>0$, represent $Y=\mu(1+\sqrt{k}Z)$ with $Z$ having the [standard normal distribution](probability-distribution.md#standard-normal-distribution). Taking the [natural logarithm](calculus.md#natural-logarithm) of the absolute value gives the displayed identity. Its random second term has a common distribution, independent of $\mu$, so this [variance-stabilizing transformation](#variance-stabilizing-transformation) gives an exactly constant [variance](variance.md). That variance is finite: the normal density is bounded near zero and $\int_0^1|\log t|^2dt<\infty$, while normal tails control logarithmic growth at infinity. The transformation is defined almost surely, loses the sign of the mean, and does not produce an exact [normal distribution](probability-distribution.md#normal-distribution). A zero mean makes the original observation identically zero and is outside its domain.

#### Functional delta method

↑ **Parent:** [Delta method](#delta-method)

If $r_n(X_n-s)$ converges in distribution to $X$ and $\Phi$ is [Hadamard differentiable](multivariable-calculus.md#hadamard-differentiability) at $s$ tangentially to a space containing the limit, the displayed transformation rule holds under the usual [measurability](measure-theory.md#measurability) and tight separable-support conditions. The variables $X_n$ must belong to the domain of $\Phi$.

#### Asymptotic distribution of the Gaussian sample correlation

↑ **Parent:** [Delta method](#delta-method)

For a centered bivariate normal sample,

$$
\sqrt n(\widehat\rho-\rho)\xrightarrow dN\bigl(0,(1-\rho^2)^2\bigr).
$$

This is the multivariate delta method for $g(a,c,b)=c/\sqrt{ab}$.

### Endpoint asymptotics of the symmetric-uniform maximum likelihood estimator

↑ **Parent:** [Asymptotic normality](#asymptotic-normality)

For an independent sample from $\operatorname{Uniform}[-\theta,\theta]$, the maximum likelihood estimator is $M_n=\max_i|X_i|$ and

$$
n(\theta-M_n)\xrightarrow d\operatorname{Exp}(1/\theta).
$$

The parameter-dependent support makes the convergence rate $n$ rather than $\sqrt n$, so the regular maximum-likelihood central limit theorem does not apply.

## Asymptotic relative efficiency

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_relative_efficiency)

Asymptotic relative efficiency compares the leading asymptotic variances of two consistent estimators.

## Wald confidence interval

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wald_confidence_interval)

A Wald interval centers at an asymptotically normal estimator and uses a consistent estimated standard error times a normal quantile.

## Heteroskedasticity-consistent standard errors

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heteroskedasticity-consistent_standard_errors)

[Heteroskedasticity-consistent standard errors](#heteroskedasticity-consistent-standard-errors) use an estimated regression covariance that remains consistent when error variances vary across observations. For ordinary least squares, the basic sandwich estimate is $(X^TX)^{-1}X^T\operatorname{diag}(\hat\varepsilon_i^2)X(X^TX)^{-1}$. The resulting standard errors are square roots of its diagonal entries. This is a regression application of a [sandwich covariance matrix](#sandwich-covariance-matrix).

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (15)

- [Actuarial statistics](actuarial-statistics.md)
- [Bootstrapping (statistics)](statistical-modelling.md#bootstrapping-statistics)
- [Capture-recapture model](statistical-modelling.md#capture-recapture-model)
- [Empirical distribution function](probability-distribution.md#empirical-distribution-function)
- [GW150914](gravitational-wave.md#gw150914)
- [History of Student's t-distribution](continuous-probability-distribution.md#history-of-student-s-t-distribution)
- [Independent random variables](random-variable.md#independent-random-variables)
- [Mathematical epidemiology](mathematical-biology.md#mathematical-epidemiology)
- [Nonparametric statistics](nonparametric-statistics.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207.md#2/f/solution)
- [Power law](analysis.md#power-law)
- [Prior probability](bayesian-statistics.md#prior-probability)
- [Probability theory](probability-theory.md)
- [Regression toward the mean and randomized comparisons](probability-and-statistics.md#regression-toward-the-mean-and-randomized-comparisons)
- [Statistical inference](statistical-inference.md)
