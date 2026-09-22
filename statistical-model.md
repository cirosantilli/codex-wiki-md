# Statistical model

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_model)

A statistical model is a family of probability distributions proposed for the process that generated observed data.

**Table of contents**

- [Spatial Bernoulli infection model](#spatial-bernoulli-infection-model)
- [Transformation model](#transformation-model)
  - [Equivariant estimator](#equivariant-estimator)
  - [Maximal invariant](#maximal-invariant)
    - [Ranks as a maximal invariant under increasing transformations](#ranks-as-a-maximal-invariant-under-increasing-transformations)
    - [Invariant tests factor through a maximal invariant](#invariant-tests-factor-through-a-maximal-invariant)
- [Parametric statistical model](#parametric-statistical-model)
- [Location-scale family](#location-scale-family)
  - [Log-transformed location-scale model](#log-transformed-location-scale-model)
  - [Conditional inference in a location-scale family](#conditional-inference-in-a-location-scale-family)
- [Regression model](#regression-model)
  - [Interaction (statistics)](#interaction-statistics)
    - [Interaction plot](#interaction-plot)
    - [Interaction term](#interaction-term)
      - [Two-factor interaction](#two-factor-interaction)
      - [Coupling constant (physics)](#coupling-constant-physics)
      - [Principle of marginality](#principle-of-marginality)
- [Statistical path](#statistical-path)
  - [Statistical tangent set](#statistical-tangent-set)
    - [Bounded density tilt](#bounded-density-tilt)
      - [Density of bounded centered scores](#density-of-bounded-centered-scores)
    - [Statistical tangent space](#statistical-tangent-space)
  - [Differentiability in quadratic mean](#differentiability-in-quadratic-mean)
    - [Quadratic-mean to L1 density derivative](#quadratic-mean-to-l1-density-derivative)
    - [Mean-zero score identity under quadratic-mean differentiability](#mean-zero-score-identity-under-quadratic-mean-differentiability)
- [Scale family](#scale-family)
- [Statistical parameter](#statistical-parameter)
  - [Nuisance parameter](#nuisance-parameter)
    - [Mixed log-likelihood derivative obstruction to parameter separation](#mixed-log-likelihood-derivative-obstruction-to-parameter-separation)
- [Covariate](#covariate)
  - [Baseline covariate](#baseline-covariate)
- [Homoscedasticity](#homoscedasticity)
- [Identifiability](#identifiability)
  - [Moment aliasing in a shared zero-inflated count model](#moment-aliasing-in-a-shared-zero-inflated-count-model)
  - [Corner-point constraint](#corner-point-constraint)
- [Location family](#location-family)
  - [Location score](#location-score)
  - [Single-observation location minimax bound](#single-observation-location-minimax-bound)
- [Probabilistic graphical model](#probabilistic-graphical-model)
  - [Junction tree](#junction-tree)
    - [Junction tree algorithm](#junction-tree-algorithm)
    - [Junction-tree sum-product message](#junction-tree-sum-product-message)
    - [Running intersection property](#running-intersection-property)
  - [Bayesian network](#bayesian-network)
    - [Bayesian network structure score](#bayesian-network-structure-score)
    - [Gaussian Bayesian network](#gaussian-bayesian-network)
  - [Belief propagation](#belief-propagation)
    - [Sum-product belief propagation](#sum-product-belief-propagation)
    - [Max-product belief propagation](#max-product-belief-propagation)
  - [Markov blanket](#markov-blanket)
    - [Minimal Markov blanket under faithfulness](#minimal-markov-blanket-under-faithfulness)
    - [Markov blanket D-separation](#markov-blanket-d-separation)
  - [Markov random field](#markov-random-field)
    - [Autologistic binary-image model](#autologistic-binary-image-model)
      - [Gaussian-noise posterior for an autologistic image](#gaussian-noise-posterior-for-an-autologistic-image)
    - [Clique potential](#clique-potential)
    - [Global Markov property for an undirected graph](#global-markov-property-for-an-undirected-graph)
- [Statistical modelling](statistical-modelling.md)
  - [Regression analysis](statistical-modelling.md#regression-analysis)
  - [Mark and recapture](statistical-modelling.md#mark-and-recapture)
    - [Capture-recapture model](statistical-modelling.md#capture-recapture-model)
      - [Missing-count EM for capture-recapture](statistical-modelling.md#missing-count-em-for-capture-recapture)
  - [Nonlinear regression](statistical-modelling.md#nonlinear-regression)
  - [Outlier](statistical-modelling.md#outlier)
  - [Regression to the mean](statistical-modelling.md#regression-to-the-mean)
  - [Response variable](statistical-modelling.md#response-variable)
  - [Scientific control](statistical-modelling.md#scientific-control)
  - [Design of experiments](statistical-modelling.md#design-of-experiments)
    - [Optimal experimental design](statistical-modelling.md#optimal-experimental-design)
      - [General equivalence theorem for optimal design](statistical-modelling.md#general-equivalence-theorem-for-optimal-design)
      - [G-optimal design](statistical-modelling.md#g-optimal-design)
      - [D-optimal design](statistical-modelling.md#d-optimal-design)
      - [Approximate experimental design](statistical-modelling.md#approximate-experimental-design)
        - [Information matrix of an experimental design](statistical-modelling.md#information-matrix-of-an-experimental-design)
          - [Design sensitivity function](statistical-modelling.md#design-sensitivity-function)
    - [Latin square](statistical-modelling.md#latin-square)
      - [Analysis of variance for a Latin square](statistical-modelling.md#analysis-of-variance-for-a-latin-square)
      - [Mutually orthogonal Latin squares](statistical-modelling.md#mutually-orthogonal-latin-squares)
        - [Graeco-Latin square](statistical-modelling.md#graeco-latin-square)
    - [Contrast (statistics)](statistical-modelling.md#contrast-statistics)
    - [Response surface methodology](statistical-modelling.md#response-surface-methodology)
      - [Center-point curvature contrast](statistical-modelling.md#center-point-curvature-contrast)
      - [Steepest ascent in response surface methodology](statistical-modelling.md#steepest-ascent-in-response-surface-methodology)
      - [Coded experimental variable](statistical-modelling.md#coded-experimental-variable)
      - [Rotatable design](statistical-modelling.md#rotatable-design)
      - [Central composite design](statistical-modelling.md#central-composite-design)
    - [Split-plot design](statistical-modelling.md#split-plot-design)
    - [Factorial design](statistical-modelling.md#factorial-design)
      - [Main effect](statistical-modelling.md#main-effect)
      - [Factorial contrast](statistical-modelling.md#factorial-contrast)
      - [Fractional factorial design](statistical-modelling.md#fractional-factorial-design)
        - [Resolution of a fractional factorial design](statistical-modelling.md#resolution-of-a-fractional-factorial-design)
        - [Defining contrast subgroup](statistical-modelling.md#defining-contrast-subgroup)
          - [Aliasing in a fractional factorial design](statistical-modelling.md#aliasing-in-a-fractional-factorial-design)
    - [Crossover design](statistical-modelling.md#crossover-design)
      - [Carryover effect](statistical-modelling.md#carryover-effect)
    - [Completely randomized design](statistical-modelling.md#completely-randomized-design)
    - [Blocks in experimental design](statistical-modelling.md#blocks-in-experimental-design)
      - [Estimability from within-block differences](statistical-modelling.md#estimability-from-within-block-differences)
      - [Block confounding in a factorial design](statistical-modelling.md#block-confounding-in-a-factorial-design)
      - [Block design](statistical-modelling.md#block-design)
        - [Balanced incomplete block design](statistical-modelling.md#balanced-incomplete-block-design)
          - [Symmetric balanced incomplete block design](statistical-modelling.md#symmetric-balanced-incomplete-block-design)
            - [Even-order symmetric design square obstruction](statistical-modelling.md#even-order-symmetric-design-square-obstruction)
          - [Fisher's inequality for block designs](statistical-modelling.md#fisher-s-inequality-for-block-designs)
        - [Row-column design](statistical-modelling.md#row-column-design)
        - [Randomized complete block design](statistical-modelling.md#randomized-complete-block-design)
        - [Orthogonal block design](statistical-modelling.md#orthogonal-block-design)
    - [Replication in experimental design](statistical-modelling.md#replication-in-experimental-design)
      - [Replicate](statistical-modelling.md#replicate)
    - [Experimental unit](statistical-modelling.md#experimental-unit)
      - [Observational unit](statistical-modelling.md#observational-unit)
  - [Fractional polynomial](statistical-modelling.md#fractional-polynomial)
  - [Restricted cubic spline](statistical-modelling.md#restricted-cubic-spline)
  - [Quantile regression](statistical-modelling.md#quantile-regression)
    - [Conditional quantile identification](statistical-modelling.md#conditional-quantile-identification)
    - [Check loss](statistical-modelling.md#check-loss)
      - [Population quantiles minimize check loss](statistical-modelling.md#population-quantiles-minimize-check-loss)
  - [Observed heterogeneity](statistical-modelling.md#observed-heterogeneity)
  - [Pairwise comparison model](statistical-modelling.md#pairwise-comparison-model)
    - [Bradley-Terry model](statistical-modelling.md#bradley-terry-model)
      - [Bradley-Terry score equation](statistical-modelling.md#bradley-terry-score-equation)
        - [Bradley-Terry maximum-likelihood estimate on a comparison tree](statistical-modelling.md#bradley-terry-maximum-likelihood-estimate-on-a-comparison-tree)
          - [Bradley-Terry maximum-likelihood estimate on a path](statistical-modelling.md#bradley-terry-maximum-likelihood-estimate-on-a-path)
          - [Edge log-ratios in a Bradley-Terry comparison tree](statistical-modelling.md#edge-log-ratios-in-a-bradley-terry-comparison-tree)
        - [Three-player Bradley-Terry comparison cycle](statistical-modelling.md#three-player-bradley-terry-comparison-cycle)
        - [Bradley-Terry likelihood Hessian](statistical-modelling.md#bradley-terry-likelihood-hessian)
  - [Fixed effect](statistical-modelling.md#fixed-effect)
  - [Geostatistics](statistical-modelling.md#geostatistics)
    - [Kriging](statistical-modelling.md#kriging)
      - [Universal kriging](statistical-modelling.md#universal-kriging)
      - [Ordinary kriging](statistical-modelling.md#ordinary-kriging)
      - [Simple kriging](statistical-modelling.md#simple-kriging)
    - [Covariogram](statistical-modelling.md#covariogram)
    - [Intrinsically stationary random field](statistical-modelling.md#intrinsically-stationary-random-field)
      - [Semivariogram](statistical-modelling.md#semivariogram)
        - [Empirical semivariogram](statistical-modelling.md#empirical-semivariogram)
        - [Range of a semivariogram](statistical-modelling.md#range-of-a-semivariogram)
          - [Practical range](statistical-modelling.md#practical-range)
        - [Sill of a semivariogram](statistical-modelling.md#sill-of-a-semivariogram)
        - [Nugget effect](statistical-modelling.md#nugget-effect)
        - [A semivariogram does not determine stationarity](statistical-modelling.md#a-semivariogram-does-not-determine-stationarity)
        - [Gaussian semivariogram](statistical-modelling.md#gaussian-semivariogram)
  - [Saturated statistical model](statistical-modelling.md#saturated-statistical-model)
    - [Bernoulli saturated log-likelihood](statistical-modelling.md#bernoulli-saturated-log-likelihood)
  - [Hurdle model](statistical-modelling.md#hurdle-model)
  - [Zero inflation](statistical-modelling.md#zero-inflation)
    - [Count-mixture structural zero](statistical-modelling.md#count-mixture-structural-zero)
    - [Zero-inflated negative binomial model](statistical-modelling.md#zero-inflated-negative-binomial-model)
      - [Shared zero-inflated Gamma-Poisson count model](statistical-modelling.md#shared-zero-inflated-gamma-poisson-count-model)
        - [Mean-ratio preservation under a multiplicative random effect](statistical-modelling.md#mean-ratio-preservation-under-a-multiplicative-random-effect)
      - [EM for zero-inflated negative binomial regression](statistical-modelling.md#em-for-zero-inflated-negative-binomial-regression)
  - [Estimator](statistical-modelling.md#estimator)
    - [Method of moments (statistics)](statistical-modelling.md#method-of-moments-statistics)
    - [U-statistic](statistical-modelling.md#u-statistic)
      - [Influence function of a U-statistic](statistical-modelling.md#influence-function-of-a-u-statistic)
      - [Kernel of a U-statistic](statistical-modelling.md#kernel-of-a-u-statistic)
      - [Variance as a U-statistic](statistical-modelling.md#variance-as-a-u-statistic)
      - [Symmetrization of a U-statistic kernel](statistical-modelling.md#symmetrization-of-a-u-statistic-kernel)
      - [U-statistic central limit theorem](statistical-modelling.md#u-statistic-central-limit-theorem)
        - [Hoeffding projection](statistical-modelling.md#hoeffding-projection)
  - [Categorical variable](statistical-modelling.md#categorical-variable)
    - [Regression factor](statistical-modelling.md#regression-factor)
    - [Ordinal categorical variable](statistical-modelling.md#ordinal-categorical-variable)
    - [Indicator variable](statistical-modelling.md#indicator-variable)
  - [Latent variable](statistical-modelling.md#latent-variable)
    - [Unobserved heterogeneity](statistical-modelling.md#unobserved-heterogeneity)
    - [Factor analysis](statistical-modelling.md#factor-analysis)
      - [Latent factor](statistical-modelling.md#latent-factor)
      - [Orthogonal factor model](statistical-modelling.md#orthogonal-factor-model)
        - [Factor rotation](statistical-modelling.md#factor-rotation)
          - [Varimax rotation](statistical-modelling.md#varimax-rotation)
        - [Communality](statistical-modelling.md#communality)
        - [Factor loading](statistical-modelling.md#factor-loading)
      - [EM update for a single-factor Gaussian model](statistical-modelling.md#em-update-for-a-single-factor-gaussian-model)
    - [Random effect](statistical-modelling.md#random-effect)
      - [Poisson-lognormal random-effect model](statistical-modelling.md#poisson-lognormal-random-effect-model)
      - [Crossed random effects](statistical-modelling.md#crossed-random-effects)
      - [Random slope](statistical-modelling.md#random-slope)
        - [Between-person slope quantile](statistical-modelling.md#between-person-slope-quantile)
        - [Random-slope linear mixed model](statistical-modelling.md#random-slope-linear-mixed-model)
    - [Expectation-maximization algorithm](statistical-modelling.md#expectation-maximization-algorithm)
      - [Ordered-rate exponential M-step](statistical-modelling.md#ordered-rate-exponential-m-step)
      - [EM for merged multinomial cells](statistical-modelling.md#em-for-merged-multinomial-cells)
      - [EM for an independent missing normal coordinate](statistical-modelling.md#em-for-an-independent-missing-normal-coordinate)
      - [EM transition-count update on a tree](statistical-modelling.md#em-transition-count-update-on-a-tree)
      - [EM for a missing observation in a Gaussian AR1 process](statistical-modelling.md#em-for-a-missing-observation-in-a-gaussian-ar1-process)
      - [EM likelihood monotonicity](statistical-modelling.md#em-likelihood-monotonicity)
  - [Functional data analysis](statistical-modelling.md#functional-data-analysis)
    - [Functional time warping](statistical-modelling.md#functional-time-warping)
      - [Square-root velocity function](statistical-modelling.md#square-root-velocity-function)
    - [Functional principal component analysis](statistical-modelling.md#functional-principal-component-analysis)
      - [Principal component function](statistical-modelling.md#principal-component-function)
      - [Functional principal component score](statistical-modelling.md#functional-principal-component-score)
      - [Karhunen–Loève expansion](statistical-modelling.md#karhunen-loeve-expansion)
        - [Brownian half-integer sine expansion](statistical-modelling.md#brownian-half-integer-sine-expansion)
    - [Functional mean test](statistical-modelling.md#functional-mean-test)
      - [FPCA mean test](statistical-modelling.md#fpca-mean-test)
        - [Two-sample FPCA mean statistic](statistical-modelling.md#two-sample-fpca-mean-statistic)
    - [Covariance-operator distance](statistical-modelling.md#covariance-operator-distance)
      - [Hilbert-Schmidt distance between covariance operators](statistical-modelling.md#hilbert-schmidt-distance-between-covariance-operators)
      - [Square-root distance between covariance operators](statistical-modelling.md#square-root-distance-between-covariance-operators)
        - [Square-root barycenter of covariance operators](statistical-modelling.md#square-root-barycenter-of-covariance-operators)
      - [Procrustes distance between covariance operators](statistical-modelling.md#procrustes-distance-between-covariance-operators)
    - [Functional linear model](statistical-modelling.md#functional-linear-model)
      - [Scalar-on-function linear model](statistical-modelling.md#scalar-on-function-linear-model)
        - [Roughness penalty matrix](statistical-modelling.md#roughness-penalty-matrix)
      - [Function-on-function linear model](statistical-modelling.md#function-on-function-linear-model)
        - [Cross-covariance operator](statistical-modelling.md#cross-covariance-operator)
  - [Goodness of fit](statistical-modelling.md#goodness-of-fit)
    - [Goodness-of-fit test](statistical-modelling.md#goodness-of-fit-test)
  - [Contingency table](statistical-modelling.md#contingency-table)
    - [Two-by-two contingency table](statistical-modelling.md#two-by-two-contingency-table)
  - [Mixture model](statistical-modelling.md#mixture-model)
    - [Threshold inference for a mixture proportion](statistical-modelling.md#threshold-inference-for-a-mixture-proportion)
    - [Gaussian scale mixture](statistical-modelling.md#gaussian-scale-mixture)
      - [Rayleigh-normal scale mixture](statistical-modelling.md#rayleigh-normal-scale-mixture)
    - [Finite mixture model](statistical-modelling.md#finite-mixture-model)
      - [Label switching](statistical-modelling.md#label-switching)
      - [Gaussian mixture Gibbs updates with independent priors](statistical-modelling.md#gaussian-mixture-gibbs-updates-with-independent-priors)
      - [Mixture responsibility](statistical-modelling.md#mixture-responsibility)
      - [Finite Gaussian mixture with a common variance](statistical-modelling.md#finite-gaussian-mixture-with-a-common-variance)
        - [Mixture regression with shared slopes](statistical-modelling.md#mixture-regression-with-shared-slopes)
        - [Residual mixture clustering](statistical-modelling.md#residual-mixture-clustering)
          - [Two-stage residual mixture fitting](statistical-modelling.md#two-stage-residual-mixture-fitting)
        - [EM for Gaussian mixtures with a common variance](statistical-modelling.md#em-for-gaussian-mixtures-with-a-common-variance)
      - [Mixture weight](statistical-modelling.md#mixture-weight)
    - [Dirichlet process mixture model](statistical-modelling.md#dirichlet-process-mixture-model)
  - [Latent-variable model](statistical-modelling.md#latent-variable-model)
  - [Statistical learning](statistical-learning.md)
    - [Unsupervised learning](statistical-learning.md#unsupervised-learning)
      - [Multidimensional scaling](statistical-learning.md#multidimensional-scaling)
        - [Classical multidimensional scaling](statistical-learning.md#classical-multidimensional-scaling)
          - [Euclidean distance matrix criterion](statistical-learning.md#euclidean-distance-matrix-criterion)
      - [Sparse coding](statistical-learning.md#sparse-coding)
      - [Hebbian learning](statistical-learning.md#hebbian-learning)
        - [Quartic norm stabilization of Hebbian learning](statistical-learning.md#quartic-norm-stabilization-of-hebbian-learning)
        - [Oja's rule](statistical-learning.md#oja-s-rule)
          - [Stability and normalization of averaged Oja learning](statistical-learning.md#stability-and-normalization-of-averaged-oja-learning)
    - [Cluster analysis](statistical-learning.md#cluster-analysis)
      - [Cluster in cluster analysis](statistical-learning.md#cluster-in-cluster-analysis)
      - [K-means clustering](statistical-learning.md#k-means-clustering)
      - [Jaccard index](statistical-learning.md#jaccard-index)
        - [Jaccard distance](statistical-learning.md#jaccard-distance)
      - [Dissimilarity matrix](statistical-learning.md#dissimilarity-matrix)
      - [Simple matching coefficient](statistical-learning.md#simple-matching-coefficient)
        - [Metric property of simple matching dissimilarity](statistical-learning.md#metric-property-of-simple-matching-dissimilarity)
      - [Agglomerative hierarchical clustering](statistical-learning.md#agglomerative-hierarchical-clustering)
        - [Ward minimum-variance clustering](statistical-learning.md#ward-minimum-variance-clustering)
        - [Average-linkage clustering](statistical-learning.md#average-linkage-clustering)
        - [Agglomerative clustering of nonmetric dissimilarities](statistical-learning.md#agglomerative-clustering-of-nonmetric-dissimilarities)
        - [Dendrogram](statistical-learning.md#dendrogram)
        - [Complete-linkage clustering](statistical-learning.md#complete-linkage-clustering)
        - [Single-linkage clustering](statistical-learning.md#single-linkage-clustering)
    - [Validation set](statistical-learning.md#validation-set)
      - [Test set](statistical-learning.md#test-set)
    - [Prediction error](statistical-learning.md#prediction-error)
      - [Test error](statistical-learning.md#test-error)
      - [Mean squared prediction error](statistical-learning.md#mean-squared-prediction-error)
    - [Training error](statistical-learning.md#training-error)
      - [Prediction optimism](statistical-learning.md#prediction-optimism)
        - [Covariance formula for prediction optimism](statistical-learning.md#covariance-formula-for-prediction-optimism)
    - [Data leakage](statistical-learning.md#data-leakage)
    - [Dataset shift](statistical-learning.md#dataset-shift)
    - [Regression function](statistical-learning.md#regression-function)
    - [Principal component analysis](statistical-learning.md#principal-component-analysis)
      - [Principal component regression](statistical-learning.md#principal-component-regression)
      - [Scree plot](statistical-learning.md#scree-plot)
      - [Principal component loading](statistical-learning.md#principal-component-loading)
      - [Principal component](statistical-learning.md#principal-component)
        - [Principal component score](statistical-learning.md#principal-component-score)
      - [Explained variance of a principal component](statistical-learning.md#explained-variance-of-a-principal-component)
      - [Principal component analysis on a correlation matrix](statistical-learning.md#principal-component-analysis-on-a-correlation-matrix)
      - [Population principal component](statistical-learning.md#population-principal-component)
      - [Sample principal component](statistical-learning.md#sample-principal-component)
        - [Normalized sample principal component](statistical-learning.md#normalized-sample-principal-component)
    - [Classification in statistical learning](statistical-learning.md#classification-in-statistical-learning)
      - [Misclassification rate](statistical-learning.md#misclassification-rate)
      - [Classification tree](statistical-learning.md#classification-tree)
        - [Cost-complexity tree pruning](statistical-learning.md#cost-complexity-tree-pruning)
        - [Classification-tree deviance](statistical-learning.md#classification-tree-deviance)
      - [Binary classification](statistical-learning.md#binary-classification)
        - [False positive rate](statistical-learning.md#false-positive-rate)
      - [Decision boundary](statistical-learning.md#decision-boundary)
        - [Bayes decision boundary](statistical-learning.md#bayes-decision-boundary)
      - [Majority vote](statistical-learning.md#majority-vote)
      - [Confusion matrix](statistical-learning.md#confusion-matrix)
      - [Classification and regression tree](statistical-learning.md#classification-and-regression-tree)
        - [Recursive partitioning](statistical-learning.md#recursive-partitioning)
          - [Surrogate split](statistical-learning.md#surrogate-split)
        - [Gini impurity](statistical-learning.md#gini-impurity)
        - [Random forest](statistical-learning.md#random-forest)
          - [Out-of-bag error](statistical-learning.md#out-of-bag-error)
      - [Conditional class probability](statistical-learning.md#conditional-class-probability)
      - [Risk consistency](statistical-learning.md#risk-consistency)
      - [K-nearest neighbors algorithm](statistical-learning.md#k-nearest-neighbors-algorithm)
        - [Bias and variance of a three-neighbour weighted smoother](statistical-learning.md#bias-and-variance-of-a-three-neighbour-weighted-smoother)
        - [One-nearest-neighbour classifier](statistical-learning.md#one-nearest-neighbour-classifier)
          - [One-nearest-neighbour asymptotic risk](statistical-learning.md#one-nearest-neighbour-asymptotic-risk)
            - [Bayes risk bound for one-nearest-neighbour classification](statistical-learning.md#bayes-risk-bound-for-one-nearest-neighbour-classification)
        - [Feature-measurable nearest-neighbour tie-breaking](statistical-learning.md#feature-measurable-nearest-neighbour-tie-breaking)
        - [L-nearest-neighbour classifier](statistical-learning.md#l-nearest-neighbour-classifier)
          - [One-nearest-neighbour classification](statistical-learning.md#one-nearest-neighbour-classification)
      - [Plug-in classifier excess-risk bound](statistical-learning.md#plug-in-classifier-excess-risk-bound)
      - [Support vector machine](statistical-learning.md#support-vector-machine)
        - [Kernel support vector machine](statistical-learning.md#kernel-support-vector-machine)
        - [Soft-margin support vector machine](statistical-learning.md#soft-margin-support-vector-machine)
          - [Kernel support-vector coefficient from hinge activity](statistical-learning.md#kernel-support-vector-coefficient-from-hinge-activity)
          - [Support-vector leave-one-out error bound](statistical-learning.md#support-vector-leave-one-out-error-bound)
          - [Dual support vectors and margin degeneracy](statistical-learning.md#dual-support-vectors-and-margin-degeneracy)
        - [Separating hyperplane](statistical-learning.md#separating-hyperplane)
        - [Slack variables of a support vector machine](statistical-learning.md#slack-variables-of-a-support-vector-machine)
        - [Support-vector-machine decision boundary](statistical-learning.md#support-vector-machine-decision-boundary)
        - [Support-vector-machine margin](statistical-learning.md#support-vector-machine-margin)
          - [Support-vector-machine margin boundaries](statistical-learning.md#support-vector-machine-margin-boundaries)
        - [Support vector](statistical-learning.md#support-vector)
      - [Perceptron](statistical-learning.md#perceptron)
    - [Cross-validation](statistical-learning.md#cross-validation)
      - [Biased cross-validation for density bandwidth](statistical-learning.md#biased-cross-validation-for-density-bandwidth)
      - [Least-squares cross-validation for density bandwidth](statistical-learning.md#least-squares-cross-validation-for-density-bandwidth)
      - [Generalized cross-validation](statistical-learning.md#generalized-cross-validation)
      - [Leave-one-out cross-validation](statistical-learning.md#leave-one-out-cross-validation)
        - [Leave-one-out residual identity for a linear smoother](statistical-learning.md#leave-one-out-residual-identity-for-a-linear-smoother)
      - [K-fold cross-validation](statistical-learning.md#k-fold-cross-validation)
    - [Neural network](statistical-learning.md#neural-network)
      - [Binary threshold unit](statistical-learning.md#binary-threshold-unit)
      - [Activation function](statistical-learning.md#activation-function)
      - [Hopfield network](statistical-learning.md#hopfield-network)
        - [Asynchronous Hopfield energy descent](statistical-learning.md#asynchronous-hopfield-energy-descent)
        - [Hebbian memory weights for a Hopfield network](statistical-learning.md#hebbian-memory-weights-for-a-hopfield-network)
      - [Feedforward neural network](statistical-learning.md#feedforward-neural-network)
        - [Four-input parity network](statistical-learning.md#four-input-parity-network)
        - [Hidden unit](statistical-learning.md#hidden-unit)
        - [Backpropagation](statistical-learning.md#backpropagation)
          - [Squared-error backpropagation](statistical-learning.md#squared-error-backpropagation)
          - [Sigmoid-softmax network gradients](statistical-learning.md#sigmoid-softmax-network-gradients)
      - [Sigmoid function](statistical-learning.md#sigmoid-function)
        - [Logistic function](statistical-learning.md#logistic-function)
      - [Rectified linear unit](statistical-learning.md#rectified-linear-unit)
      - [Gaussian error linear unit](statistical-learning.md#gaussian-error-linear-unit)
      - [Softmax function](statistical-learning.md#softmax-function)
        - [Softmax non-identifiability](statistical-learning.md#softmax-non-identifiability)
        - [Categorical cross-entropy loss](statistical-learning.md#categorical-cross-entropy-loss)
    - [Overfitting](statistical-learning.md#overfitting)
    - [Regularization](statistical-learning.md#regularization)
      - [Penalized least squares](statistical-learning.md#penalized-least-squares)
        - [Penalized least-squares estimator](statistical-learning.md#penalized-least-squares-estimator)
          - [Basic inequality for a penalized least-squares estimator](statistical-learning.md#basic-inequality-for-a-penalized-least-squares-estimator)
      - [Roughness penalty](statistical-learning.md#roughness-penalty)
      - [Early stopping](statistical-learning.md#early-stopping)
  - [Sampling distribution](statistical-modelling.md#sampling-distribution)
  - [Unbiased estimator](statistical-modelling.md#unbiased-estimator)
    - [Unbiased endpoint estimator for a shifted exponential sample](statistical-modelling.md#unbiased-endpoint-estimator-for-a-shifted-exponential-sample)
    - [Uniformly minimum-variance unbiased estimator](statistical-modelling.md#uniformly-minimum-variance-unbiased-estimator)
    - [Conditionally unbiased estimator](statistical-modelling.md#conditionally-unbiased-estimator)
      - [Uniform minimum variance conditionally unbiased estimator](statistical-modelling.md#uniform-minimum-variance-conditionally-unbiased-estimator)
    - [Linear unbiased estimator](statistical-modelling.md#linear-unbiased-estimator)
      - [Best linear unbiased estimator](statistical-modelling.md#best-linear-unbiased-estimator)
      - [Correlated Gaussian common-mean estimator](statistical-modelling.md#correlated-gaussian-common-mean-estimator)
      - [Inverse-variance weighted mean](statistical-modelling.md#inverse-variance-weighted-mean)
        - [Inverse-variance weight](statistical-modelling.md#inverse-variance-weight)
  - [Bias of an estimator](statistical-modelling.md#bias-of-an-estimator)
  - [Variance of an estimator](statistical-modelling.md#variance-of-an-estimator)
    - [Asymptotic variance](statistical-modelling.md#asymptotic-variance)
    - [Bias-variance tradeoff](statistical-modelling.md#bias-variance-tradeoff)
  - [Homoskedasticity](statistical-modelling.md#homoskedasticity)
  - [Homoscedasticity and heteroscedasticity](statistical-modelling.md#homoscedasticity-and-heteroscedasticity)
    - [Heteroscedastic](statistical-modelling.md#heteroscedastic)
  - [Logarithmic transformation](statistical-modelling.md#logarithmic-transformation)
    - [Gaussian log-response model](statistical-modelling.md#gaussian-log-response-model)
    - [Retransformation bias](statistical-modelling.md#retransformation-bias)
  - [Power transform](statistical-modelling.md#power-transform)
    - [Box–Cox transformation](statistical-modelling.md#box-cox-transformation)
      - [Bias correction after an inverse transformation](statistical-modelling.md#bias-correction-after-an-inverse-transformation)
  - [Residual degrees of freedom](statistical-modelling.md#residual-degrees-of-freedom)
  - [Model selection](statistical-modelling.md#model-selection)
    - [Deviance information criterion](statistical-modelling.md#deviance-information-criterion)
      - [Effective parameter count in DIC](statistical-modelling.md#effective-parameter-count-in-dic)
        - [Quadratic posterior deviance moments](statistical-modelling.md#quadratic-posterior-deviance-moments)
    - [Variable selection](statistical-modelling.md#variable-selection)
    - [Nonregular mixture model selection](statistical-modelling.md#nonregular-mixture-model-selection)
    - [Akaike information criterion](statistical-modelling.md#akaike-information-criterion)
      - [Stepwise selection by the Akaike information criterion](statistical-modelling.md#stepwise-selection-by-the-akaike-information-criterion)
        - [AIC deletion threshold in a normal linear model](statistical-modelling.md#aic-deletion-threshold-in-a-normal-linear-model)
      - [Distribution of the Akaike information criterion in a normal linear model](statistical-modelling.md#distribution-of-the-akaike-information-criterion-in-a-normal-linear-model)
      - [Mallows's Cp](statistical-modelling.md#mallows-s-cp)
        - [Bias-variance decomposition for linear prediction](statistical-modelling.md#bias-variance-decomposition-for-linear-prediction)
        - [Unbiased prediction-error identity for ordinary least squares](statistical-modelling.md#unbiased-prediction-error-identity-for-ordinary-least-squares)
    - [Bayesian information criterion](statistical-modelling.md#bayesian-information-criterion)
  - [Shape parameter](statistical-modelling.md#shape-parameter)
  - [Precision parameter](statistical-modelling.md#precision-parameter)
  - [Exponential family](exponential-family.md)
    - [Curved exponential family](exponential-family.md#curved-exponential-family)
      - [Conditional scale density in a curved Gaussian family](exponential-family.md#conditional-scale-density-in-a-curved-gaussian-family)
    - [Minimal exponential family](exponential-family.md#minimal-exponential-family)
    - [Natural exponential family](exponential-family.md#natural-exponential-family)
      - [Convex support of an exponential family](exponential-family.md#convex-support-of-an-exponential-family)
      - [Regular natural exponential family](exponential-family.md#regular-natural-exponential-family)
      - [Full natural exponential family](exponential-family.md#full-natural-exponential-family)
        - [Maximum likelihood existence in a full regular natural exponential family](exponential-family.md#maximum-likelihood-existence-in-a-full-regular-natural-exponential-family)
    - [Normal natural-mean parameter ratio estimator](exponential-family.md#normal-natural-mean-parameter-ratio-estimator)
    - [Log-density domination in an exponential family](exponential-family.md#log-density-domination-in-an-exponential-family)
    - [Conjugate prior](exponential-family.md#conjugate-prior)
      - [Normal-gamma distribution](exponential-family.md#normal-gamma-distribution)
      - [Gamma rate gamma conjugacy](exponential-family.md#gamma-rate-gamma-conjugacy)
      - [Uniform-Pareto conjugacy](exponential-family.md#uniform-pareto-conjugacy)
        - [Uniform-Pareto model evidence](exponential-family.md#uniform-pareto-model-evidence)
      - [Gamma scale inverse-gamma conjugacy](exponential-family.md#gamma-scale-inverse-gamma-conjugacy)
        - [Exact Bühlmann credibility for gamma claims](exponential-family.md#exact-buhlmann-credibility-for-gamma-claims)
      - [Normal-inverse-gamma prior](exponential-family.md#normal-inverse-gamma-prior)
      - [Natural conjugate prior](exponential-family.md#natural-conjugate-prior)
        - [Natural conjugate credibility identity](exponential-family.md#natural-conjugate-credibility-identity)
          - [Endpoint control for a Laplace-family conjugate posterior](exponential-family.md#endpoint-control-for-a-laplace-family-conjugate-posterior)
    - [Natural parameter of an exponential family](exponential-family.md#natural-parameter-of-an-exponential-family)
      - [Natural parameter space](exponential-family.md#natural-parameter-space)
    - [Cumulant function of an exponential family](exponential-family.md#cumulant-function-of-an-exponential-family)
      - [Exponential-family derivative identities](exponential-family.md#exponential-family-derivative-identities)
      - [Mean parameter of an exponential family](exponential-family.md#mean-parameter-of-an-exponential-family)
        - [Interior moment matching in a finite exponential family](exponential-family.md#interior-moment-matching-in-a-finite-exponential-family)
    - [Inverse Gaussian distribution](exponential-family.md#inverse-gaussian-distribution)
      - [Inverse Gaussian shape estimation and nuisance orthogonality](exponential-family.md#inverse-gaussian-shape-estimation-and-nuisance-orthogonality)
      - [Inverse Gaussian sum closure](exponential-family.md#inverse-gaussian-sum-closure)
        - [Exact saddlepoint density of an inverse Gaussian sum](exponential-family.md#exact-saddlepoint-density-of-an-inverse-gaussian-sum)
      - [Chi-squared transform of an inverse Gaussian variable](exponential-family.md#chi-squared-transform-of-an-inverse-gaussian-variable)
      - [Reciprocal-root inverse Gaussian sampler](exponential-family.md#reciprocal-root-inverse-gaussian-sampler)
        - [Stable root evaluation for inverse Gaussian sampling](exponential-family.md#stable-root-evaluation-for-inverse-gaussian-sampling)
    - [Exponential-family deviance](exponential-family.md#exponential-family-deviance)
      - [Scaled deviance](exponential-family.md#scaled-deviance)
    - [Negative binomial exponential family](exponential-family.md#negative-binomial-exponential-family)
    - [Exponential dispersion model](exponential-family.md#exponential-dispersion-model)
      - [Exponential dispersion family of order one](exponential-family.md#exponential-dispersion-family-of-order-one)
      - [Dispersion parameter](exponential-family.md#dispersion-parameter)
        - [Underdispersion](exponential-family.md#underdispersion)
        - [Overdispersion](exponential-family.md#overdispersion)
      - [Variance function](exponential-family.md#variance-function)
  - [Generalized linear model](statistical-modelling.md#generalized-linear-model)
    - [Gamma regression with canonical link](statistical-modelling.md#gamma-regression-with-canonical-link)
    - [Generalized linear model offset](statistical-modelling.md#generalized-linear-model-offset)
    - [Deviance goodness-of-fit test](statistical-modelling.md#deviance-goodness-of-fit-test)
      - [Individual Bernoulli deviance need not have a chi-squared calibration](statistical-modelling.md#individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration)
    - [Deviance residual](statistical-modelling.md#deviance-residual)
    - [Generalized additive model](statistical-modelling.md#generalized-additive-model)
      - [Additive regression model](statistical-modelling.md#additive-regression-model)
        - [Identifiability of additive regression components](statistical-modelling.md#identifiability-of-additive-regression-components)
          - [Concurvity](statistical-modelling.md#concurvity)
      - [Backfitting algorithm](statistical-modelling.md#backfitting-algorithm)
        - [Linear backfitting equations](statistical-modelling.md#linear-backfitting-equations)
      - [Generalized additive mixed model](statistical-modelling.md#generalized-additive-mixed-model)
    - [Quasi-likelihood](statistical-modelling.md#quasi-likelihood)
      - [Quasibinomial regression](statistical-modelling.md#quasibinomial-regression)
    - [Linear predictor](statistical-modelling.md#linear-predictor)
    - [Link function](statistical-modelling.md#link-function)
      - [Identity link](statistical-modelling.md#identity-link)
      - [Logit](statistical-modelling.md#logit)
      - [Logarithmic link function](statistical-modelling.md#logarithmic-link-function)
    - [Binomial regression](statistical-modelling.md#binomial-regression)
      - [Binomial deviance](statistical-modelling.md#binomial-deviance)
    - [Pearson dispersion estimator](statistical-modelling.md#pearson-dispersion-estimator)
      - [Pearson residual](statistical-modelling.md#pearson-residual)
      - [Pearson chi-squared statistic](statistical-modelling.md#pearson-chi-squared-statistic)
    - [Canonical link function](statistical-modelling.md#canonical-link-function)
      - [Poisson canonical link](statistical-modelling.md#poisson-canonical-link)
    - [Poisson regression](statistical-modelling.md#poisson-regression)
      - [Profile likelihood for a common Poisson rate ratio with unequal exposures](statistical-modelling.md#profile-likelihood-for-a-common-poisson-rate-ratio-with-unequal-exposures)
      - [Concavity of the Poisson regression likelihood](statistical-modelling.md#concavity-of-the-poisson-regression-likelihood)
      - [Poisson slope information after eliminating an intercept](statistical-modelling.md#poisson-slope-information-after-eliminating-an-intercept)
      - [Poisson regression margin-matching score equations](statistical-modelling.md#poisson-regression-margin-matching-score-equations)
      - [Two-group Poisson ratio conditional likelihood](statistical-modelling.md#two-group-poisson-ratio-conditional-likelihood)
        - [Paired Poisson conditional likelihood](statistical-modelling.md#paired-poisson-conditional-likelihood)
          - [Conditional cure-weight equations for paired Poisson counts](statistical-modelling.md#conditional-cure-weight-equations-for-paired-poisson-counts)
      - [Common versus factor-specific slopes in Poisson regression](statistical-modelling.md#common-versus-factor-specific-slopes-in-poisson-regression)
      - [Poisson working models for averaged counts](statistical-modelling.md#poisson-working-models-for-averaged-counts)
      - [Poisson log-rate ratio](statistical-modelling.md#poisson-log-rate-ratio)
      - [Poisson mean saturation at three distinct times](statistical-modelling.md#poisson-mean-saturation-at-three-distinct-times)
      - [Pooling selected slopes in a Poisson regression](statistical-modelling.md#pooling-selected-slopes-in-a-poisson-regression)
      - [Treatment interaction contrast in a Poisson regression](statistical-modelling.md#treatment-interaction-contrast-in-a-poisson-regression)
      - [Poisson deviance](statistical-modelling.md#poisson-deviance)
        - [Quadratic Pearson approximation to the Poisson deviance](statistical-modelling.md#quadratic-pearson-approximation-to-the-poisson-deviance)
        - [Poisson deviance simplifies when an intercept is fitted](statistical-modelling.md#poisson-deviance-simplifies-when-an-intercept-is-fitted)
    - [Gamma regression with logarithmic link](statistical-modelling.md#gamma-regression-with-logarithmic-link)
    - [Quasi-Poisson regression](statistical-modelling.md#quasi-poisson-regression)
      - [Poisson score linearization under proportional variance](statistical-modelling.md#poisson-score-linearization-under-proportional-variance)
      - [Quasi-score equation](statistical-modelling.md#quasi-score-equation)
    - [Negative binomial regression](statistical-modelling.md#negative-binomial-regression)
      - [Fixed-size negative binomial generalized linear model](statistical-modelling.md#fixed-size-negative-binomial-generalized-linear-model)
        - [Negative binomial deviance](statistical-modelling.md#negative-binomial-deviance)
    - [Poisson exposure model](statistical-modelling.md#poisson-exposure-model)
      - [Rate ratio](statistical-modelling.md#rate-ratio)
      - [Finite-exposure Poisson inconsistency](statistical-modelling.md#finite-exposure-poisson-inconsistency)
      - [Estimators for a Poisson exposure model](statistical-modelling.md#estimators-for-a-poisson-exposure-model)
        - [Variance comparison for Poisson exposure estimators](statistical-modelling.md#variance-comparison-for-poisson-exposure-estimators)
      - [Normal-approximation tests for a Poisson exposure model](statistical-modelling.md#normal-approximation-tests-for-a-poisson-exposure-model)
    - [Logistic regression](statistical-modelling.md#logistic-regression)
      - [Proportional-odds model](statistical-modelling.md#proportional-odds-model)
      - [Separation in logistic regression](statistical-modelling.md#separation-in-logistic-regression)
      - [Finite maximum-likelihood estimate in a one-parameter logistic model](statistical-modelling.md#finite-maximum-likelihood-estimate-in-a-one-parameter-logistic-model)
      - [Conditional logistic model for longitudinal binary data](statistical-modelling.md#conditional-logistic-model-for-longitudinal-binary-data)
        - [Cumulative-response logistic model](statistical-modelling.md#cumulative-response-logistic-model)
        - [True state dependence](statistical-modelling.md#true-state-dependence)
      - [Multinomial logistic regression](statistical-modelling.md#multinomial-logistic-regression)
        - [Continuation-ratio logits](statistical-modelling.md#continuation-ratio-logits)
        - [Conditional multinomial sufficient statistics](statistical-modelling.md#conditional-multinomial-sufficient-statistics)
      - [Logistic-normal regression with autoregressive random effects](statistical-modelling.md#logistic-normal-regression-with-autoregressive-random-effects)
      - [Logistic model](statistical-modelling.md#logistic-model)
        - [Log odds](statistical-modelling.md#log-odds)
      - [Separation (statistics)](statistical-modelling.md#separation-statistics)
        - [Quasi-complete separation](statistical-modelling.md#quasi-complete-separation)
        - [Complete separation](statistical-modelling.md#complete-separation)
      - [Bernoulli logistic-regression model](statistical-modelling.md#bernoulli-logistic-regression-model)
        - [Fitted-mean balance for logistic regression with an intercept](statistical-modelling.md#fitted-mean-balance-for-logistic-regression-with-an-intercept)
      - [Logistic loss](statistical-modelling.md#logistic-loss)
        - [Positive semidefinite quadratic-form classifier](statistical-modelling.md#positive-semidefinite-quadratic-form-classifier)
      - [L1-penalized logistic regression](statistical-modelling.md#l1-penalized-logistic-regression)
      - [Grouped-binomial logistic regression](statistical-modelling.md#grouped-binomial-logistic-regression)
        - [Baseline logit estimator in a group-factor binomial model](statistical-modelling.md#baseline-logit-estimator-in-a-group-factor-binomial-model)
        - [Denominators in grouped birth-outcome models](statistical-modelling.md#denominators-in-grouped-birth-outcome-models)
      - [Reference level in a regression factor](statistical-modelling.md#reference-level-in-a-regression-factor)
      - [Stochastic block model](statistical-modelling.md#stochastic-block-model)
        - [Spectral norm bound for a centered Bernoulli adjacency matrix](statistical-modelling.md#spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix)
        - [Logistic stochastic block model](statistical-modelling.md#logistic-stochastic-block-model)
          - [Additive class-effect logistic network model](statistical-modelling.md#additive-class-effect-logistic-network-model)
            - [Degree-sum sufficient statistic for an additive logistic network model](statistical-modelling.md#degree-sum-sufficient-statistic-for-an-additive-logistic-network-model)
    - [Probit model](statistical-modelling.md#probit-model)
      - [Latent-normal Gibbs sampler for probit regression](statistical-modelling.md#latent-normal-gibbs-sampler-for-probit-regression)
      - [Threshold observation of a lognormal regression](statistical-modelling.md#threshold-observation-of-a-lognormal-regression)
      - [Probit posterior score](statistical-modelling.md#probit-posterior-score)
    - [Iteratively reweighted least squares](statistical-modelling.md#iteratively-reweighted-least-squares)
    - [Generalized linear mixed model](statistical-modelling.md#generalized-linear-mixed-model)
      - [Logistic random-intercept model for repeated binary outcomes](statistical-modelling.md#logistic-random-intercept-model-for-repeated-binary-outcomes)
        - [Random-intercept attenuation of marginal logistic slopes](statistical-modelling.md#random-intercept-attenuation-of-marginal-logistic-slopes)
      - [Gaussian linear mixed model](statistical-modelling.md#gaussian-linear-mixed-model)
        - [Correlated random-intercept and random-slope model](statistical-modelling.md#correlated-random-intercept-and-random-slope-model)
        - [Variance component](statistical-modelling.md#variance-component)
          - [Method-of-moments variance component estimate](statistical-modelling.md#method-of-moments-variance-component-estimate)
        - [Best linear unbiased prediction](statistical-modelling.md#best-linear-unbiased-prediction)
        - [Conditional mode of Gaussian random effects](statistical-modelling.md#conditional-mode-of-gaussian-random-effects)
        - [Continuous-time autoregressive residual correlation](statistical-modelling.md#continuous-time-autoregressive-residual-correlation)
        - [Independent random-intercept and random-slope model](statistical-modelling.md#independent-random-intercept-and-random-slope-model)
      - [Poisson generalized linear mixed model](statistical-modelling.md#poisson-generalized-linear-mixed-model)
        - [Gamma random-intercept Poisson model](statistical-modelling.md#gamma-random-intercept-poisson-model)
          - [Scale identifiability in a gamma random-intercept Poisson model](statistical-modelling.md#scale-identifiability-in-a-gamma-random-intercept-poisson-model)
        - [Marginal mean of a Poisson random-slope model](statistical-modelling.md#marginal-mean-of-a-poisson-random-slope-model)
      - [Random intercept](statistical-modelling.md#random-intercept)
        - [Marginal and conditional slopes agree for an independent log-link random intercept](statistical-modelling.md#marginal-and-conditional-slopes-agree-for-an-independent-log-link-random-intercept)
        - [Random-intercept linear mixed model](statistical-modelling.md#random-intercept-linear-mixed-model)
  - [Clustered data](statistical-modelling.md#clustered-data)
    - [Pseudoreplication](statistical-modelling.md#pseudoreplication)
  - [Independent Poisson conditioning](statistical-modelling.md#independent-poisson-conditioning)
  - [Normal linear model](statistical-modelling.md#normal-linear-model)
    - [Variance of a fitted regression mean](statistical-modelling.md#variance-of-a-fitted-regression-mean)
    - [Analysis of covariance](statistical-modelling.md#analysis-of-covariance)
    - [Normal linear model maximum-likelihood sampling distributions](statistical-modelling.md#normal-linear-model-maximum-likelihood-sampling-distributions)
    - [Lack of fit](statistical-modelling.md#lack-of-fit)
      - [Lack-of-fit F-test](statistical-modelling.md#lack-of-fit-f-test)
    - [Pure error](statistical-modelling.md#pure-error)
    - [Two-factor normal linear model](statistical-modelling.md#two-factor-normal-linear-model)
      - [Factor-level pooling test](statistical-modelling.md#factor-level-pooling-test)
    - [Joint distribution of least-squares and variance estimators](statistical-modelling.md#joint-distribution-of-least-squares-and-variance-estimators)
    - [Restricted maximum likelihood](statistical-modelling.md#restricted-maximum-likelihood)
      - [Restricted likelihood from orthogonal error contrasts](statistical-modelling.md#restricted-likelihood-from-orthogonal-error-contrasts)
    - [Gaussian conjugacy for a normal linear model](statistical-modelling.md#gaussian-conjugacy-for-a-normal-linear-model)
      - [Gaussian conjugacy for an initialized AR(2) regression](statistical-modelling.md#gaussian-conjugacy-for-an-initialized-ar-2-regression)
      - [Normal-gamma posterior with a flat prior](statistical-modelling.md#normal-gamma-posterior-with-a-flat-prior)
      - [Gaussian posterior in the zero-noise limit](statistical-modelling.md#gaussian-posterior-in-the-zero-noise-limit)
      - [Gaussian likelihood](statistical-modelling.md#gaussian-likelihood)
    - [Cochran's theorem](statistical-modelling.md#cochran-s-theorem)
      - [Rank-sum form of Cochran's theorem](statistical-modelling.md#rank-sum-form-of-cochran-s-theorem)
    - [Linear regression](linear-regression.md)
      - [Multiple linear regression](linear-regression.md#multiple-linear-regression)
      - [Normal equations for linear least squares](linear-regression.md#normal-equations-for-linear-least-squares)
      - [Omitted-variable bias](linear-regression.md#omitted-variable-bias)
      - [Predictor centering](linear-regression.md#predictor-centering)
      - [Regression diagnostics](linear-regression.md#regression-diagnostics)
        - [Influential observation](linear-regression.md#influential-observation)
        - [Regression outlier](linear-regression.md#regression-outlier)
      - [Least angle regression](linear-regression.md#least-angle-regression)
        - [Equiangular direction in least angle regression](linear-regression.md#equiangular-direction-in-least-angle-regression)
        - [Sign compatibility of LAR and Lasso](linear-regression.md#sign-compatibility-of-lar-and-lasso)
        - [LAR active correlation invariant](linear-regression.md#lar-active-correlation-invariant)
        - [Entry knot in least angle regression](linear-regression.md#entry-knot-in-least-angle-regression)
      - [Reciprocal-predictor regression](linear-regression.md#reciprocal-predictor-regression)
      - [Regression intercept](linear-regression.md#regression-intercept)
        - [Student t test for a simple-regression intercept](linear-regression.md#student-t-test-for-a-simple-regression-intercept)
      - [Polynomial regression](linear-regression.md#polynomial-regression)
        - [Independent normal and inverse-gamma regression priors](linear-regression.md#independent-normal-and-inverse-gamma-regression-priors)
        - [Quadratic regression](linear-regression.md#quadratic-regression)
      - [Coefficient of determination](linear-regression.md#coefficient-of-determination)
        - [Adjusted coefficient of determination](linear-regression.md#adjusted-coefficient-of-determination)
      - [Residual-versus-fitted plot](linear-regression.md#residual-versus-fitted-plot)
        - [Scale-location plot](linear-regression.md#scale-location-plot)
      - [Analysis of variance](linear-regression.md#analysis-of-variance)
        - [Multivariate analysis of variance](linear-regression.md#multivariate-analysis-of-variance)
          - [Within-group and between-group scatter decomposition](linear-regression.md#within-group-and-between-group-scatter-decomposition)
          - [Wilks lambda statistic](linear-regression.md#wilks-lambda-statistic)
        - [Two-way analysis of variance](linear-regression.md#two-way-analysis-of-variance)
          - [Missing cells can destroy factor orthogonality in two-way ANOVA](linear-regression.md#missing-cells-can-destroy-factor-orthogonality-in-two-way-anova)
          - [Identifiability of an incomplete two-factor additive design](linear-regression.md#identifiability-of-an-incomplete-two-factor-additive-design)
          - [Saturation of an unreplicated two-factor regression](linear-regression.md#saturation-of-an-unreplicated-two-factor-regression)
        - [Sequential sum of squares](linear-regression.md#sequential-sum-of-squares)
        - [Sum of squares in ANOVA](linear-regression.md#sum-of-squares-in-anova)
          - [Mean square in ANOVA](linear-regression.md#mean-square-in-anova)
        - [ANOVA stratum](linear-regression.md#anova-stratum)
          - [Within-block ANOVA stratum](linear-regression.md#within-block-anova-stratum)
        - [Balanced factorial orthogonality](linear-regression.md#balanced-factorial-orthogonality)
      - [Frisch–Waugh–Lovell theorem](linear-regression.md#frisch-waugh-lovell-theorem)
      - [Simple linear regression](linear-regression.md#simple-linear-regression)
        - [Centred simple linear regression](linear-regression.md#centred-simple-linear-regression)
      - [Residual sum of squares](linear-regression.md#residual-sum-of-squares)
      - [Ridge regression](linear-regression.md#ridge-regression)
        - [Gaussian posterior representation of ridge regression](linear-regression.md#gaussian-posterior-representation-of-ridge-regression)
        - [Unbounded directional risk of fixed ridge shrinkage](linear-regression.md#unbounded-directional-risk-of-fixed-ridge-shrinkage)
        - [Uniform directional risk improvement by ridge regression](linear-regression.md#uniform-directional-risk-improvement-by-ridge-regression)
        - [Unpenalized intercept in ridge regression](linear-regression.md#unpenalized-intercept-in-ridge-regression)
        - [Covariance and bias of a ridge regression estimator](linear-regression.md#covariance-and-bias-of-a-ridge-regression-estimator)
        - [Closed-form ridge regression estimator](linear-regression.md#closed-form-ridge-regression-estimator)
          - [Vanishing-penalty ridge limit](linear-regression.md#vanishing-penalty-ridge-limit)
          - [Primal-dual identity for ridge regression](linear-regression.md#primal-dual-identity-for-ridge-regression)
          - [Principal-component shrinkage by ridge regression](linear-regression.md#principal-component-shrinkage-by-ridge-regression)
      - [Fitted values](linear-regression.md#fitted-values)
        - [Linear smoother](linear-regression.md#linear-smoother)
          - [Effective degrees of freedom](linear-regression.md#effective-degrees-of-freedom)
      - [Design matrix](linear-regression.md#design-matrix)
        - [Confounding of nested fixed factors](linear-regression.md#confounding-of-nested-fixed-factors)
      - [Regression coefficient](linear-regression.md#regression-coefficient)
      - [Attenuation bias from classical measurement error](linear-regression.md#attenuation-bias-from-classical-measurement-error)
    - [R linear-model formula](statistical-modelling.md#r-linear-model-formula)
      - [Treatment coding](statistical-modelling.md#treatment-coding)
      - [Degrees of freedom of a factor predictor](statistical-modelling.md#degrees-of-freedom-of-a-factor-predictor)
    - [Hat matrix](statistical-modelling.md#hat-matrix)
      - [Fitted-residual orthogonality](statistical-modelling.md#fitted-residual-orthogonality)
    - [Normal linear-model confidence ellipsoid](statistical-modelling.md#normal-linear-model-confidence-ellipsoid)
      - [Cook's distance](statistical-modelling.md#cook-s-distance)
    - [Multicollinearity](statistical-modelling.md#multicollinearity)
      - [Variance inflation factor](statistical-modelling.md#variance-inflation-factor)
      - [Two-predictor variance inflation](statistical-modelling.md#two-predictor-variance-inflation)
    - [Ordinary least squares](statistical-modelling.md#ordinary-least-squares)
      - [Residual estimate of Gaussian noise variance](statistical-modelling.md#residual-estimate-of-gaussian-noise-variance)
        - [Residual standard error](statistical-modelling.md#residual-standard-error)
      - [Partial regression](statistical-modelling.md#partial-regression)
      - [Rank-deficient ordinary least squares](statistical-modelling.md#rank-deficient-ordinary-least-squares)
        - [Nonidentifiability prevents unbiased coefficient estimation](statistical-modelling.md#nonidentifiability-prevents-unbiased-coefficient-estimation)
      - [Linear regression through the origin](statistical-modelling.md#linear-regression-through-the-origin)
        - [Student t test for regression through the origin](statistical-modelling.md#student-t-test-for-regression-through-the-origin)
      - [Ordinary least squares estimators](statistical-modelling.md#ordinary-least-squares-estimators)
        - [Residual sum of squares in simple linear regression](statistical-modelling.md#residual-sum-of-squares-in-simple-linear-regression)
    - [Gauss-Markov theorem](statistical-modelling.md#gauss-markov-theorem)
    - [Weighted least squares](statistical-modelling.md#weighted-least-squares)
      - [Generalized least squares](statistical-modelling.md#generalized-least-squares)
        - [Whitening transformation](statistical-modelling.md#whitening-transformation)
    - [Normal equation](statistical-modelling.md#normal-equation)
    - [Consistency of least squares](statistical-modelling.md#consistency-of-least-squares)
    - [One-way normal linear model](statistical-modelling.md#one-way-normal-linear-model)
      - [Cell-means parametrization](statistical-modelling.md#cell-means-parametrization)
        - [Equal-cell replication variance formula](statistical-modelling.md#equal-cell-replication-variance-formula)
        - [Linear contrast of cell means](statistical-modelling.md#linear-contrast-of-cell-means)
          - [Treatment contrast](statistical-modelling.md#treatment-contrast)
            - [Orthogonal polynomial contrast](statistical-modelling.md#orthogonal-polynomial-contrast)
            - [Variance of a treatment contrast](statistical-modelling.md#variance-of-a-treatment-contrast)
            - [Interaction contrast](statistical-modelling.md#interaction-contrast)
              - [Logistic interaction as a ratio of odds ratios](statistical-modelling.md#logistic-interaction-as-a-ratio-of-odds-ratios)
      - [Full-dominance mean constraint](statistical-modelling.md#full-dominance-mean-constraint)
      - [Additive allele-count model](statistical-modelling.md#additive-allele-count-model)
  - [Regression leverage](statistical-modelling.md#regression-leverage)
  - [Risk ratio](statistical-modelling.md#risk-ratio)
    - [Relative risk from group compositions](statistical-modelling.md#relative-risk-from-group-compositions)
      - [Relative risk bounds from rounded group compositions](statistical-modelling.md#relative-risk-bounds-from-rounded-group-compositions)
    - [Log risk ratio](statistical-modelling.md#log-risk-ratio)
    - [Drug efficacy as a risk reduction](statistical-modelling.md#drug-efficacy-as-a-risk-reduction)
  - [Odds ratio](statistical-modelling.md#odds-ratio)
    - [Noncollapsibility of the odds ratio](statistical-modelling.md#noncollapsibility-of-the-odds-ratio)
    - [Log odds ratio](statistical-modelling.md#log-odds-ratio)
      - [Log odds ratio variance from a two-by-two table](statistical-modelling.md#log-odds-ratio-variance-from-a-two-by-two-table)
  - [Log-linear model](statistical-modelling.md#log-linear-model)
    - [Poisson surrogate for a conditional multinomial model](statistical-modelling.md#poisson-surrogate-for-a-conditional-multinomial-model)
    - [Stratified two-by-two conditional independence model](statistical-modelling.md#stratified-two-by-two-conditional-independence-model)
    - [Gaussian-prior Poisson log-effect conditional](statistical-modelling.md#gaussian-prior-poisson-log-effect-conditional)
    - [Independence log-linear model for a two-way contingency table](statistical-modelling.md#independence-log-linear-model-for-a-two-way-contingency-table)
    - [Saturated log-linear model](statistical-modelling.md#saturated-log-linear-model)
    - [Equal-efficacy Poisson log-linear model](statistical-modelling.md#equal-efficacy-poisson-log-linear-model)
  - [Maximum likelihood estimation](statistical-modelling.md#maximum-likelihood-estimation)
    - [Normal likelihood with variance equal to squared mean](statistical-modelling.md#normal-likelihood-with-variance-equal-to-squared-mean)
    - [Singular covariance and nonexistence of a Gaussian maximum likelihood estimate](statistical-modelling.md#singular-covariance-and-nonexistence-of-a-gaussian-maximum-likelihood-estimate)
    - [Compact-parameter consistency of maximum likelihood](statistical-modelling.md#compact-parameter-consistency-of-maximum-likelihood)
    - [Shifted exponential maximum likelihood](statistical-modelling.md#shifted-exponential-maximum-likelihood)
      - [Exact endpoint limit for a shifted exponential distribution](statistical-modelling.md#exact-endpoint-limit-for-a-shifted-exponential-distribution)
    - [Maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator)
      - [Likelihood supremum at an excluded boundary](statistical-modelling.md#likelihood-supremum-at-an-excluded-boundary)
      - [Uniform endpoint maximum-likelihood estimator](statistical-modelling.md#uniform-endpoint-maximum-likelihood-estimator)
      - [Neyman-Scott incidental parameter problem](statistical-modelling.md#neyman-scott-incidental-parameter-problem)
      - [Endpoint maximum likelihood for a singular location density](statistical-modelling.md#endpoint-maximum-likelihood-for-a-singular-location-density)
      - [Exponential-rate maximum-likelihood estimator](statistical-modelling.md#exponential-rate-maximum-likelihood-estimator)
      - [Maximum-likelihood fitted value](statistical-modelling.md#maximum-likelihood-fitted-value)
        - [Maximum-likelihood fitted probability](statistical-modelling.md#maximum-likelihood-fitted-probability)
      - [Normal mean and variance maximum-likelihood estimators](statistical-modelling.md#normal-mean-and-variance-maximum-likelihood-estimators)
      - [Invariance property of maximum likelihood estimation](statistical-modelling.md#invariance-property-of-maximum-likelihood-estimation)
      - [Likelihood function](statistical-modelling.md#likelihood-function)
        - [Marginal likelihood from a nuisance-free statistic](statistical-modelling.md#marginal-likelihood-from-a-nuisance-free-statistic)
        - [Conditional likelihood](statistical-modelling.md#conditional-likelihood)
          - [Saddlepoint conditional likelihood adjustment](statistical-modelling.md#saddlepoint-conditional-likelihood-adjustment)
        - [Observed-data likelihood](statistical-modelling.md#observed-data-likelihood)
        - [Bayesian deviance](statistical-modelling.md#bayesian-deviance)
        - [Conditional maximum likelihood](statistical-modelling.md#conditional-maximum-likelihood)
        - [Profile likelihood](statistical-modelling.md#profile-likelihood)
          - [Modified profile likelihood](statistical-modelling.md#modified-profile-likelihood)
            - [Modified profile likelihood for inverse Gaussian shape](statistical-modelling.md#modified-profile-likelihood-for-inverse-gaussian-shape)
            - [Modified profile likelihood for exponential regression](statistical-modelling.md#modified-profile-likelihood-for-exponential-regression)
          - [Gamma-ratio marginal and profile likelihood identity](statistical-modelling.md#gamma-ratio-marginal-and-profile-likelihood-identity)
          - [Profile log-likelihood](statistical-modelling.md#profile-log-likelihood)
      - [Log-likelihood](statistical-modelling.md#log-likelihood)
      - [Binomial proportion maximum-likelihood estimator](statistical-modelling.md#binomial-proportion-maximum-likelihood-estimator)
      - [Exponential distribution rate estimator](statistical-modelling.md#exponential-distribution-rate-estimator)
      - [Asymptotic normality of a maximum likelihood estimator](statistical-modelling.md#asymptotic-normality-of-a-maximum-likelihood-estimator)
  - [Logistic distribution](statistical-modelling.md#logistic-distribution)
  - [Gaussian conditional expectation](statistical-modelling.md#gaussian-conditional-expectation)
  - [Linear discriminant analysis](statistical-modelling.md#linear-discriminant-analysis)
    - [Canonical discriminant directions](statistical-modelling.md#canonical-discriminant-directions)
    - [Kernel linear discriminant analysis](statistical-modelling.md#kernel-linear-discriminant-analysis)
  - [Quadratic discriminant analysis](statistical-modelling.md#quadratic-discriminant-analysis)
  - [Bootstrapping (statistics)](statistical-modelling.md#bootstrapping-statistics)
    - [Bootstrap failure for a uniform endpoint](statistical-modelling.md#bootstrap-failure-for-a-uniform-endpoint)
    - [Bootstrap standard error](statistical-modelling.md#bootstrap-standard-error)
    - [Bootstrap confidence interval](statistical-modelling.md#bootstrap-confidence-interval)
      - [Bootstrap inference for a product of regression coefficients](statistical-modelling.md#bootstrap-inference-for-a-product-of-regression-coefficients)
      - [Bootstrap-t confidence interval](statistical-modelling.md#bootstrap-t-confidence-interval)
      - [Percentile bootstrap confidence interval](statistical-modelling.md#percentile-bootstrap-confidence-interval)
      - [Basic bootstrap confidence interval](statistical-modelling.md#basic-bootstrap-confidence-interval)
    - [Bootstrap consistency theorem for the sample mean](statistical-modelling.md#bootstrap-consistency-theorem-for-the-sample-mean)
    - [Bootstrap sample](statistical-modelling.md#bootstrap-sample)
      - [Wild bootstrap](statistical-modelling.md#wild-bootstrap)
      - [Paired bootstrap](statistical-modelling.md#paired-bootstrap)
      - [Conditional bootstrap variance of a sample mean](statistical-modelling.md#conditional-bootstrap-variance-of-a-sample-mean)
      - [Bootstrap count vectors](statistical-modelling.md#bootstrap-count-vectors)
    - [Parametric bootstrap](statistical-modelling.md#parametric-bootstrap)
  - [Risk function](statistical-modelling.md#risk-function)
    - [Mean squared error](statistical-modelling.md#mean-squared-error)
      - [Asymptotic mean squared error](statistical-modelling.md#asymptotic-mean-squared-error)
      - [Shrinking a sample mean with variance proportional to mean squared](statistical-modelling.md#shrinking-a-sample-mean-with-variance-proportional-to-mean-squared)
      - [Integrated mean squared error](statistical-modelling.md#integrated-mean-squared-error)
        - [Asymptotic mean integrated squared error](statistical-modelling.md#asymptotic-mean-integrated-squared-error)
      - [Bias-variance decomposition of mean squared error](statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error)
      - [Affine shrinkage estimator for a binomial proportion](statistical-modelling.md#affine-shrinkage-estimator-for-a-binomial-proportion)
    - [Admissible decision rule](statistical-modelling.md#admissible-decision-rule)
      - [Admissible estimator](statistical-modelling.md#admissible-estimator)
        - [James–Stein estimator](statistical-modelling.md#james-stein-estimator)
          - [James–Stein shrinkage toward the sample mean](statistical-modelling.md#james-stein-shrinkage-toward-the-sample-mean)
          - [Identical worst-case risk under strict James-Stein domination](statistical-modelling.md#identical-worst-case-risk-under-strict-james-stein-domination)
    - [Minimax estimator](statistical-modelling.md#minimax-estimator)
      - [Constant-risk binomial proportion estimator](statistical-modelling.md#constant-risk-binomial-proportion-estimator)
      - [Minimax risk](statistical-modelling.md#minimax-risk)
        - [Pointwise versus uniform risk distinction](statistical-modelling.md#pointwise-versus-uniform-risk-distinction)
      - [Minimaxity of the usual multivariate normal mean estimator](statistical-modelling.md#minimaxity-of-the-usual-multivariate-normal-mean-estimator)
  - [Cramér-Rao bound](statistical-modelling.md#cramer-rao-bound)
    - [Efficient estimator](statistical-modelling.md#efficient-estimator)
    - [Van Trees inequality](statistical-modelling.md#van-trees-inequality)
  - [Informant function](statistical-modelling.md#informant-function)
    - [Gaussian regression score](statistical-modelling.md#gaussian-regression-score)
    - [Score equation](statistical-modelling.md#score-equation)
    - [Mean-zero score identity](statistical-modelling.md#mean-zero-score-identity)
    - [Fisher information matrix](statistical-modelling.md#fisher-information-matrix)
      - [Orthogonal statistical parameters](statistical-modelling.md#orthogonal-statistical-parameters)
        - [Score factorization implies parameter orthogonality](statistical-modelling.md#score-factorization-implies-parameter-orthogonality)
        - [Orthogonal coefficient blocks in a centered normal linear model](statistical-modelling.md#orthogonal-coefficient-blocks-in-a-centered-normal-linear-model)
        - [Cox-Reid adjusted profile likelihood](statistical-modelling.md#cox-reid-adjusted-profile-likelihood)
        - [Local orthogonal nuisance reparametrization](statistical-modelling.md#local-orthogonal-nuisance-reparametrization)
        - [Negative binomial mean-size parameter orthogonality](statistical-modelling.md#negative-binomial-mean-size-parameter-orthogonality)
        - [Interest-respecting reparametrization](statistical-modelling.md#interest-respecting-reparametrization)
          - [Orthogonalization equation for two statistical parameters](statistical-modelling.md#orthogonalization-equation-for-two-statistical-parameters)
      - [Jeffreys prior](statistical-modelling.md#jeffreys-prior)
        - [Proper gamma approximation to a Poisson Jeffreys prior](statistical-modelling.md#proper-gamma-approximation-to-a-poisson-jeffreys-prior)
        - [Jeffreys prior for a scale parameter](statistical-modelling.md#jeffreys-prior-for-a-scale-parameter)
        - [Jeffreys prior for an additive variance component](statistical-modelling.md#jeffreys-prior-for-an-additive-variance-component)
      - [Fisher information of a multivariate normal location model](statistical-modelling.md#fisher-information-of-a-multivariate-normal-location-model)
      - [Empirical score outer-product information](statistical-modelling.md#empirical-score-outer-product-information)
      - [Observed Fisher information](statistical-modelling.md#observed-fisher-information)
      - [Tensorization of Fisher information](statistical-modelling.md#tensorization-of-fisher-information)
      - [Fisher information in a stationary Gaussian autoregressive location model](statistical-modelling.md#fisher-information-in-a-stationary-gaussian-autoregressive-location-model)
      - [Scoring algorithm](statistical-modelling.md#scoring-algorithm)
        - [Binomial-proportion Fisher scoring](statistical-modelling.md#binomial-proportion-fisher-scoring)
      - [Information identity](statistical-modelling.md#information-identity)
      - [Normal location-scale score](statistical-modelling.md#normal-location-scale-score)
      - [Local asymptotic normality](statistical-modelling.md#local-asymptotic-normality)
        - [Contiguity under locally asymptotically normal alternatives](statistical-modelling.md#contiguity-under-locally-asymptotically-normal-alternatives)
        - [Gaussian shift model](statistical-modelling.md#gaussian-shift-model)
  - [Statistical hypothesis test](statistical-modelling.md#statistical-hypothesis-test)
    - [Statistical hypothesis](statistical-modelling.md#statistical-hypothesis)
    - [Sequential probability ratio test](statistical-modelling.md#sequential-probability-ratio-test)
    - [Statistical significance](statistical-modelling.md#statistical-significance)
    - [Two-sided hypothesis test](statistical-modelling.md#two-sided-hypothesis-test)
    - [One-sided hypothesis test](statistical-modelling.md#one-sided-hypothesis-test)
    - [Alternative hypothesis](statistical-modelling.md#alternative-hypothesis)
    - [Hotelling's T-squared statistic](statistical-modelling.md#hotelling-s-t-squared-statistic)
      - [Affine invariance of Hotelling's statistic](statistical-modelling.md#affine-invariance-of-hotelling-s-statistic)
      - [Hotelling test of linear hypotheses](statistical-modelling.md#hotelling-test-of-linear-hypotheses)
        - [Second-difference test of a linear mean profile](statistical-modelling.md#second-difference-test-of-a-linear-mean-profile)
    - [Rejection region](statistical-modelling.md#rejection-region)
    - [McNemar's test](statistical-modelling.md#mcnemar-s-test)
      - [Equality criterion for paired and unpaired allele tests](statistical-modelling.md#equality-criterion-for-paired-and-unpaired-allele-tests)
      - [Paired binary sample size calculation](statistical-modelling.md#paired-binary-sample-size-calculation)
    - [Significant and nonsignificant results need not differ significantly](statistical-modelling.md#significant-and-nonsignificant-results-need-not-differ-significantly)
    - [Monte Carlo test](statistical-modelling.md#monte-carlo-test)
    - [Predictive discrepancy statistic](statistical-modelling.md#predictive-discrepancy-statistic)
    - [Scan statistic](statistical-modelling.md#scan-statistic)
      - [Cyclic interval overlap bound](statistical-modelling.md#cyclic-interval-overlap-bound)
      - [Quadratic scan statistic](statistical-modelling.md#quadratic-scan-statistic)
    - [Least-favourable null configuration](statistical-modelling.md#least-favourable-null-configuration)
    - [Pearson chi-squared test of homogeneity](statistical-modelling.md#pearson-chi-squared-test-of-homogeneity)
      - [Empty groups in a binomial homogeneity test](statistical-modelling.md#empty-groups-in-a-binomial-homogeneity-test)
      - [Pearson chi-squared statistic for contingency tables](statistical-modelling.md#pearson-chi-squared-statistic-for-contingency-tables)
        - [Yates's correction for continuity](statistical-modelling.md#yates-s-correction-for-continuity)
    - [Statistical test](statistical-modelling.md#statistical-test)
      - [Most powerful test](statistical-modelling.md#most-powerful-test)
    - [Test statistic](statistical-modelling.md#test-statistic)
    - [Student's t-test](statistical-modelling.md#student-s-t-test)
      - [Exact pooled two-sample t statistic](statistical-modelling.md#exact-pooled-two-sample-t-statistic)
      - [Normal-mean likelihood ratio with unknown variance](statistical-modelling.md#normal-mean-likelihood-ratio-with-unknown-variance)
      - [Regression coefficient test power ignores nuisance coefficients](statistical-modelling.md#regression-coefficient-test-power-ignores-nuisance-coefficients)
    - [Fixed alternative](statistical-modelling.md#fixed-alternative)
    - [Local alternative](statistical-modelling.md#local-alternative)
    - [Randomization test](statistical-modelling.md#randomization-test)
      - [Conditional randomization test](statistical-modelling.md#conditional-randomization-test)
      - [Permutation test](statistical-modelling.md#permutation-test)
      - [Sign-flip randomization test](statistical-modelling.md#sign-flip-randomization-test)
    - [Null hypothesis](statistical-modelling.md#null-hypothesis)
    - [Simple hypothesis](statistical-modelling.md#simple-hypothesis)
    - [Size of a statistical test](statistical-modelling.md#size-of-a-statistical-test)
    - [Significance level](statistical-modelling.md#significance-level)
    - [P-value](statistical-modelling.md#p-value)
      - [Super-uniform random variable](statistical-modelling.md#super-uniform-random-variable)
    - [Fisher's exact test](statistical-modelling.md#fisher-s-exact-test)
      - [Exact power of Fisher's exact test](statistical-modelling.md#exact-power-of-fisher-s-exact-test)
    - [Maximin test](statistical-modelling.md#maximin-test)
    - [Multiple hypothesis testing](statistical-modelling.md#multiple-hypothesis-testing)
      - [Intersection hypothesis](statistical-modelling.md#intersection-hypothesis)
        - [Closure of a family of statistical hypotheses](statistical-modelling.md#closure-of-a-family-of-statistical-hypotheses)
      - [Hochberg procedure](statistical-modelling.md#hochberg-procedure)
      - [Simes inequality](statistical-modelling.md#simes-inequality)
        - [Simes test](statistical-modelling.md#simes-test)
      - [Weighted interval testing for a piecewise-constant mean](statistical-modelling.md#weighted-interval-testing-for-a-piecewise-constant-mean)
      - [Intersection-union test](statistical-modelling.md#intersection-union-test)
      - [Bonferroni correction](statistical-modelling.md#bonferroni-correction)
        - [Weighted Bonferroni correction](statistical-modelling.md#weighted-bonferroni-correction)
          - [Weighted Holm step-down procedure](statistical-modelling.md#weighted-holm-step-down-procedure)
        - [Holm–Bonferroni method](statistical-modelling.md#holm-bonferroni-method)
          - [First true null argument for Holm control](statistical-modelling.md#first-true-null-argument-for-holm-control)
      - [Benjamini-Hochberg procedure](statistical-modelling.md#benjamini-hochberg-procedure)
        - [Benjamini-Hochberg leave-one-out identity](statistical-modelling.md#benjamini-hochberg-leave-one-out-identity)
          - [Benjamini-Hochberg leave-two-out identity](statistical-modelling.md#benjamini-hochberg-leave-two-out-identity)
            - [Second moment of the Benjamini-Hochberg false discovery proportion](statistical-modelling.md#second-moment-of-the-benjamini-hochberg-false-discovery-proportion)
          - [Exact false discovery rate under independent null p-values](statistical-modelling.md#exact-false-discovery-rate-under-independent-null-p-values)
      - [False discovery rate](statistical-modelling.md#false-discovery-rate)
        - [False discovery proportion](statistical-modelling.md#false-discovery-proportion)
      - [Familywise error rate](statistical-modelling.md#familywise-error-rate)
        - [Familywise error control for a laminar hypothesis family](statistical-modelling.md#familywise-error-control-for-a-laminar-hypothesis-family)
      - [Closed testing procedure](statistical-modelling.md#closed-testing-procedure)
        - [Closed-testing control of the familywise error rate](statistical-modelling.md#closed-testing-control-of-the-familywise-error-rate)
    - [Joint hypothesis test](statistical-modelling.md#joint-hypothesis-test)
    - [Power function of a statistical test](statistical-modelling.md#power-function-of-a-statistical-test)
    - [Uniformly most powerful test](statistical-modelling.md#uniformly-most-powerful-test)
      - [Crossing-power obstruction to a uniformly most powerful test](statistical-modelling.md#crossing-power-obstruction-to-a-uniformly-most-powerful-test)
    - [Pearson's chi-squared test](statistical-modelling.md#pearson-s-chi-squared-test)
      - [Pearson chi-squared goodness-of-fit test](statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test)
        - [Binomial goodness-of-fit with an estimated parameter](statistical-modelling.md#binomial-goodness-of-fit-with-an-estimated-parameter)
        - [Pearson chi-squared test of independence](statistical-modelling.md#pearson-chi-squared-test-of-independence)
    - [Likelihood-ratio test of independence in a contingency table](statistical-modelling.md#likelihood-ratio-test-of-independence-in-a-contingency-table)
      - [Aggregation can change a contingency-table independence test](statistical-modelling.md#aggregation-can-change-a-contingency-table-independence-test)
    - [Linear-by-linear association test](statistical-modelling.md#linear-by-linear-association-test)
    - [Wald test](statistical-modelling.md#wald-test)
      - [Signed normal Wald statistic](statistical-modelling.md#signed-normal-wald-statistic)
      - [Wald statistics with a shared control](statistical-modelling.md#wald-statistics-with-a-shared-control)
      - [Multivariate Wald statistic](statistical-modelling.md#multivariate-wald-statistic)
        - [Wald statistic for linear restrictions](statistical-modelling.md#wald-statistic-for-linear-restrictions)
      - [Wald and likelihood-ratio asymptotic equivalence](statistical-modelling.md#wald-and-likelihood-ratio-asymptotic-equivalence)
      - [Two-sided Gaussian p-value](statistical-modelling.md#two-sided-gaussian-p-value)
    - [Likelihood-ratio test](statistical-modelling.md#likelihood-ratio-test)
      - [Gaussian covariance diagonality likelihood-ratio test](statistical-modelling.md#gaussian-covariance-diagonality-likelihood-ratio-test)
      - [Gaussian diagonal-covariance likelihood-ratio test](statistical-modelling.md#gaussian-diagonal-covariance-likelihood-ratio-test)
      - [One-sided likelihood-ratio test for two normal variances](statistical-modelling.md#one-sided-likelihood-ratio-test-for-two-normal-variances)
      - [Boundary likelihood-ratio test for two Gaussian means](statistical-modelling.md#boundary-likelihood-ratio-test-for-two-gaussian-means)
      - [Single-parameter boundary likelihood-ratio test](statistical-modelling.md#single-parameter-boundary-likelihood-ratio-test)
      - [Variance-component likelihood-ratio test at a boundary](statistical-modelling.md#variance-component-likelihood-ratio-test-at-a-boundary)
        - [Location-scale invariant simulation test for a Gaussian variance component](statistical-modelling.md#location-scale-invariant-simulation-test-for-a-gaussian-variance-component)
      - [Likelihood ratio](statistical-modelling.md#likelihood-ratio)
        - [Log-likelihood ratio](statistical-modelling.md#log-likelihood-ratio)
      - [Likelihood-ratio test statistic](statistical-modelling.md#likelihood-ratio-test-statistic)
        - [Bartlett correction](statistical-modelling.md#bartlett-correction)
          - [Bartlett-corrected likelihood-ratio statistic](statistical-modelling.md#bartlett-corrected-likelihood-ratio-statistic)
          - [Bartlett correction coefficient](statistical-modelling.md#bartlett-correction-coefficient)
            - [Bartlett correction for a normal variance with unknown mean](statistical-modelling.md#bartlett-correction-for-a-normal-variance-with-unknown-mean)
      - [Generalized likelihood-ratio test](statistical-modelling.md#generalized-likelihood-ratio-test)
        - [Likelihood-ratio test of area-proportional Poisson means](statistical-modelling.md#likelihood-ratio-test-of-area-proportional-poisson-means)
        - [Analysis of deviance for nested generalized linear models](statistical-modelling.md#analysis-of-deviance-for-nested-generalized-linear-models)
          - [Residual deviance](statistical-modelling.md#residual-deviance)
            - [Null deviance](statistical-modelling.md#null-deviance)
        - [Likelihood-ratio test for equality of two normal means](statistical-modelling.md#likelihood-ratio-test-for-equality-of-two-normal-means)
        - [Nested likelihood-ratio rejection regions](statistical-modelling.md#nested-likelihood-ratio-rejection-regions)
    - [Score test](statistical-modelling.md#score-test)
      - [Restricted maximum-likelihood estimator](statistical-modelling.md#restricted-maximum-likelihood-estimator)
      - [Score test under a simple null](statistical-modelling.md#score-test-under-a-simple-null)
        - [Quadratic form of a standard normal vector](statistical-modelling.md#quadratic-form-of-a-standard-normal-vector)
      - [Residual sum of squares in a normal sample](statistical-modelling.md#residual-sum-of-squares-in-a-normal-sample)
        - [Chi-square central limit theorem](statistical-modelling.md#chi-square-central-limit-theorem)
    - [Neyman-Pearson lemma](statistical-modelling.md#neyman-pearson-lemma)
      - [Most powerful test for a Laplace location shift](statistical-modelling.md#most-powerful-test-for-a-laplace-location-shift)
      - [Minimum sum of errors in a simple hypothesis test](statistical-modelling.md#minimum-sum-of-errors-in-a-simple-hypothesis-test)
      - [Exponential-rate likelihood-ratio test](statistical-modelling.md#exponential-rate-likelihood-ratio-test)
      - [Uniformly most powerful test for an exponential rate](statistical-modelling.md#uniformly-most-powerful-test-for-an-exponential-rate)
      - [Monotone likelihood ratio](statistical-modelling.md#monotone-likelihood-ratio)
        - [Posterior odds are monotone under a monotone likelihood ratio](statistical-modelling.md#posterior-odds-are-monotone-under-a-monotone-likelihood-ratio)
        - [Monotone test](statistical-modelling.md#monotone-test)
        - [Karlin-Rubin theorem](statistical-modelling.md#karlin-rubin-theorem)
          - [Uniformly most powerful upper-tail test for a logistic location](statistical-modelling.md#uniformly-most-powerful-upper-tail-test-for-a-logistic-location)
  - [Grouped exponential observation](statistical-modelling.md#grouped-exponential-observation)
    - [Asymptotic information loss from grouping](statistical-modelling.md#asymptotic-information-loss-from-grouping)

## Spatial Bernoulli infection model

↑ **Parent:** [Statistical model](statistical-model.md)

Given the currently infected set $I_t$ and susceptible set $S_t$, define $A_{it}(\eta)=\sum_{j\in I_t}K_\eta(d_{ij})$ and $P_{it}=1-e^{-\alpha A_{it}}$. Conditionally [independent](random-variable.md#independent-random-variables) new-infection indicators $Y_{it}$ have [likelihood](statistical-modelling.md#likelihood-function)

$$
L(\alpha,\eta)=\prod_t\prod_{i\in S_t}(1-e^{-\alpha A_{it}(\eta)})^{Y_{it}}e^{-\alpha A_{it}(\eta)(1-Y_{it})}.
$$

A nonnegative infection intensity requires $\alpha\geq0$; an unrestricted [normal distribution](probability-theory.md#normal-distribution) [prior distribution](statistical-inference.md#prior-probability) for $\alpha$ must therefore be restricted or replaced. With $K_\beta(d)=d^{-\beta}$ or $K_\gamma(d)=e^{-\gamma d}$ and positive distances, the conditional [posterior](statistical-inference.md#bayesian-posterior) kernels are not generally conjugate normal [probability densities](quantum-mechanics.md#probability-density). [Metropolis–Hastings algorithm](statistical-inference.md#metropolis-hastings-algorithm) updates, optionally on $\log\alpha$ with its [Jacobian determinant](calculus.md#jacobian-determinant), provide a direct sampling method.

## Transformation model

↑ **Parent:** [Statistical model](statistical-model.md)

A [group action](group-theory.md#group-action) on the sample space induces a compatible action on the parameter space, preserving the family of [probability laws](probability-theory.md#probability-distribution). In a transitive model every law arises by transforming a fixed reference law. A [location-scale model](#location-scale-family) is generated by $y\mapsto a+by$, $b>0$, with parameter action $(\mu,\sigma)\mapsto(a+b\mu,b\sigma)$.

### Equivariant estimator

↑ **Parent:** [Transformation model](#transformation-model)

An estimator respects the [group action](group-theory.md#group-action) if the displayed identity holds. If it takes values in the transformation [group](group.md) itself, normalization $T(y)^{-1}y$ is a [maximal invariant](#maximal-invariant): equivariance proves invariance, and equality of normalized samples reconstructs the transformation between them. For estimates in a homogeneous parameter space with a nontrivial stabilizer, normalization is defined only modulo that stabilizer; quotienting the remaining action is essential.

### Maximal invariant

↑ **Parent:** [Transformation model](#transformation-model)

A statistic is invariant if $A(gy)=A(y)$; it is maximal when it also separates different [group orbits](group-theory.md#orbit-of-a-group-action). Consequently every invariant procedure factors through the [maximal invariant](#maximal-invariant), subject to the usual measurability conditions on the orbit space. Standardizing a sample by an [equivariant estimator](#equivariant-estimator) of location and positive scale gives a [maximal invariant](#maximal-invariant) for the positive affine [group](group.md).

#### Ranks as a maximal invariant under increasing transformations

↑ **Parent:** [Maximal invariant](#maximal-invariant)

On samples of distinct real observations, the labeled rank vector is a [maximal invariant](#maximal-invariant) for simultaneous strictly increasing bijections of the real line. Such transformations preserve every comparison. Conversely two samples with the same ranks can be matched by a piecewise linear increasing bijection through their corresponding ordered observations, with positive-slope tails. Under a common continuous [probability distribution](probability-theory.md#probability-distribution), every labeled ordering is equally likely by [exchangeability](probability-theory.md#exchangeable-random-variables), giving distribution-free [rank tests](nonparametric-statistics.md#rank-test). This argument does not assume that all continuous distributions lie in one orbit of real-line homeomorphisms.

#### Invariant tests factor through a maximal invariant

↑ **Parent:** [Maximal invariant](#maximal-invariant)

If $T$ is a [maximal invariant](#maximal-invariant) for a [group action](group-theory.md#group-action), an invariant test function is constant on each [group orbit](group-theory.md#orbit-of-a-group-action) and therefore equals $b\circ T$ for a function $b$ on the orbit space. Conversely every such function is invariant. Appropriate quotient measurability is understood. If the action is transitive on a null family of [probability distributions](probability-theory.md#probability-distribution), invariance also gives the same null law of $T$ under every member. Thus tests based on $T$ eliminate that null nuisance variation.

## Parametric statistical model

↑ **Parent:** [Statistical model](statistical-model.md)

A [statistical model](statistical-model.md) indexed by a parameter vector of fixed finite dimension is parametric. Examples include a [normal distribution](probability-theory.md#normal-distribution) with unknown mean and variance and a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with unknown mean. Its [likelihood function](statistical-modelling.md#likelihood-function) is the joint sample density or mass function, regarded as a function of the parameter at the observed sample.

## Location-scale family

↑ **Parent:** [Statistical model](statistical-model.md)

In a location-scale family, $Y=\mu+\sigma Z$ for a fixed base [probability distribution](probability-theory.md#probability-distribution) of $Z$, with $\mu\in\mathbb R$ and $\sigma>0$. Location translates observations, and scale multiplies their deviations. For an independent sample with a base density and at least two observations, the normalized residual vector $(Y_i-\bar Y)/s$, where $s^2=n^{-1}\sum_i(Y_i-\bar Y)^2$, is an [ancillary statistic](probability-and-statistics.md#ancillary-statistic). Indeed, $\bar Y=\mu+\sigma\bar Z$ and $s=\sigma s_Z$, making the residual vector a function of the base sample alone. This algebraic result needs no population moments.

### Log-transformed location-scale model

↑ **Parent:** [Location-scale family](#location-scale-family)

If $W$ has [probability density function](continuous-probability-distribution.md#probability-density-function) $f(w;q)$ and [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $F_W(w;q)$, then $T=\exp(\alpha+\sigma W)$, $\sigma>0$, has density $f((\log t-\alpha)/\sigma;q)/(\sigma t)$ and distribution function $F_W((\log t-\alpha)/\sigma;q)$ for $t>0$. The factor $1/(\sigma t)$ follows from the [change-of-variables formula for a probability density](continuous-probability-distribution.md#change-of-variables-formula-for-a-probability-density). Upper truncation at $M$ divides the density by $F_W((\log M-\alpha)/\sigma;q)$.

### Conditional inference in a location-scale family

↑ **Parent:** [Location-scale family](#location-scale-family)

For normalized residuals $A_i=(Y_i-\bar Y)/s$, [Fisherian conditional inference](statistical-inference.md#fisherian-conditional-inference) uses the [conditional distribution](probability-theory.md#conditional-distribution) of $(\bar Y,s)$ given the observed $A=a$. For almost every attainable ancillary value, the joint conditional density of $\bar Y=m$ and $s=t>0$ is proportional to

$$
t^{n-2}\sigma^{-n}\prod_{i=1}^nf_0\!\left(\frac{m+ta_i-\mu}{\sigma}\right).
$$

The factor $t^{n-2}$ is the radial Jacobian on the $(n-1)$-dimensional centered residual space. After setting $u=(m-\mu)/\sigma$ and $v=t/\sigma$, the conditional density is proportional to $v^{n-2}\prod_i f_0(u+va_i)$, which is parameter-free. Conditioning on a continuous ancillary uses a [regular conditional distribution](probability-theory.md#regular-conditional-distribution), rather than division by the probability of a singleton ancillary value.

## Regression model

↑ **Parent:** [Statistical model](statistical-model.md)

A regression model specifies features of the [conditional distribution](probability-theory.md#conditional-distribution) of a response given predictor [covariates](#covariate), often a conditional mean or a full parametric density. [Linear regression](linear-regression.md) specifies a linear conditional mean; [logistic regression](statistical-modelling.md#logistic-regression) specifies a logit-linear conditional probability for a binary response. The conditional comparison represented by a coefficient depends on which covariates are included.

### Interaction (statistics)

↑ **Parent:** [Regression model](#regression-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interaction_(statistics))

A statistical interaction means that the effect of one predictor depends on another on the chosen response scale. In a [linear regression](linear-regression.md), an [interaction term](#interaction-term) $\beta_3XZ$ changes the slope in $X$ to $\beta_1+\beta_3Z$. Whether interaction is present depends on the comparison scale; additive effects and multiplicative effects use different null contrasts. Comparing subgroup effects requires an [interaction contrast](statistical-modelling.md#interaction-contrast), rather than contrasting their separate significance labels.

#### Interaction plot

↑ **Parent:** [Interaction (statistics)](#interaction-statistics)

An interaction plot displays response means against levels of one factor, with separate lines for levels of another and optional panels for further factors. In an additive [linear regression](linear-regression.md), the difference between two lines is constant across the horizontal factor, so the population-mean lines are parallel. Changing line separations or crossings show a [statistical interaction](#interaction-statistics) on that response scale. Sample means may be nonparallel through noise, so the plot describes the effect pattern rather than replacing a formal [hypothesis test](statistical-modelling.md#statistical-hypothesis-test).

#### Interaction term

↑ **Parent:** [Interaction (statistics)](#interaction-statistics)

An interaction term lets the effect of one predictor depend on another. In

$$
\mathbb E[Y\mid X,Z]
=\beta_0+\beta_1X+\beta_2Z+\beta_3XZ,
$$

the slope with respect to $X$ is $\beta_1+\beta_3Z$.

##### Two-factor interaction

↑ **Parent:** [Interaction term](#interaction-term)

A two-factor interaction means that changing one factor has a different effect at different levels of another. For a two-level [factorial design](statistical-modelling.md#factorial-design), its sign column is $x_ix_j$, and four times its coefficient is the corresponding difference of differences. It can be confounded with other [factorial contrasts](statistical-modelling.md#factorial-contrast) in a [fractional factorial design](statistical-modelling.md#fractional-factorial-design).

##### Coupling constant (physics)

↑ **Parent:** [Interaction term](#interaction-term)

A coefficient multiplying an interaction term controls its strength relative to the chosen field normalization. Its [engineering dimension](critical-phenomenon.md#engineering-dimension) determines whether it is dimensionless, relevant or irrelevant. A renormalized [coupling constant](#coupling-constant-physics) constant is specified at a [renormalization scale](perturbative-quantum-field-theory.md#renormalization-scale); its change with that scale is described by the [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics).

##### Principle of marginality

↑ **Parent:** [Interaction term](#interaction-term)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principle_of_marginality)

A hierarchical [statistical model](statistical-model.md) that contains an [interaction term](#interaction-term) retains its associated lower-order effects. For two [categorical predictors](statistical-modelling.md#regression-factor) this means keeping both main effects when keeping their interaction. A nonsignificant averaged main effect may coexist with large opposite effects in different groups. Dropping its lower-order term while retaining the interaction can make the model depend on arbitrary factor coding.

## Statistical path

↑ **Parent:** [Statistical model](statistical-model.md)

A statistical path is a one-dimensional family of [probability measures](probability-theory.md#probability-measure) inside a [statistical model](statistical-model.md), passing through a specified baseline $P$. A [differentiability in quadratic mean](#differentiability-in-quadratic-mean) condition gives its [score function](statistical-modelling.md#informant-function), the first-order direction of the family in square-root-density coordinates. The path must respect all restrictions of the [statistical model](statistical-model.md), including normalization and any fixed [moments](probability-theory.md#moment).

### Statistical tangent set

↑ **Parent:** [Statistical path](#statistical-path)

A statistical tangent set is the collection of [score functions](statistical-modelling.md#informant-function) attained by a specified family of [differentiable-in-quadratic-mean paths](#differentiability-in-quadratic-mean) through $P$. The choice of paths is part of the definition. Its elements lie in the [mean-zero L2 space](measure-theory.md#mean-zero-l2-space), but the set need not already be a closed [vector subspace](vector-space.md#vector-subspace).

#### Bounded density tilt

↑ **Parent:** [Statistical tangent set](#statistical-tangent-set)

For bounded measurable $g$ with $Pg=0$, the formula $p_t=p(1+tg)$ defines a normalized positive [probability density function](continuous-probability-distribution.md#probability-density-function) for $|t|\|g\|_\infty<1$. A uniform [Taylor expansion](calculus.md#taylor-expansion) of the square root proves [differentiability in quadratic mean](#differentiability-in-quadratic-mean) with [score function](statistical-modelling.md#informant-function) $g$: the squared remainder is $O(t^4Pg^4)$. Such paths realize all bounded centered directions of an unrestricted density model.

##### Density of bounded centered scores

↑ **Parent:** [Bounded density tilt](#bounded-density-tilt)

For $h\in L^2_0(P)$, truncate $h$ to $h_m=\max(-m,\min(h,m))$ and subtract $Ph_m$. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) gives $h_m\to h$ in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $Ph_m\to0$. Thus bounded centered directions are dense in the [mean-zero L2 space](measure-theory.md#mean-zero-l2-space). The measure defining the [L2 norm](real-analysis.md#l2-norm) is essential: density-weighted [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) can contain [functions](function.md) outside the unweighted Lebesgue space.

#### Statistical tangent space

↑ **Parent:** [Statistical tangent set](#statistical-tangent-set)

The statistical tangent space is the closed linear span in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) of a [statistical tangent set](#statistical-tangent-set). Taking this closure makes [orthogonal projection](hilbert-space.md#orthogonal-projection) available and ensures that a continuous [derivative](calculus.md#derivative) specified on attainable [score functions](statistical-modelling.md#informant-function) extends to the whole space.

### Differentiability in quadratic mean

↑ **Parent:** [Statistical path](#statistical-path)

A dominated [statistical path](#statistical-path) is differentiable in quadratic mean at $P$ if its square-root [probability density function](continuous-probability-distribution.md#probability-density-function) has an [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) [derivative](calculus.md#derivative) $(1/2)g\sqrt p$, with $g\in L^2(P)$. The [score function](statistical-modelling.md#informant-function) is $g$. This formulation controls mass near zeros of $p$ as well as the [derivative](calculus.md#derivative) on the support of $P$; a pointwise log-density [derivative](calculus.md#derivative) is insufficient by itself.

#### Quadratic-mean to L1 density derivative

↑ **Parent:** [Differentiability in quadratic mean](#differentiability-in-quadratic-mean)

Let $\delta_t=\sqrt{p_t}-\sqrt p=(t/2)g\sqrt p+r_t$, with $\|r_t\|_2=o(|t|)$. Since $p_t-p=2\sqrt p\,\delta_t+\delta_t^2$, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|p_t-p-tpg\|_1\leq2\|r_t\|_2+\|\delta_t\|_2^2=o(|t|)$. Thus [differentiability in quadratic mean](#differentiability-in-quadratic-mean) suffices to differentiate bounded density [integrals](calculus.md#integral), even when the density itself has no useful pointwise [derivative](calculus.md#derivative).

#### Mean-zero score identity under quadratic-mean differentiability

↑ **Parent:** [Differentiability in quadratic mean](#differentiability-in-quadratic-mean)

For a [differentiable-in-quadratic-mean path](#differentiability-in-quadratic-mean), normalization gives $\langle(\sqrt{p_t}-\sqrt p)/t,\sqrt{p_t}+\sqrt p\rangle=0$. The two factors converge in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) to $g\sqrt p/2$ and $2\sqrt p$. Continuity of the [inner product](linear-algebra.md#inner-product) therefore gives $Pg=0$. This proves [score function](statistical-modelling.md#informant-function) centering without differentiating the density [integral](calculus.md#integral).

## Scale family

↑ **Parent:** [Statistical model](statistical-model.md)

A scale family rescales a fixed distribution by a positive parameter. The standardized variable $Y/\sigma$ has density $f$, independent of $\sigma$. This simplifies moments, simulations and the [Jeffreys prior for a scale parameter](statistical-modelling.md#jeffreys-prior-for-a-scale-parameter).

## Statistical parameter

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_parameter)

A [statistical parameter](#statistical-parameter) indexes a family of [probability distributions](probability-theory.md#probability-distribution) in a [statistical model](statistical-model.md). It is fixed in a frequentist sampling model; a [prior distribution](statistical-inference.md#prior-probability) makes it random for [Bayesian statistics](statistical-inference.md#bayesian-statistics). Different [statistical parameter](#statistical-parameter) values should produce different observable distributions when [identifiability](#identifiability) is claimed.

### Nuisance parameter

↑ **Parent:** [Statistical parameter](#statistical-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nuisance_parameter)

A [nuisance parameter](#nuisance-parameter) is a [statistical parameter](#statistical-parameter) required to specify the distribution of observations but not itself the target of inference. A [profile likelihood](statistical-modelling.md#profile-likelihood) maximizes over it; [Bayesian model evidence](statistical-inference.md#bayesian-model-evidence) integrates over it using a proper [prior distribution](statistical-inference.md#prior-probability). These operations differ and need not give the same inference. A [baseline hazard](survival-analysis.md#baseline-hazard) in a [Cox proportional-hazards model](survival-analysis.md#cox-proportional-hazards-model) is an infinite-dimensional example.

#### Mixed log-likelihood derivative obstruction to parameter separation

↑ **Parent:** [Nuisance parameter](#nuisance-parameter)

On a common positive support, a factorization $f=\phi_0(x)\phi_C(x;\psi)\phi_S(x;\lambda)$ implies $\partial_\psi\partial_\lambda\log f=0$. Thus any nonzero mixed derivative prevents this exact separation. For $n$ independent [gamma distributed](continuous-probability-distribution.md#gamma-distribution) observations with shape $a$ and rate $b$, this mixed derivative is $n/b$, so exact separation of shape and rate into such factors is impossible.

## Covariate

↑ **Parent:** [Statistical model](statistical-model.md)

A covariate is an observed explanatory variable used to model the [conditional distribution](probability-theory.md#conditional-distribution) of a response. A vector of covariates can enter a [linear predictor](statistical-modelling.md#linear-predictor), a treatment-effect adjustment or a [hazard multiplier](survival-analysis.md#hazard-multiplier). Conditioning on a covariate does not itself establish that its effect is causal.

### Baseline covariate

↑ **Parent:** [Covariate](#covariate)

A baseline covariate is measured before treatment assignment or exposure. A prognostic baseline covariate predicts the outcome. Adjusting for such variables in a [randomized controlled trial](causal-inference.md#randomized-controlled-trial) can improve [statistical efficiency](statistical-inference.md#efficiency-statistics) without conditioning on a treatment consequence. For example, if $Y=\tau Z+\gamma X+\varepsilon$ with randomized $Z$ independent of $X$, adjustment for $X$ reduces the unexplained [variance](variance.md) from $\gamma^2\operatorname{Var}(X)+\operatorname{Var}(\varepsilon)$ to $\operatorname{Var}(\varepsilon)$. This precision role of prognostic baseline adjustment is described in [the FDA statistical guidance on covariate adjustment](https://www.fda.gov/media/148910/download).

## Homoscedasticity

↑ **Parent:** [Statistical model](statistical-model.md)

Constancy of the error [variance](variance.md) across observations or conditional covariate values. In [fixed-design nonparametric regression](nonparametric-statistics.md#fixed-design-nonparametric-regression), $Y_i=m(x_i)+\sigma\epsilon_i$ with $\operatorname{Var}(\epsilon_i)=1$ has $\operatorname{Var}(Y_i)=\sigma^2$ for every design point.

## Identifiability

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Identifiability)

A statistical model is identifiable when distinct parameter values determine distinct probability distributions. In a nonidentifiable parameterization, data can at most estimate combinations of parameters that remain unchanged along each equivalent parameter set.

### Moment aliasing in a shared zero-inflated count model

↑ **Parent:** [Identifiability](#identifiability)

In a [shared zero-inflated Gamma-Poisson count model](statistical-modelling.md#shared-zero-inflated-gamma-poisson-count-model), write $m_j=(1-\pi)\mu_j$ and $\kappa=(\tau+\pi)/(1-\pi)$. Its first two moments are $\operatorname{Var}(Y_j)=m_j+\kappa m_j^2$ and $\operatorname{Cov}(Y_j,Y_k)=\kappa m_jm_k$. These moments do not separately identify $\pi$, $\tau$, and the component-mean intercept: taking $\pi'=0$, $\tau'=\kappa$ and $\mu'_j=m_j$ gives the same first two moments. The full count distribution can carry information absent from the moments. A [consistent estimator](statistical-inference.md#consistency-statistics) of a marginal mean ratio therefore need not consistently estimate a structural-zero fraction from a misspecified moment parameterization.

### Corner-point constraint

↑ **Parent:** [Identifiability](#identifiability)

In a [normal linear model](statistical-modelling.md#normal-linear-model) with an intercept and factor effects, set the effect of one factor level to zero. The intercept then denotes that reference level's mean, and the remaining effects are contrasts to it. The constraint removes redundant [statistical parameters](#statistical-parameter) without altering the fitted mean space.

## Location family

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Location_family)

A location family has distribution functions $F_\theta(x)=F_0(x-\theta)$, so changing the parameter translates the distribution without changing its shape.

### Location score

↑ **Parent:** [Location family](#location-family)

The location score is the [score function](statistical-modelling.md#informant-function) for translating a [probability density function](continuous-probability-distribution.md#probability-density-function) $f$. The minus sign comes from differentiating $f(y-\theta)$ in $\theta$. Under regular tail conditions, [integration by parts](calculus.md#integration-by-parts) gives $E_f\rho=0$ and $E_f(\varepsilon\rho)=1$. These identities determine projections of the [score function](statistical-modelling.md#informant-function) onto the span of the centered error.

### Single-observation location minimax bound

↑ **Parent:** [Location family](#location-family)

For a known mean-zero noise law with finite [variance](variance.md) $\sigma^2$, observing only $Y=a+\epsilon$ with unrestricted $a\in\mathbb R$ has [minimax risk](statistical-modelling.md#minimax-risk) $\sigma^2$ under [squared-error loss](statistical-inference.md#squared-error-loss). The observation itself attains this risk. For the lower bound, use a flat [prior distribution](statistical-inference.md#prior-probability) on $[-A,A]$ and condition an easier experiment on $|\epsilon|\leq M$. Away from the prior endpoints, the [Bayesian posterior](statistical-inference.md#bayesian-posterior) noise has its original truncated law. Let $A\to\infty$ and then $M\to\infty$ in the resulting [Bayes risk](statistical-inference.md#bayes-risk) lower bound. No [normal distribution](probability-theory.md#normal-distribution) or density for the noise is required.

## Probabilistic graphical model

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_graphical_model)

A probabilistic graphical model represents factorization and conditional-independence structure using a graph whose vertices are random variables.

### Junction tree

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)

A junction tree connects the [maximal cliques](graph-theory.md#maximal-clique) of a [chordal graph](graph-theory.md#chordal-graph) into a [tree](combinatorics.md#tree-graph-theory) satisfying the [running intersection property](#running-intersection-property). Its edges carry separators equal to the intersections of the endpoint cliques. Assigning original factors to containing cliques permits exact [sum-product belief propagation](#sum-product-belief-propagation) without summing independently over the entire collection of variables.

#### Junction tree algorithm

↑ **Parent:** [Junction tree](#junction-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Junction_tree_algorithm)

The junction tree algorithm performs exact inference in a finite [probabilistic graphical model](#probabilistic-graphical-model). First moralize a [Bayesian network](#bayesian-network) if necessary; then apply [triangulation of an undirected graph](graph-theory.md#triangulation-of-an-undirected-graph), organize its [maximal cliques](graph-theory.md#maximal-clique) into a [junction tree](#junction-tree), and assign each original factor to one containing clique. Inward and outward [junction-tree sum-product messages](#junction-tree-sum-product-message) compute the [normalizing constant](continuous-probability-distribution.md#normalizing-constant) and [marginal distributions](probability-theory.md#marginal-distribution). Its cost depends exponentially on the largest clique's number of variables, rather than necessarily on the total number of variables.

#### Junction-tree sum-product message

↑ **Parent:** [Junction tree](#junction-tree)

Assign each factor exactly once to a containing [clique](graph-theory.md#clique-graph-theory) and multiply the factors there into $\psi_i$. The displayed [sum-product belief propagation](#sum-product-belief-propagation) message sums out variables of $C_i$ outside the separator $S_{ij}=C_i\cap C_j$. By the [running intersection property](#running-intersection-property), eliminating all variables in the subtree on the $i$ side creates precisely this function of the separator. An inward pass computes the [normalizing constant](continuous-probability-distribution.md#normalizing-constant) at the root; an outward pass produces [marginal distributions](probability-theory.md#marginal-distribution). For [pedigree likelihoods](biology.md#pedigree-likelihood), observed genotypes and [penetrance](biology.md#penetrance) factors simply multiply the relevant potentials.

#### Running intersection property

↑ **Parent:** [Junction tree](#junction-tree)

The running intersection property says that every variable belongs to a connected subtree of a [junction tree](#junction-tree). Equivalently, every clique along the path between two cliques contains their intersection. This ensures that eliminating variables on one side of a tree edge leaves a message depending only on its separator with the other side.

### Bayesian network

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayesian_network)

A Bayesian network consists of a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) $G$ whose nodes are [random variables](random-variable.md), together with [conditional distributions](probability-theory.md#conditional-distribution) satisfying $p(x)=\prod_jp(x_j\mid x_{\operatorname{pa}_G(j)})$. Its [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) encodes [conditional independence](random-variable.md#conditional-independence) constraints. For unrestricted binary variables it has $\sum_j2^{|\operatorname{pa}_G(j)|}$ free [conditional probabilities](probability-theory.md#conditional-probability). A [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) used this way need not have a causal interpretation.

#### Bayesian network structure score

↑ **Parent:** [Bayesian network](#bayesian-network)

For observations $\mathcal D$ and graph $G$, [Bayes' theorem](probability-theory.md#bayes-theorem) gives $p(G\mid\mathcal D)\propto\pi(G)\int p(\mathcal D\mid\theta_G,G)\pi(\theta_G\mid G)\,d\theta_G$. Here $\pi(G)$ is the graph [prior distribution](statistical-inference.md#prior-probability) and $\theta_G$ the local distribution [statistical parameters](#statistical-parameter). The integral is [Bayesian model evidence](statistical-inference.md#bayesian-model-evidence); it averages over [nuisance parameters](#nuisance-parameter) with a proper [statistical parameter](#statistical-parameter) [prior distribution](statistical-inference.md#prior-probability). For [independent](random-variable.md#independent-random-variables) complete observations, the node-factorized [likelihood function](statistical-modelling.md#likelihood-function) and [independence](random-variable.md#independent-random-variables) of local [statistical parameter](#statistical-parameter) [prior distributions](statistical-inference.md#prior-probability) make the evidence factor over nodes; suitable [conjugate priors](exponential-family.md#conjugate-prior) can make the local integrals analytic. With missing node observations, integrating out unobserved values can couple the local parameters, so [independence](random-variable.md#independent-random-variables) of local [prior distributions](statistical-inference.md#prior-probability) alone does not guarantee this factorization. Proper priors and coherent hyperparameters matter for comparing different graphs.

#### Gaussian Bayesian network

↑ **Parent:** [Bayesian network](#bayesian-network)

A Gaussian Bayesian network specifies a linear normal conditional model at each node of a [Bayesian network](#bayesian-network): $X_j\mid X_{\operatorname{pa}(j)}\sim N(\alpha_j+\gamma_j^TX_{\operatorname{pa}(j)},\sigma_j^2)$. [Independent](random-variable.md#independent-random-variables) local errors and an acyclic ordering generate a joint [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution). Positive conditional [variances](variance.md) give a nonsingular joint [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution). The graph constrains [regression coefficients](linear-regression.md#regression-coefficient) and hence [conditional independence](random-variable.md#conditional-independence).

### Belief propagation

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Belief_propagation)

Belief propagation passes local messages between factors or neighboring variables to compute marginal distributions or maximizing assignments. On a tree, two directed messages per edge give exact results in time linear in the number of vertices when state spaces are fixed.

#### Sum-product belief propagation

↑ **Parent:** [Belief propagation](#belief-propagation)

The sum-product form of [belief propagation](#belief-propagation) sums over eliminated states in each message. On a tree it computes exact normalization constants and marginal distributions.

#### Max-product belief propagation

↑ **Parent:** [Belief propagation](#belief-propagation)

The max-product form of [belief propagation](#belief-propagation) replaces summation by maximization. On a tree, storing maximizing states while passing messages and then backtracking gives an exact [maximum a posteriori estimate](statistical-inference.md#maximum-a-posteriori-estimate).

### Markov blanket

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Markov_blanket)

A Markov blanket of a variable is a set that makes it conditionally independent of every remaining variable. In a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph), the parents, children, and other parents of the children form the standard Markov blanket.

#### Minimal Markov blanket under faithfulness

↑ **Parent:** [Markov blanket](#markov-blanket)

Under [faithfulness of a directed acyclic graph](causal-inference.md#faithfulness-of-a-directed-acyclic-graph), every conditioning set screening a vertex from all remaining vertices contains its graphical [Markov blanket](#markov-blanket). A missing adjacent vertex leaves a one-edge active path; a missing other parent of a child leaves the active path $k\to h\leftarrow u$, since the child $h$ is necessarily conditioned. Thus the graphical blanket is the unique smallest screening set.

#### Markov blanket D-separation

↑ **Parent:** [Markov blanket](#markov-blanket)

In a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph), let $B$ contain the parents, children, and other parents of children of vertex $k$. Then $k$ is [D-separated](combinatorics.md#d-separation) from all remaining vertices by $B$. Every path out of $k$ meets a conditioned noncollider either at a parent, at a child, or at another parent just after a conditioned child-collider. The [global Markov property for a directed acyclic graph](causal-inference.md#global-markov-property-for-a-directed-acyclic-graph) gives $Z_k\perp Z_{(B\cup\{k\})^c}\mid Z_B$.

### Markov random field

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Markov_random_field)

A Markov random field is an undirected graphical model whose graph encodes conditional independence by vertex separation.

#### Autologistic binary-image model

↑ **Parent:** [Markov random field](#markov-random-field)

On a graph, a binary configuration has probability proportional to $\exp(\alpha\sum_v x_v+\beta\sum_{\{v,w\}}x_vx_w)$, with each edge counted once. The full [conditional probability](probability-theory.md#conditional-probability) of a one is logistic with [linear predictor](statistical-modelling.md#linear-predictor) $\alpha+\beta\sum_{w\sim v}x_w$. Local neighbor sums eliminate the need to evaluate the [normalizing constant](continuous-probability-distribution.md#normalizing-constant).

##### Gaussian-noise posterior for an autologistic image

↑ **Parent:** [Autologistic binary-image model](#autologistic-binary-image-model)

Independent unit-variance Gaussian observations with mean $x_v$ add $y_v-1/2$ to the local binary field. The [posterior distribution](statistical-inference.md#bayesian-posterior) [conditional probability](probability-theory.md#conditional-probability) is $\operatorname{logistic}(\alpha+\beta z_v+y_v-1/2)$. The neighbor interaction is unchanged, so checkerboard conditional independence and the same Gibbs schemes remain valid.

#### Clique potential

↑ **Parent:** [Markov random field](#markov-random-field)

A clique potential is a nonnegative function of the variables belonging to one clique. Products of clique potentials define the unnormalized density of a Markov random field.

#### Global Markov property for an undirected graph

↑ **Parent:** [Markov random field](#markov-random-field)

The global Markov property says that graph separation of vertex sets $A$ and $B$ by $S$ implies conditional independence of the corresponding random vectors given the variables at $S$.

## Statistical modelling

↑ **Parent:** [Statistical model](statistical-model.md)

[This section is present in another page, follow this link to view it.](statistical-modelling.md)

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (19)

- [Ancillary statistic](probability-and-statistics.md#ancillary-statistic)
- [Optimal experimental design](statistical-modelling.md#optimal-experimental-design)
- [Parametric statistical model](#parametric-statistical-model)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#5/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#3/b/iii/solution)
- [Principle of marginality](#principle-of-marginality)
- [Regression factor](statistical-modelling.md#regression-factor)
- [Score factorization implies parameter orthogonality](statistical-modelling.md#score-factorization-implies-parameter-orthogonality)
- [Statistical functional](statistical-inference.md#statistical-functional)
- [Statistical modelling](statistical-modelling.md)
- [Statistical parameter](#statistical-parameter)
- [Statistical path](#statistical-path)
- [Statistical sample](statistical-inference.md#statistical-sample)
