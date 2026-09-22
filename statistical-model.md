# Statistical model

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_model)

A statistical model is a family of probability distributions proposed for the process that generated observed data.

**Table of contents**

- [Parameter space](#parameter-space)
- [Parameter recovery](#parameter-recovery)
- [Mixed model](#mixed-model)
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
    - [Simple-effects analysis](#simple-effects-analysis)
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
  - [Normality assumption](statistical-modelling.md#normality-assumption)
  - [Data centering](statistical-modelling.md#data-centering)
  - [Regression analysis](statistical-modelling.md#regression-analysis)
    - [Statistical mediation](statistical-modelling.md#statistical-mediation)
  - [Mark and recapture](statistical-modelling.md#mark-and-recapture)
    - [Capture-recapture model](statistical-modelling.md#capture-recapture-model)
      - [Closed-population capture-recapture model](statistical-modelling.md#closed-population-capture-recapture-model)
      - [Missing-count EM for capture-recapture](statistical-modelling.md#missing-count-em-for-capture-recapture)
  - [Nonlinear regression](statistical-modelling.md#nonlinear-regression)
  - [Outlier](statistical-modelling.md#outlier)
  - [Regression to the mean](statistical-modelling.md#regression-to-the-mean)
  - [Response variable](statistical-modelling.md#response-variable)
  - [Scientific control](statistical-modelling.md#scientific-control)
  - [Design of experiments](design-of-experiments.md)
    - [Crossed disconnection experiment](design-of-experiments.md#crossed-disconnection-experiment)
    - [Demand characteristic](design-of-experiments.md#demand-characteristic)
    - [Dismantling study](design-of-experiments.md#dismantling-study)
    - [Waiting-list control](design-of-experiments.md#waiting-list-control)
    - [Manipulation check](design-of-experiments.md#manipulation-check)
    - [Yoked control](design-of-experiments.md#yoked-control)
    - [Active control](design-of-experiments.md#active-control)
      - [Befriending intervention](design-of-experiments.md#befriending-intervention)
    - [Pilot study](design-of-experiments.md#pilot-study)
    - [Randomized experiment](design-of-experiments.md#randomized-experiment)
    - [Between-subject design](design-of-experiments.md#between-subject-design)
    - [Within-subject design](design-of-experiments.md#within-subject-design)
    - [Independent variable](design-of-experiments.md#independent-variable)
    - [Positive control](design-of-experiments.md#positive-control)
    - [Negative control](design-of-experiments.md#negative-control)
      - [Vehicle control](design-of-experiments.md#vehicle-control)
    - [Pair feeding](design-of-experiments.md#pair-feeding)
    - [Blinding](design-of-experiments.md#blinding)
    - [Sham treatment](design-of-experiments.md#sham-treatment)
    - [Construct validity](design-of-experiments.md#construct-validity)
      - [Predictive validity](design-of-experiments.md#predictive-validity)
      - [Task impurity](design-of-experiments.md#task-impurity)
      - [Criterion validity](design-of-experiments.md#criterion-validity)
      - [Discriminant validity](design-of-experiments.md#discriminant-validity)
      - [Convergent validity](design-of-experiments.md#convergent-validity)
      - [Content validity](design-of-experiments.md#content-validity)
    - [Ecological validity](design-of-experiments.md#ecological-validity)
    - [Before-after control-impact design](design-of-experiments.md#before-after-control-impact-design)
    - [Batch effect](design-of-experiments.md#batch-effect)
    - [Cross-fostering](design-of-experiments.md#cross-fostering)
    - [Optimal experimental design](design-of-experiments.md#optimal-experimental-design)
      - [General equivalence theorem for optimal design](design-of-experiments.md#general-equivalence-theorem-for-optimal-design)
      - [G-optimal design](design-of-experiments.md#g-optimal-design)
      - [D-optimal design](design-of-experiments.md#d-optimal-design)
      - [Approximate experimental design](design-of-experiments.md#approximate-experimental-design)
    - [Latin square](design-of-experiments.md#latin-square)
      - [Latin square enumeration](design-of-experiments.md#latin-square-enumeration)
      - [Analysis of variance for a Latin square](design-of-experiments.md#analysis-of-variance-for-a-latin-square)
      - [Mutually orthogonal Latin squares](design-of-experiments.md#mutually-orthogonal-latin-squares)
    - [Contrast (statistics)](design-of-experiments.md#contrast-statistics)
    - [Response surface methodology](design-of-experiments.md#response-surface-methodology)
      - [Center-point curvature contrast](design-of-experiments.md#center-point-curvature-contrast)
      - [Steepest ascent in response surface methodology](design-of-experiments.md#steepest-ascent-in-response-surface-methodology)
      - [Coded experimental variable](design-of-experiments.md#coded-experimental-variable)
      - [Rotatable design](design-of-experiments.md#rotatable-design)
      - [Central composite design](design-of-experiments.md#central-composite-design)
    - [Split-plot design](design-of-experiments.md#split-plot-design)
    - [Factorial design](design-of-experiments.md#factorial-design)
      - [Main effect](design-of-experiments.md#main-effect)
      - [Factorial contrast](design-of-experiments.md#factorial-contrast)
      - [Fractional factorial design](design-of-experiments.md#fractional-factorial-design)
    - [Crossover design](design-of-experiments.md#crossover-design)
      - [Carryover effect](design-of-experiments.md#carryover-effect)
    - [Completely randomized design](design-of-experiments.md#completely-randomized-design)
    - [Blocks in experimental design](design-of-experiments.md#blocks-in-experimental-design)
      - [Estimability from within-block differences](design-of-experiments.md#estimability-from-within-block-differences)
      - [Block confounding in a factorial design](design-of-experiments.md#block-confounding-in-a-factorial-design)
      - [Block design](design-of-experiments.md#block-design)
    - [Replication in experimental design](design-of-experiments.md#replication-in-experimental-design)
      - [Replicate](design-of-experiments.md#replicate)
      - [Nested measurements](design-of-experiments.md#nested-measurements)
      - [Biological replicate](design-of-experiments.md#biological-replicate)
      - [Technical replicate](design-of-experiments.md#technical-replicate)
    - [Experimental unit](design-of-experiments.md#experimental-unit)
      - [Observational unit](design-of-experiments.md#observational-unit)
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
  - [Fixed effect](statistical-modelling.md#fixed-effect)
  - [Geostatistics](statistical-modelling.md#geostatistics)
    - [Kriging](statistical-modelling.md#kriging)
      - [Universal kriging](statistical-modelling.md#universal-kriging)
      - [Ordinary kriging](statistical-modelling.md#ordinary-kriging)
      - [Simple kriging](statistical-modelling.md#simple-kriging)
    - [Covariogram](statistical-modelling.md#covariogram)
    - [Intrinsically stationary random field](statistical-modelling.md#intrinsically-stationary-random-field)
      - [Semivariogram](statistical-modelling.md#semivariogram)
  - [Saturated statistical model](statistical-modelling.md#saturated-statistical-model)
    - [Bernoulli saturated log-likelihood](statistical-modelling.md#bernoulli-saturated-log-likelihood)
  - [Hurdle model](statistical-modelling.md#hurdle-model)
  - [Zero inflation](statistical-modelling.md#zero-inflation)
    - [Count-mixture structural zero](statistical-modelling.md#count-mixture-structural-zero)
    - [Zero-inflated negative binomial model](statistical-modelling.md#zero-inflated-negative-binomial-model)
      - [Shared zero-inflated Gamma-Poisson count model](statistical-modelling.md#shared-zero-inflated-gamma-poisson-count-model)
      - [EM for zero-inflated negative binomial regression](statistical-modelling.md#em-for-zero-inflated-negative-binomial-regression)
  - [Estimator](statistical-modelling.md#estimator)
    - [Method of moments (statistics)](statistical-modelling.md#method-of-moments-statistics)
    - [U-statistic](statistical-modelling.md#u-statistic)
      - [Influence function of a U-statistic](statistical-modelling.md#influence-function-of-a-u-statistic)
      - [Kernel of a U-statistic](statistical-modelling.md#kernel-of-a-u-statistic)
      - [Variance as a U-statistic](statistical-modelling.md#variance-as-a-u-statistic)
      - [Symmetrization of a U-statistic kernel](statistical-modelling.md#symmetrization-of-a-u-statistic-kernel)
      - [U-statistic central limit theorem](statistical-modelling.md#u-statistic-central-limit-theorem)
  - [Categorical variable](statistical-modelling.md#categorical-variable)
    - [Binary categorical variable](statistical-modelling.md#binary-categorical-variable)
    - [Nominal categorical variable](statistical-modelling.md#nominal-categorical-variable)
    - [Regression factor](statistical-modelling.md#regression-factor)
    - [Ordinal categorical variable](statistical-modelling.md#ordinal-categorical-variable)
      - [Sign reversal under reversal of one ordinal ordering](statistical-modelling.md#sign-reversal-under-reversal-of-one-ordinal-ordering)
      - [Stuart's tau-c](statistical-modelling.md#stuart-s-tau-c)
      - [Kendall rank correlation coefficient](statistical-modelling.md#kendall-rank-correlation-coefficient)
      - [Unordered-pair partition for ordinal data](statistical-modelling.md#unordered-pair-partition-for-ordinal-data)
      - [Tied pair (ordinal data)](statistical-modelling.md#tied-pair-ordinal-data)
      - [Somers' D](statistical-modelling.md#somers-d)
      - [Goodman and Kruskal's gamma](statistical-modelling.md#goodman-and-kruskal-s-gamma)
      - [Concordant pair](statistical-modelling.md#concordant-pair)
      - [Discordant pair](statistical-modelling.md#discordant-pair)
    - [Indicator variable](statistical-modelling.md#indicator-variable)
  - [Latent variable](latent-variable.md)
    - [Latent growth model](latent-variable.md#latent-growth-model)
      - [Growth mixture model](latent-variable.md#growth-mixture-model)
    - [Unobserved heterogeneity](latent-variable.md#unobserved-heterogeneity)
    - [Factor analysis](latent-variable.md#factor-analysis)
      - [Gaussian-process factor analysis](latent-variable.md#gaussian-process-factor-analysis)
      - [Method factor](latent-variable.md#method-factor)
      - [Confirmatory factor analysis](latent-variable.md#confirmatory-factor-analysis)
      - [Exploratory factor analysis](latent-variable.md#exploratory-factor-analysis)
      - [Latent factor](latent-variable.md#latent-factor)
      - [Orthogonal factor model](latent-variable.md#orthogonal-factor-model)
      - [EM update for a single-factor Gaussian model](latent-variable.md#em-update-for-a-single-factor-gaussian-model)
    - [Random effect](latent-variable.md#random-effect)
      - [Poisson-lognormal random-effect model](latent-variable.md#poisson-lognormal-random-effect-model)
      - [Crossed random effects](latent-variable.md#crossed-random-effects)
      - [Random slope](latent-variable.md#random-slope)
    - [Expectation-maximization algorithm](latent-variable.md#expectation-maximization-algorithm)
      - [EM expectation step](latent-variable.md#em-expectation-step)
      - [EM maximization step](latent-variable.md#em-maximization-step)
      - [Known-variance Gaussian mixture EM example](latent-variable.md#known-variance-gaussian-mixture-em-example)
      - [Ordered-rate exponential M-step](latent-variable.md#ordered-rate-exponential-m-step)
      - [EM for merged multinomial cells](latent-variable.md#em-for-merged-multinomial-cells)
      - [EM for an independent missing normal coordinate](latent-variable.md#em-for-an-independent-missing-normal-coordinate)
      - [EM transition-count update on a tree](latent-variable.md#em-transition-count-update-on-a-tree)
      - [EM for a missing observation in a Gaussian AR1 process](latent-variable.md#em-for-a-missing-observation-in-a-gaussian-ar1-process)
      - [EM likelihood monotonicity](latent-variable.md#em-likelihood-monotonicity)
  - [Functional data analysis](statistical-modelling.md#functional-data-analysis)
    - [Functional time warping](statistical-modelling.md#functional-time-warping)
      - [Square-root velocity function](statistical-modelling.md#square-root-velocity-function)
    - [Functional principal component analysis](statistical-modelling.md#functional-principal-component-analysis)
      - [Principal component function](statistical-modelling.md#principal-component-function)
      - [Functional principal component score](statistical-modelling.md#functional-principal-component-score)
      - [Karhunen–Loève expansion](statistical-modelling.md#karhunen-loeve-expansion)
    - [Functional mean test](statistical-modelling.md#functional-mean-test)
      - [FPCA mean test](statistical-modelling.md#fpca-mean-test)
    - [Covariance-operator distance](statistical-modelling.md#covariance-operator-distance)
      - [Hilbert-Schmidt distance between covariance operators](statistical-modelling.md#hilbert-schmidt-distance-between-covariance-operators)
      - [Square-root distance between covariance operators](statistical-modelling.md#square-root-distance-between-covariance-operators)
      - [Procrustes distance between covariance operators](statistical-modelling.md#procrustes-distance-between-covariance-operators)
    - [Functional linear model](statistical-modelling.md#functional-linear-model)
      - [Scalar-on-function linear model](statistical-modelling.md#scalar-on-function-linear-model)
      - [Function-on-function linear model](statistical-modelling.md#function-on-function-linear-model)
  - [Goodness of fit](statistical-modelling.md#goodness-of-fit)
    - [Reduced chi-squared](statistical-modelling.md#reduced-chi-squared)
    - [Goodness-of-fit test](statistical-modelling.md#goodness-of-fit-test)
  - [Contingency table](statistical-modelling.md#contingency-table)
    - [Contingency coefficient](statistical-modelling.md#contingency-coefficient)
    - [Generalized phi coefficient](statistical-modelling.md#generalized-phi-coefficient)
    - [Goodman and Kruskal's lambda](statistical-modelling.md#goodman-and-kruskal-s-lambda)
    - [Cramér's V](statistical-modelling.md#cramer-s-v)
    - [Two-by-two contingency table](statistical-modelling.md#two-by-two-contingency-table)
  - [Mixture model](statistical-modelling.md#mixture-model)
    - [Threshold inference for a mixture proportion](statistical-modelling.md#threshold-inference-for-a-mixture-proportion)
    - [Gaussian scale mixture](statistical-modelling.md#gaussian-scale-mixture)
      - [Rayleigh-normal scale mixture](statistical-modelling.md#rayleigh-normal-scale-mixture)
    - [Finite mixture model](statistical-modelling.md#finite-mixture-model)
      - [Mixture component](statistical-modelling.md#mixture-component)
      - [Mixture allocation indicator](statistical-modelling.md#mixture-allocation-indicator)
      - [Two-Gaussian mixture example](statistical-modelling.md#two-gaussian-mixture-example)
      - [Observed and latent mixture labels](statistical-modelling.md#observed-and-latent-mixture-labels)
      - [Mixture identifiability](statistical-modelling.md#mixture-identifiability)
      - [Label switching](statistical-modelling.md#label-switching)
      - [Gaussian mixture Gibbs updates with independent priors](statistical-modelling.md#gaussian-mixture-gibbs-updates-with-independent-priors)
      - [Mixture responsibility](statistical-modelling.md#mixture-responsibility)
      - [Finite Gaussian mixture with a common variance](statistical-modelling.md#finite-gaussian-mixture-with-a-common-variance)
      - [Mixture weight](statistical-modelling.md#mixture-weight)
    - [Dirichlet process mixture model](statistical-modelling.md#dirichlet-process-mixture-model)
  - [Latent-variable model](statistical-modelling.md#latent-variable-model)
  - [Statistical learning](statistical-learning.md)
    - [Dimensionality reduction](statistical-learning.md#dimensionality-reduction)
    - [Stochastic approximation](statistical-learning.md#stochastic-approximation)
      - [Stochastic-approximation step-size conditions](statistical-learning.md#stochastic-approximation-step-size-conditions)
    - [Self-supervised learning](statistical-learning.md#self-supervised-learning)
      - [Contrastive representation learning](statistical-learning.md#contrastive-representation-learning)
    - [Noise ceiling](statistical-learning.md#noise-ceiling)
    - [Stability-plasticity dilemma](statistical-learning.md#stability-plasticity-dilemma)
    - [Catastrophic interference](statistical-learning.md#catastrophic-interference)
    - [Inductive bias](statistical-learning.md#inductive-bias)
    - [Reinforcement learning](statistical-learning.md#reinforcement-learning)
      - [Distributional reinforcement learning](statistical-learning.md#distributional-reinforcement-learning)
      - [Experience replay](statistical-learning.md#experience-replay)
      - [Model-based reinforcement learning](statistical-learning.md#model-based-reinforcement-learning)
      - [Model-free reinforcement learning](statistical-learning.md#model-free-reinforcement-learning)
      - [Temporal-difference learning](statistical-learning.md#temporal-difference-learning)
      - [Actor-critic architecture](statistical-learning.md#actor-critic-architecture)
    - [Multivariate pattern analysis](statistical-learning.md#multivariate-pattern-analysis)
      - [Cross-modal decoding](statistical-learning.md#cross-modal-decoding)
      - [Representational similarity analysis](statistical-learning.md#representational-similarity-analysis)
    - [Online learning](statistical-learning.md#online-learning)
      - [Optimism in the face of uncertainty](statistical-learning.md#optimism-in-the-face-of-uncertainty)
      - [Multi-armed bandit](statistical-learning.md#multi-armed-bandit)
    - [Feature interaction](statistical-learning.md#feature-interaction)
    - [Multilabel classification](statistical-learning.md#multilabel-classification)
    - [Multiclass classification](statistical-learning.md#multiclass-classification)
    - [One-hot encoding](statistical-learning.md#one-hot-encoding)
    - [scGen](statistical-learning.md#scgen)
    - [Supervised learning](statistical-learning.md#supervised-learning)
      - [Error-correction learning](statistical-learning.md#error-correction-learning)
    - [Generalization in statistical learning](statistical-learning.md#generalization-in-statistical-learning)
      - [Compositional generalization](statistical-learning.md#compositional-generalization)
    - [Unsupervised learning](statistical-learning.md#unsupervised-learning)
      - [Continuous transformation learning](statistical-learning.md#continuous-transformation-learning)
      - [Competitive learning](statistical-learning.md#competitive-learning)
      - [Multidimensional scaling](statistical-learning.md#multidimensional-scaling)
      - [Sparse coding](statistical-learning.md#sparse-coding)
      - [Hebbian learning](statistical-learning.md#hebbian-learning)
    - [Cluster analysis](statistical-learning.md#cluster-analysis)
      - [Cluster in cluster analysis](statistical-learning.md#cluster-in-cluster-analysis)
      - [K-means clustering](statistical-learning.md#k-means-clustering)
      - [Jaccard index](statistical-learning.md#jaccard-index)
      - [Dissimilarity matrix](statistical-learning.md#dissimilarity-matrix)
      - [Simple matching coefficient](statistical-learning.md#simple-matching-coefficient)
      - [Agglomerative hierarchical clustering](statistical-learning.md#agglomerative-hierarchical-clustering)
    - [Validation set](statistical-learning.md#validation-set)
      - [Test set](statistical-learning.md#test-set)
    - [Prediction error](statistical-learning.md#prediction-error)
      - [Test error](statistical-learning.md#test-error)
      - [Mean squared prediction error](statistical-learning.md#mean-squared-prediction-error)
    - [Training error](statistical-learning.md#training-error)
      - [Prediction optimism](statistical-learning.md#prediction-optimism)
    - [Data leakage](statistical-learning.md#data-leakage)
    - [Dataset shift](statistical-learning.md#dataset-shift)
    - [Regression function](statistical-learning.md#regression-function)
    - [Principal component analysis](statistical-learning.md#principal-component-analysis)
      - [High explained variance need not preserve class information under PCA](statistical-learning.md#high-explained-variance-need-not-preserve-class-information-under-pca)
      - [Principal component regression](statistical-learning.md#principal-component-regression)
      - [Scree plot](statistical-learning.md#scree-plot)
      - [Principal component loading](statistical-learning.md#principal-component-loading)
      - [Principal component](statistical-learning.md#principal-component)
      - [Explained variance of a principal component](statistical-learning.md#explained-variance-of-a-principal-component)
      - [Principal component analysis on a correlation matrix](statistical-learning.md#principal-component-analysis-on-a-correlation-matrix)
      - [Population principal component](statistical-learning.md#population-principal-component)
      - [Sample principal component](statistical-learning.md#sample-principal-component)
    - [Classification in statistical learning](statistical-learning.md#classification-in-statistical-learning)
      - [Classification accuracy](statistical-learning.md#classification-accuracy)
      - [Misclassification rate](statistical-learning.md#misclassification-rate)
      - [Classification tree](statistical-learning.md#classification-tree)
      - [Binary classification](statistical-learning.md#binary-classification)
      - [Decision boundary](statistical-learning.md#decision-boundary)
      - [Majority vote](statistical-learning.md#majority-vote)
      - [Confusion matrix](statistical-learning.md#confusion-matrix)
      - [Classification and regression tree](statistical-learning.md#classification-and-regression-tree)
      - [Conditional class probability](statistical-learning.md#conditional-class-probability)
      - [Risk consistency](statistical-learning.md#risk-consistency)
      - [K-nearest neighbors algorithm](statistical-learning.md#k-nearest-neighbors-algorithm)
      - [Plug-in classifier excess-risk bound](statistical-learning.md#plug-in-classifier-excess-risk-bound)
      - [Support vector machine](statistical-learning.md#support-vector-machine)
      - [Perceptron](statistical-learning.md#perceptron)
    - [Cross-validation](statistical-learning.md#cross-validation)
      - [Nested cross-validation](statistical-learning.md#nested-cross-validation)
      - [Biased cross-validation for density bandwidth](statistical-learning.md#biased-cross-validation-for-density-bandwidth)
      - [Least-squares cross-validation for density bandwidth](statistical-learning.md#least-squares-cross-validation-for-density-bandwidth)
      - [Generalized cross-validation](statistical-learning.md#generalized-cross-validation)
      - [Leave-one-out cross-validation](statistical-learning.md#leave-one-out-cross-validation)
      - [K-fold cross-validation](statistical-learning.md#k-fold-cross-validation)
    - [Neural network](statistical-learning.md#neural-network)
      - [Winner-take-all network](statistical-learning.md#winner-take-all-network)
      - [Exploding gradient problem](statistical-learning.md#exploding-gradient-problem)
      - [Vanishing gradient problem](statistical-learning.md#vanishing-gradient-problem)
      - [Recurrent neural network](statistical-learning.md#recurrent-neural-network)
      - [Dropout](statistical-learning.md#dropout)
      - [Residual connection](statistical-learning.md#residual-connection)
      - [Layer normalization](statistical-learning.md#layer-normalization)
      - [Transformer model](statistical-learning.md#transformer-model)
      - [Neural network bias](statistical-learning.md#neural-network-bias)
      - [Weight sharing](statistical-learning.md#weight-sharing)
      - [Convolutional neural network](statistical-learning.md#convolutional-neural-network)
      - [Binary threshold unit](statistical-learning.md#binary-threshold-unit)
      - [Activation function](statistical-learning.md#activation-function)
      - [Associative memory in neural networks](statistical-learning.md#associative-memory-in-neural-networks)
      - [Hopfield network](statistical-learning.md#hopfield-network)
      - [Boltzmann machine](statistical-learning.md#boltzmann-machine)
      - [Feedforward neural network](statistical-learning.md#feedforward-neural-network)
      - [Sigmoid function](statistical-learning.md#sigmoid-function)
      - [Rectified linear unit](statistical-learning.md#rectified-linear-unit)
      - [Gaussian error linear unit](statistical-learning.md#gaussian-error-linear-unit)
      - [Softmax function](statistical-learning.md#softmax-function)
    - [Overfitting](statistical-learning.md#overfitting)
      - [Underfitting](statistical-learning.md#underfitting)
    - [Regularization](statistical-learning.md#regularization)
      - [Penalized least squares](statistical-learning.md#penalized-least-squares)
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
    - [Variable selection](statistical-modelling.md#variable-selection)
    - [Nonregular mixture model selection](statistical-modelling.md#nonregular-mixture-model-selection)
    - [Akaike information criterion](statistical-modelling.md#akaike-information-criterion)
      - [Corrected Akaike information criterion](statistical-modelling.md#corrected-akaike-information-criterion)
      - [Stepwise selection by the Akaike information criterion](statistical-modelling.md#stepwise-selection-by-the-akaike-information-criterion)
      - [Distribution of the Akaike information criterion in a normal linear model](statistical-modelling.md#distribution-of-the-akaike-information-criterion-in-a-normal-linear-model)
      - [Mallows's Cp](statistical-modelling.md#mallows-s-cp)
    - [Bayesian information criterion](statistical-modelling.md#bayesian-information-criterion)
  - [Shape parameter](statistical-modelling.md#shape-parameter)
  - [Precision parameter](statistical-modelling.md#precision-parameter)
  - [Exponential family](exponential-family.md)
    - [Curved exponential family](exponential-family.md#curved-exponential-family)
      - [Normal mean proportional to standard deviation model](exponential-family.md#normal-mean-proportional-to-standard-deviation-model)
      - [Conditional scale density in a curved Gaussian family](exponential-family.md#conditional-scale-density-in-a-curved-gaussian-family)
    - [Minimal exponential family](exponential-family.md#minimal-exponential-family)
    - [Natural exponential family](exponential-family.md#natural-exponential-family)
      - [Convex support of an exponential family](exponential-family.md#convex-support-of-an-exponential-family)
      - [Regular natural exponential family](exponential-family.md#regular-natural-exponential-family)
      - [Full natural exponential family](exponential-family.md#full-natural-exponential-family)
    - [Normal natural-mean parameter ratio estimator](exponential-family.md#normal-natural-mean-parameter-ratio-estimator)
    - [Log-density domination in an exponential family](exponential-family.md#log-density-domination-in-an-exponential-family)
    - [Conjugate prior](exponential-family.md#conjugate-prior)
      - [Normal-gamma distribution](exponential-family.md#normal-gamma-distribution)
      - [Gamma rate gamma conjugacy](exponential-family.md#gamma-rate-gamma-conjugacy)
      - [Uniform-Pareto conjugacy](exponential-family.md#uniform-pareto-conjugacy)
      - [Gamma scale inverse-gamma conjugacy](exponential-family.md#gamma-scale-inverse-gamma-conjugacy)
      - [Normal-inverse-gamma prior](exponential-family.md#normal-inverse-gamma-prior)
      - [Natural conjugate prior](exponential-family.md#natural-conjugate-prior)
    - [Natural parameter of an exponential family](exponential-family.md#natural-parameter-of-an-exponential-family)
      - [Natural parameter space](exponential-family.md#natural-parameter-space)
    - [Cumulant function of an exponential family](exponential-family.md#cumulant-function-of-an-exponential-family)
      - [Exponential-family derivative identities](exponential-family.md#exponential-family-derivative-identities)
      - [Mean parameter of an exponential family](exponential-family.md#mean-parameter-of-an-exponential-family)
    - [Inverse Gaussian distribution](exponential-family.md#inverse-gaussian-distribution)
      - [Inverse Gaussian mean estimation](exponential-family.md#inverse-gaussian-mean-estimation)
      - [Inverse Gaussian shape estimation and nuisance orthogonality](exponential-family.md#inverse-gaussian-shape-estimation-and-nuisance-orthogonality)
      - [Inverse Gaussian sum closure](exponential-family.md#inverse-gaussian-sum-closure)
      - [Chi-squared transform of an inverse Gaussian variable](exponential-family.md#chi-squared-transform-of-an-inverse-gaussian-variable)
      - [Reciprocal-root inverse Gaussian sampler](exponential-family.md#reciprocal-root-inverse-gaussian-sampler)
    - [Exponential-family deviance](exponential-family.md#exponential-family-deviance)
      - [Scaled deviance](exponential-family.md#scaled-deviance)
    - [Negative binomial exponential family](exponential-family.md#negative-binomial-exponential-family)
    - [Exponential dispersion model](exponential-family.md#exponential-dispersion-model)
      - [Exponential dispersion family of order one](exponential-family.md#exponential-dispersion-family-of-order-one)
      - [Dispersion parameter](exponential-family.md#dispersion-parameter)
      - [Variance function](exponential-family.md#variance-function)
  - [Generalized linear model](generalized-linear-model.md)
    - [Gamma regression with canonical link](generalized-linear-model.md#gamma-regression-with-canonical-link)
    - [Generalized linear model offset](generalized-linear-model.md#generalized-linear-model-offset)
    - [Deviance goodness-of-fit test](generalized-linear-model.md#deviance-goodness-of-fit-test)
      - [Individual Bernoulli deviance need not have a chi-squared calibration](generalized-linear-model.md#individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration)
    - [Deviance residual](generalized-linear-model.md#deviance-residual)
    - [Generalized additive model](generalized-linear-model.md#generalized-additive-model)
      - [Additive regression model](generalized-linear-model.md#additive-regression-model)
      - [Backfitting algorithm](generalized-linear-model.md#backfitting-algorithm)
      - [Generalized additive mixed model](generalized-linear-model.md#generalized-additive-mixed-model)
    - [Quasi-likelihood](generalized-linear-model.md#quasi-likelihood)
      - [Quasibinomial regression](generalized-linear-model.md#quasibinomial-regression)
    - [Linear predictor](generalized-linear-model.md#linear-predictor)
    - [Link function](generalized-linear-model.md#link-function)
      - [Complementary log-log link](generalized-linear-model.md#complementary-log-log-link)
      - [Identity link](generalized-linear-model.md#identity-link)
      - [Logit](generalized-linear-model.md#logit)
      - [Logarithmic link function](generalized-linear-model.md#logarithmic-link-function)
    - [Binomial regression](generalized-linear-model.md#binomial-regression)
      - [Binomial deviance](generalized-linear-model.md#binomial-deviance)
    - [Pearson dispersion estimator](generalized-linear-model.md#pearson-dispersion-estimator)
      - [Pearson residual](generalized-linear-model.md#pearson-residual)
      - [Pearson chi-squared statistic](generalized-linear-model.md#pearson-chi-squared-statistic)
    - [Canonical link function](generalized-linear-model.md#canonical-link-function)
      - [Poisson canonical link](generalized-linear-model.md#poisson-canonical-link)
    - [Poisson regression](generalized-linear-model.md#poisson-regression)
      - [Profile likelihood for a common Poisson rate ratio with unequal exposures](generalized-linear-model.md#profile-likelihood-for-a-common-poisson-rate-ratio-with-unequal-exposures)
      - [Concavity of the Poisson regression likelihood](generalized-linear-model.md#concavity-of-the-poisson-regression-likelihood)
      - [Poisson slope information after eliminating an intercept](generalized-linear-model.md#poisson-slope-information-after-eliminating-an-intercept)
      - [Poisson regression margin-matching score equations](generalized-linear-model.md#poisson-regression-margin-matching-score-equations)
      - [Two-group Poisson ratio conditional likelihood](generalized-linear-model.md#two-group-poisson-ratio-conditional-likelihood)
      - [Common versus factor-specific slopes in Poisson regression](generalized-linear-model.md#common-versus-factor-specific-slopes-in-poisson-regression)
      - [Poisson working models for averaged counts](generalized-linear-model.md#poisson-working-models-for-averaged-counts)
      - [Poisson log-rate ratio](generalized-linear-model.md#poisson-log-rate-ratio)
      - [Poisson mean saturation at three distinct times](generalized-linear-model.md#poisson-mean-saturation-at-three-distinct-times)
      - [Pooling selected slopes in a Poisson regression](generalized-linear-model.md#pooling-selected-slopes-in-a-poisson-regression)
      - [Treatment interaction contrast in a Poisson regression](generalized-linear-model.md#treatment-interaction-contrast-in-a-poisson-regression)
      - [Poisson deviance](generalized-linear-model.md#poisson-deviance)
    - [Gamma regression with logarithmic link](generalized-linear-model.md#gamma-regression-with-logarithmic-link)
    - [Quasi-Poisson regression](generalized-linear-model.md#quasi-poisson-regression)
      - [Poisson score linearization under proportional variance](generalized-linear-model.md#poisson-score-linearization-under-proportional-variance)
      - [Quasi-score equation](generalized-linear-model.md#quasi-score-equation)
    - [Negative binomial regression](generalized-linear-model.md#negative-binomial-regression)
      - [Fixed-size negative binomial generalized linear model](generalized-linear-model.md#fixed-size-negative-binomial-generalized-linear-model)
    - [Poisson exposure model](generalized-linear-model.md#poisson-exposure-model)
      - [Exposure time for a Poisson rate at fixed fractional precision](generalized-linear-model.md#exposure-time-for-a-poisson-rate-at-fixed-fractional-precision)
      - [Rate ratio](generalized-linear-model.md#rate-ratio)
      - [Finite-exposure Poisson inconsistency](generalized-linear-model.md#finite-exposure-poisson-inconsistency)
      - [Estimators for a Poisson exposure model](generalized-linear-model.md#estimators-for-a-poisson-exposure-model)
      - [Normal-approximation tests for a Poisson exposure model](generalized-linear-model.md#normal-approximation-tests-for-a-poisson-exposure-model)
    - [Logistic regression](generalized-linear-model.md#logistic-regression)
      - [Proportional-odds model](generalized-linear-model.md#proportional-odds-model)
      - [Separation in logistic regression](generalized-linear-model.md#separation-in-logistic-regression)
      - [Finite maximum-likelihood estimate in a one-parameter logistic model](generalized-linear-model.md#finite-maximum-likelihood-estimate-in-a-one-parameter-logistic-model)
      - [Conditional logistic model for longitudinal binary data](generalized-linear-model.md#conditional-logistic-model-for-longitudinal-binary-data)
      - [Multinomial logistic regression](generalized-linear-model.md#multinomial-logistic-regression)
      - [Logistic-normal regression with autoregressive random effects](generalized-linear-model.md#logistic-normal-regression-with-autoregressive-random-effects)
      - [Logistic model](generalized-linear-model.md#logistic-model)
      - [Separation (statistics)](generalized-linear-model.md#separation-statistics)
      - [Bernoulli logistic-regression model](generalized-linear-model.md#bernoulli-logistic-regression-model)
      - [Logistic loss](generalized-linear-model.md#logistic-loss)
      - [L1-penalized logistic regression](generalized-linear-model.md#l1-penalized-logistic-regression)
      - [Grouped-binomial logistic regression](generalized-linear-model.md#grouped-binomial-logistic-regression)
      - [Reference level in a regression factor](generalized-linear-model.md#reference-level-in-a-regression-factor)
      - [Stochastic block model](generalized-linear-model.md#stochastic-block-model)
    - [Probit model](generalized-linear-model.md#probit-model)
      - [Latent-normal Gibbs sampler for probit regression](generalized-linear-model.md#latent-normal-gibbs-sampler-for-probit-regression)
      - [Threshold observation of a lognormal regression](generalized-linear-model.md#threshold-observation-of-a-lognormal-regression)
      - [Probit posterior score](generalized-linear-model.md#probit-posterior-score)
    - [Iteratively reweighted least squares](generalized-linear-model.md#iteratively-reweighted-least-squares)
    - [Generalized linear mixed model](generalized-linear-model.md#generalized-linear-mixed-model)
      - [Logistic random-intercept model for repeated binary outcomes](generalized-linear-model.md#logistic-random-intercept-model-for-repeated-binary-outcomes)
      - [Gaussian linear mixed model](generalized-linear-model.md#gaussian-linear-mixed-model)
      - [Poisson generalized linear mixed model](generalized-linear-model.md#poisson-generalized-linear-mixed-model)
      - [Random intercept](generalized-linear-model.md#random-intercept)
  - [Clustered data](statistical-modelling.md#clustered-data)
    - [Pseudoreplication](statistical-modelling.md#pseudoreplication)
  - [Independent Poisson conditioning](statistical-modelling.md#independent-poisson-conditioning)
  - [Normal linear model](normal-linear-model.md)
    - [Variance of a fitted regression mean](normal-linear-model.md#variance-of-a-fitted-regression-mean)
    - [Analysis of covariance](normal-linear-model.md#analysis-of-covariance)
    - [Normal linear model maximum-likelihood sampling distributions](normal-linear-model.md#normal-linear-model-maximum-likelihood-sampling-distributions)
    - [Lack of fit](normal-linear-model.md#lack-of-fit)
      - [Lack-of-fit F-test](normal-linear-model.md#lack-of-fit-f-test)
    - [Pure error](normal-linear-model.md#pure-error)
    - [Two-factor normal linear model](normal-linear-model.md#two-factor-normal-linear-model)
      - [Factor-level pooling test](normal-linear-model.md#factor-level-pooling-test)
    - [Joint distribution of least-squares and variance estimators](normal-linear-model.md#joint-distribution-of-least-squares-and-variance-estimators)
    - [Restricted maximum likelihood](normal-linear-model.md#restricted-maximum-likelihood)
      - [Restricted likelihood from orthogonal error contrasts](normal-linear-model.md#restricted-likelihood-from-orthogonal-error-contrasts)
    - [Gaussian conjugacy for a normal linear model](normal-linear-model.md#gaussian-conjugacy-for-a-normal-linear-model)
      - [Normal regression with independent coefficient and variance priors](normal-linear-model.md#normal-regression-with-independent-coefficient-and-variance-priors)
      - [Gaussian conjugacy for an initialized AR(2) regression](normal-linear-model.md#gaussian-conjugacy-for-an-initialized-ar-2-regression)
      - [Normal-gamma posterior with a flat prior](normal-linear-model.md#normal-gamma-posterior-with-a-flat-prior)
      - [Gaussian posterior in the zero-noise limit](normal-linear-model.md#gaussian-posterior-in-the-zero-noise-limit)
      - [Gaussian likelihood](normal-linear-model.md#gaussian-likelihood)
    - [Cochran's theorem](normal-linear-model.md#cochran-s-theorem)
      - [Rank-sum form of Cochran's theorem](normal-linear-model.md#rank-sum-form-of-cochran-s-theorem)
    - [Linear regression](linear-regression.md)
      - [Independent slope and curvature estimates in a symmetric quadratic design](linear-regression.md#independent-slope-and-curvature-estimates-in-a-symmetric-quadratic-design)
      - [Orthogonal centered quadratic regression design](linear-regression.md#orthogonal-centered-quadratic-regression-design)
      - [Asymptotic normality of a weighted regression slope](linear-regression.md#asymptotic-normality-of-a-weighted-regression-slope)
      - [Linear regression model](linear-regression.md#linear-regression-model)
      - [Log-linear exponential-decay fit](linear-regression.md#log-linear-exponential-decay-fit)
      - [Multiple linear regression](linear-regression.md#multiple-linear-regression)
      - [Normal equations for linear least squares](linear-regression.md#normal-equations-for-linear-least-squares)
      - [Omitted-variable bias](linear-regression.md#omitted-variable-bias)
      - [Predictor centering](linear-regression.md#predictor-centering)
      - [Regression diagnostics](linear-regression.md#regression-diagnostics)
      - [Least angle regression](linear-regression.md#least-angle-regression)
      - [Reciprocal-predictor regression](linear-regression.md#reciprocal-predictor-regression)
      - [Regression intercept](linear-regression.md#regression-intercept)
      - [Polynomial regression](linear-regression.md#polynomial-regression)
      - [Coefficient of determination](linear-regression.md#coefficient-of-determination)
      - [Residual-versus-fitted plot](linear-regression.md#residual-versus-fitted-plot)
      - [Analysis of variance](linear-regression.md#analysis-of-variance)
      - [Frisch–Waugh–Lovell theorem](linear-regression.md#frisch-waugh-lovell-theorem)
      - [Simple linear regression](linear-regression.md#simple-linear-regression)
      - [Residual sum of squares](linear-regression.md#residual-sum-of-squares)
      - [Ridge regression](linear-regression.md#ridge-regression)
      - [Fitted values](linear-regression.md#fitted-values)
      - [Design matrix](linear-regression.md#design-matrix)
      - [Regression coefficient](linear-regression.md#regression-coefficient)
      - [Attenuation bias from classical measurement error](linear-regression.md#attenuation-bias-from-classical-measurement-error)
    - [R linear-model formula](normal-linear-model.md#r-linear-model-formula)
      - [Treatment coding](normal-linear-model.md#treatment-coding)
      - [Degrees of freedom of a factor predictor](normal-linear-model.md#degrees-of-freedom-of-a-factor-predictor)
    - [Hat matrix](normal-linear-model.md#hat-matrix)
      - [Fitted-residual orthogonality](normal-linear-model.md#fitted-residual-orthogonality)
    - [Normal linear-model confidence ellipsoid](normal-linear-model.md#normal-linear-model-confidence-ellipsoid)
      - [Cook's distance](normal-linear-model.md#cook-s-distance)
    - [Multicollinearity](normal-linear-model.md#multicollinearity)
      - [Variance inflation factor](normal-linear-model.md#variance-inflation-factor)
      - [Two-predictor variance inflation](normal-linear-model.md#two-predictor-variance-inflation)
    - [Ordinary least squares](normal-linear-model.md#ordinary-least-squares)
      - [Residual estimate of Gaussian noise variance](normal-linear-model.md#residual-estimate-of-gaussian-noise-variance)
      - [Partial regression](normal-linear-model.md#partial-regression)
      - [Rank-deficient ordinary least squares](normal-linear-model.md#rank-deficient-ordinary-least-squares)
      - [Linear regression through the origin](normal-linear-model.md#linear-regression-through-the-origin)
      - [Ordinary least squares estimators](normal-linear-model.md#ordinary-least-squares-estimators)
    - [Gauss-Markov theorem](normal-linear-model.md#gauss-markov-theorem)
    - [Weighted least squares](normal-linear-model.md#weighted-least-squares)
      - [Admissible polynomials for a singular inverse-linear weight](normal-linear-model.md#admissible-polynomials-for-a-singular-inverse-linear-weight)
      - [Endpoint concentration in weighted constant approximation](normal-linear-model.md#endpoint-concentration-in-weighted-constant-approximation)
      - [Gamma-ray energy-network fit](normal-linear-model.md#gamma-ray-energy-network-fit)
      - [Additional measurements decrease known-error covariance](normal-linear-model.md#additional-measurements-decrease-known-error-covariance)
      - [Fixed-phase sinusoidal least squares](normal-linear-model.md#fixed-phase-sinusoidal-least-squares)
      - [Variable projection](normal-linear-model.md#variable-projection)
      - [Generalized least squares](normal-linear-model.md#generalized-least-squares)
    - [Normal equation](normal-linear-model.md#normal-equation)
    - [Consistency of least squares](normal-linear-model.md#consistency-of-least-squares)
    - [One-way normal linear model](normal-linear-model.md#one-way-normal-linear-model)
      - [Cell-means parametrization](normal-linear-model.md#cell-means-parametrization)
      - [Full-dominance mean constraint](normal-linear-model.md#full-dominance-mean-constraint)
      - [Additive allele-count model](normal-linear-model.md#additive-allele-count-model)
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
  - [Maximum likelihood estimation](maximum-likelihood-estimation.md)
    - [Normal likelihood with variance equal to squared mean](maximum-likelihood-estimation.md#normal-likelihood-with-variance-equal-to-squared-mean)
    - [Singular covariance and nonexistence of a Gaussian maximum likelihood estimate](maximum-likelihood-estimation.md#singular-covariance-and-nonexistence-of-a-gaussian-maximum-likelihood-estimate)
    - [Compact-parameter consistency of maximum likelihood](maximum-likelihood-estimation.md#compact-parameter-consistency-of-maximum-likelihood)
    - [Shifted exponential maximum likelihood](maximum-likelihood-estimation.md#shifted-exponential-maximum-likelihood)
      - [Exact endpoint limit for a shifted exponential distribution](maximum-likelihood-estimation.md#exact-endpoint-limit-for-a-shifted-exponential-distribution)
    - [Maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator)
      - [Likelihood supremum at an excluded boundary](maximum-likelihood-estimation.md#likelihood-supremum-at-an-excluded-boundary)
      - [Uniform endpoint maximum-likelihood estimator](maximum-likelihood-estimation.md#uniform-endpoint-maximum-likelihood-estimator)
      - [Neyman-Scott incidental parameter problem](maximum-likelihood-estimation.md#neyman-scott-incidental-parameter-problem)
      - [Endpoint maximum likelihood for a singular location density](maximum-likelihood-estimation.md#endpoint-maximum-likelihood-for-a-singular-location-density)
      - [Exponential-rate maximum-likelihood estimator](maximum-likelihood-estimation.md#exponential-rate-maximum-likelihood-estimator)
      - [Maximum-likelihood fitted value](maximum-likelihood-estimation.md#maximum-likelihood-fitted-value)
      - [Normal mean and variance maximum-likelihood estimators](maximum-likelihood-estimation.md#normal-mean-and-variance-maximum-likelihood-estimators)
      - [Invariance property of maximum likelihood estimation](maximum-likelihood-estimation.md#invariance-property-of-maximum-likelihood-estimation)
      - [Likelihood function](maximum-likelihood-estimation.md#likelihood-function)
      - [Binomial proportion maximum-likelihood estimator](maximum-likelihood-estimation.md#binomial-proportion-maximum-likelihood-estimator)
      - [Exponential distribution rate estimator](maximum-likelihood-estimation.md#exponential-distribution-rate-estimator)
      - [Asymptotic normality of a maximum likelihood estimator](maximum-likelihood-estimation.md#asymptotic-normality-of-a-maximum-likelihood-estimator)
  - [Logistic distribution](statistical-modelling.md#logistic-distribution)
    - [Location-scale form of the logistic distribution](statistical-modelling.md#location-scale-form-of-the-logistic-distribution)
  - [Gaussian conditional expectation](statistical-modelling.md#gaussian-conditional-expectation)
  - [Linear discriminant analysis](statistical-modelling.md#linear-discriminant-analysis)
    - [Canonical discriminant directions](statistical-modelling.md#canonical-discriminant-directions)
    - [Kernel linear discriminant analysis](statistical-modelling.md#kernel-linear-discriminant-analysis)
  - [Quadratic discriminant analysis](statistical-modelling.md#quadratic-discriminant-analysis)
  - [Bootstrapping (statistics)](statistical-modelling.md#bootstrapping-statistics)
    - [Exact bootstrap distribution for three observations](statistical-modelling.md#exact-bootstrap-distribution-for-three-observations)
    - [Bootstrap publication history](statistical-modelling.md#bootstrap-publication-history)
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
      - [Bias-variance decomposition of mean squared error](statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error)
      - [Affine shrinkage estimator for a binomial proportion](statistical-modelling.md#affine-shrinkage-estimator-for-a-binomial-proportion)
    - [Admissible decision rule](statistical-modelling.md#admissible-decision-rule)
      - [Admissible estimator](statistical-modelling.md#admissible-estimator)
    - [Minimax estimator](statistical-modelling.md#minimax-estimator)
      - [Constant-risk binomial proportion estimator](statistical-modelling.md#constant-risk-binomial-proportion-estimator)
      - [Minimax risk](statistical-modelling.md#minimax-risk)
      - [Minimaxity of the usual multivariate normal mean estimator](statistical-modelling.md#minimaxity-of-the-usual-multivariate-normal-mean-estimator)
  - [Cramér-Rao bound](statistical-modelling.md#cramer-rao-bound)
    - [Efficient estimator](statistical-modelling.md#efficient-estimator)
    - [Van Trees inequality](statistical-modelling.md#van-trees-inequality)
  - [Informant function](statistical-modelling.md#informant-function)
    - [Score-function gradient estimator](statistical-modelling.md#score-function-gradient-estimator)
      - [Constant score baseline](statistical-modelling.md#constant-score-baseline)
    - [Gaussian regression score](statistical-modelling.md#gaussian-regression-score)
    - [Score equation](statistical-modelling.md#score-equation)
    - [Mean-zero score identity](statistical-modelling.md#mean-zero-score-identity)
    - [Fisher information matrix](statistical-modelling.md#fisher-information-matrix)
      - [Fisher information in an exponential survival snapshot](statistical-modelling.md#fisher-information-in-an-exponential-survival-snapshot)
      - [Fisher information loss from thresholding an exponential observation](statistical-modelling.md#fisher-information-loss-from-thresholding-an-exponential-observation)
      - [Fisher information per observation and per trial](statistical-modelling.md#fisher-information-per-observation-and-per-trial)
      - [Orthogonal statistical parameters](statistical-modelling.md#orthogonal-statistical-parameters)
      - [Jeffreys prior](statistical-modelling.md#jeffreys-prior)
      - [Fisher information of a multivariate normal location model](statistical-modelling.md#fisher-information-of-a-multivariate-normal-location-model)
      - [Empirical score outer-product information](statistical-modelling.md#empirical-score-outer-product-information)
      - [Observed Fisher information](statistical-modelling.md#observed-fisher-information)
      - [Tensorization of Fisher information](statistical-modelling.md#tensorization-of-fisher-information)
      - [Fisher information in a stationary Gaussian autoregressive location model](statistical-modelling.md#fisher-information-in-a-stationary-gaussian-autoregressive-location-model)
      - [Scoring algorithm](statistical-modelling.md#scoring-algorithm)
      - [Information identity](statistical-modelling.md#information-identity)
      - [Normal location-scale score](statistical-modelling.md#normal-location-scale-score)
      - [Local asymptotic normality](statistical-modelling.md#local-asymptotic-normality)
  - [Statistical hypothesis test](statistical-hypothesis-test.md)
    - [Equivalence test](statistical-hypothesis-test.md#equivalence-test)
    - [Randomized statistical test](statistical-hypothesis-test.md#randomized-statistical-test)
    - [False alarm rate](statistical-hypothesis-test.md#false-alarm-rate)
    - [Statistical hypothesis](statistical-hypothesis-test.md#statistical-hypothesis)
    - [Sequential probability ratio test](statistical-hypothesis-test.md#sequential-probability-ratio-test)
    - [Statistical significance](statistical-hypothesis-test.md#statistical-significance)
      - [Poisson tail discovery probability](statistical-hypothesis-test.md#poisson-tail-discovery-probability)
      - [Look-elsewhere effect](statistical-hypothesis-test.md#look-elsewhere-effect)
    - [Two-sided hypothesis test](statistical-hypothesis-test.md#two-sided-hypothesis-test)
    - [One-sided hypothesis test](statistical-hypothesis-test.md#one-sided-hypothesis-test)
    - [Alternative hypothesis](statistical-hypothesis-test.md#alternative-hypothesis)
    - [Hotelling's T-squared statistic](statistical-hypothesis-test.md#hotelling-s-t-squared-statistic)
      - [Affine invariance of Hotelling's statistic](statistical-hypothesis-test.md#affine-invariance-of-hotelling-s-statistic)
      - [Hotelling test of linear hypotheses](statistical-hypothesis-test.md#hotelling-test-of-linear-hypotheses)
    - [Rejection region](statistical-hypothesis-test.md#rejection-region)
    - [McNemar's test](statistical-hypothesis-test.md#mcnemar-s-test)
      - [Equality criterion for paired and unpaired allele tests](statistical-hypothesis-test.md#equality-criterion-for-paired-and-unpaired-allele-tests)
      - [Paired binary sample size calculation](statistical-hypothesis-test.md#paired-binary-sample-size-calculation)
    - [Significant and nonsignificant results need not differ significantly](statistical-hypothesis-test.md#significant-and-nonsignificant-results-need-not-differ-significantly)
    - [Monte Carlo test](statistical-hypothesis-test.md#monte-carlo-test)
    - [Predictive discrepancy statistic](statistical-hypothesis-test.md#predictive-discrepancy-statistic)
    - [Scan statistic](statistical-hypothesis-test.md#scan-statistic)
      - [Cyclic interval overlap bound](statistical-hypothesis-test.md#cyclic-interval-overlap-bound)
      - [Quadratic scan statistic](statistical-hypothesis-test.md#quadratic-scan-statistic)
    - [Least-favourable null configuration](statistical-hypothesis-test.md#least-favourable-null-configuration)
    - [Pearson chi-squared test of homogeneity](statistical-hypothesis-test.md#pearson-chi-squared-test-of-homogeneity)
      - [Empty groups in a binomial homogeneity test](statistical-hypothesis-test.md#empty-groups-in-a-binomial-homogeneity-test)
      - [Pearson chi-squared statistic for contingency tables](statistical-hypothesis-test.md#pearson-chi-squared-statistic-for-contingency-tables)
    - [Statistical test](statistical-hypothesis-test.md#statistical-test)
      - [Most powerful test](statistical-hypothesis-test.md#most-powerful-test)
    - [Test statistic](statistical-hypothesis-test.md#test-statistic)
      - [Null distribution](statistical-hypothesis-test.md#null-distribution)
    - [Student's t-test](statistical-hypothesis-test.md#student-s-t-test)
      - [Consistency identities for a two-sided t-test](statistical-hypothesis-test.md#consistency-identities-for-a-two-sided-t-test)
      - [Paired t-test](statistical-hypothesis-test.md#paired-t-test)
      - [Welch's t-test](statistical-hypothesis-test.md#welch-s-t-test)
      - [Exact pooled two-sample t statistic](statistical-hypothesis-test.md#exact-pooled-two-sample-t-statistic)
      - [Normal-mean likelihood ratio with unknown variance](statistical-hypothesis-test.md#normal-mean-likelihood-ratio-with-unknown-variance)
      - [Regression coefficient test power ignores nuisance coefficients](statistical-hypothesis-test.md#regression-coefficient-test-power-ignores-nuisance-coefficients)
    - [Fixed alternative](statistical-hypothesis-test.md#fixed-alternative)
    - [Local alternative](statistical-hypothesis-test.md#local-alternative)
    - [Randomization test](statistical-hypothesis-test.md#randomization-test)
      - [Conditional randomization test](statistical-hypothesis-test.md#conditional-randomization-test)
      - [Permutation test](statistical-hypothesis-test.md#permutation-test)
      - [Sign-flip randomization test](statistical-hypothesis-test.md#sign-flip-randomization-test)
    - [Null hypothesis](statistical-hypothesis-test.md#null-hypothesis)
    - [Simple hypothesis](statistical-hypothesis-test.md#simple-hypothesis)
    - [Size of a statistical test](statistical-hypothesis-test.md#size-of-a-statistical-test)
    - [Significance level](statistical-hypothesis-test.md#significance-level)
    - [P-value](statistical-hypothesis-test.md#p-value)
      - [Super-uniform random variable](statistical-hypothesis-test.md#super-uniform-random-variable)
    - [Fisher's exact test](statistical-hypothesis-test.md#fisher-s-exact-test)
      - [Exact power of Fisher's exact test](statistical-hypothesis-test.md#exact-power-of-fisher-s-exact-test)
    - [Maximin test](statistical-hypothesis-test.md#maximin-test)
    - [Multiple hypothesis testing](statistical-hypothesis-test.md#multiple-hypothesis-testing)
      - [Intersection hypothesis](statistical-hypothesis-test.md#intersection-hypothesis)
      - [Hochberg procedure](statistical-hypothesis-test.md#hochberg-procedure)
      - [Simes inequality](statistical-hypothesis-test.md#simes-inequality)
      - [Weighted interval testing for a piecewise-constant mean](statistical-hypothesis-test.md#weighted-interval-testing-for-a-piecewise-constant-mean)
      - [Intersection-union test](statistical-hypothesis-test.md#intersection-union-test)
      - [Bonferroni correction](statistical-hypothesis-test.md#bonferroni-correction)
      - [Benjamini-Hochberg procedure](statistical-hypothesis-test.md#benjamini-hochberg-procedure)
      - [False discovery rate](statistical-hypothesis-test.md#false-discovery-rate)
      - [Familywise error rate](statistical-hypothesis-test.md#familywise-error-rate)
      - [Closed testing procedure](statistical-hypothesis-test.md#closed-testing-procedure)
    - [Joint hypothesis test](statistical-hypothesis-test.md#joint-hypothesis-test)
    - [Power function of a statistical test](statistical-hypothesis-test.md#power-function-of-a-statistical-test)
      - [A p-value does not determine the type II error probability](statistical-hypothesis-test.md#a-p-value-does-not-determine-the-type-ii-error-probability)
    - [Uniformly most powerful test](statistical-hypothesis-test.md#uniformly-most-powerful-test)
      - [Normal sample-size design for an upper-tail Poisson test](statistical-hypothesis-test.md#normal-sample-size-design-for-an-upper-tail-poisson-test)
      - [Crossing-power obstruction to a uniformly most powerful test](statistical-hypothesis-test.md#crossing-power-obstruction-to-a-uniformly-most-powerful-test)
    - [Pearson's chi-squared test](statistical-hypothesis-test.md#pearson-s-chi-squared-test)
      - [Joint conditional independence test for stratified contingency tables](statistical-hypothesis-test.md#joint-conditional-independence-test-for-stratified-contingency-tables)
      - [Pearson chi-squared goodness-of-fit test](statistical-hypothesis-test.md#pearson-chi-squared-goodness-of-fit-test)
    - [Likelihood-ratio test of independence in a contingency table](statistical-hypothesis-test.md#likelihood-ratio-test-of-independence-in-a-contingency-table)
      - [Aggregation can change a contingency-table independence test](statistical-hypothesis-test.md#aggregation-can-change-a-contingency-table-independence-test)
    - [Linear-by-linear association test](statistical-hypothesis-test.md#linear-by-linear-association-test)
    - [Wald test](statistical-hypothesis-test.md#wald-test)
      - [Signed normal Wald statistic](statistical-hypothesis-test.md#signed-normal-wald-statistic)
      - [Wald statistics with a shared control](statistical-hypothesis-test.md#wald-statistics-with-a-shared-control)
      - [Multivariate Wald statistic](statistical-hypothesis-test.md#multivariate-wald-statistic)
      - [Wald and likelihood-ratio asymptotic equivalence](statistical-hypothesis-test.md#wald-and-likelihood-ratio-asymptotic-equivalence)
      - [Two-sided Gaussian p-value](statistical-hypothesis-test.md#two-sided-gaussian-p-value)
    - [Likelihood-ratio test](statistical-hypothesis-test.md#likelihood-ratio-test)
      - [Likelihood-ratio test for equality of exponential means](statistical-hypothesis-test.md#likelihood-ratio-test-for-equality-of-exponential-means)
      - [Likelihood-ratio test for equality of beta shape parameters](statistical-hypothesis-test.md#likelihood-ratio-test-for-equality-of-beta-shape-parameters)
      - [Likelihood-ratio test for a normal variance](statistical-hypothesis-test.md#likelihood-ratio-test-for-a-normal-variance)
      - [Gaussian covariance diagonality likelihood-ratio test](statistical-hypothesis-test.md#gaussian-covariance-diagonality-likelihood-ratio-test)
      - [Gaussian diagonal-covariance likelihood-ratio test](statistical-hypothesis-test.md#gaussian-diagonal-covariance-likelihood-ratio-test)
      - [One-sided likelihood-ratio test for two normal variances](statistical-hypothesis-test.md#one-sided-likelihood-ratio-test-for-two-normal-variances)
      - [Boundary likelihood-ratio test for two Gaussian means](statistical-hypothesis-test.md#boundary-likelihood-ratio-test-for-two-gaussian-means)
      - [Single-parameter boundary likelihood-ratio test](statistical-hypothesis-test.md#single-parameter-boundary-likelihood-ratio-test)
      - [Variance-component likelihood-ratio test at a boundary](statistical-hypothesis-test.md#variance-component-likelihood-ratio-test-at-a-boundary)
      - [Likelihood ratio](statistical-hypothesis-test.md#likelihood-ratio)
      - [Likelihood-ratio test statistic](statistical-hypothesis-test.md#likelihood-ratio-test-statistic)
      - [Generalized likelihood-ratio test](statistical-hypothesis-test.md#generalized-likelihood-ratio-test)
    - [Score test](statistical-hypothesis-test.md#score-test)
      - [Restricted maximum-likelihood estimator](statistical-hypothesis-test.md#restricted-maximum-likelihood-estimator)
      - [Score test under a simple null](statistical-hypothesis-test.md#score-test-under-a-simple-null)
      - [Residual sum of squares in a normal sample](statistical-hypothesis-test.md#residual-sum-of-squares-in-a-normal-sample)
    - [Neyman-Pearson lemma](statistical-hypothesis-test.md#neyman-pearson-lemma)
      - [Shape-two Weibull scale likelihood-ratio test](statistical-hypothesis-test.md#shape-two-weibull-scale-likelihood-ratio-test)
      - [Fixed-mean normal variance test](statistical-hypothesis-test.md#fixed-mean-normal-variance-test)
      - [Uniformly most powerful test for a gamma rate](statistical-hypothesis-test.md#uniformly-most-powerful-test-for-a-gamma-rate)
      - [Most powerful test for a Laplace location shift](statistical-hypothesis-test.md#most-powerful-test-for-a-laplace-location-shift)
      - [Minimum sum of errors in a simple hypothesis test](statistical-hypothesis-test.md#minimum-sum-of-errors-in-a-simple-hypothesis-test)
      - [Exponential-rate likelihood-ratio test](statistical-hypothesis-test.md#exponential-rate-likelihood-ratio-test)
      - [Uniformly most powerful test for an exponential rate](statistical-hypothesis-test.md#uniformly-most-powerful-test-for-an-exponential-rate)
      - [Monotone likelihood ratio](statistical-hypothesis-test.md#monotone-likelihood-ratio)
  - [Grouped exponential observation](statistical-modelling.md#grouped-exponential-observation)
    - [Asymptotic information loss from grouping](statistical-modelling.md#asymptotic-information-loss-from-grouping)

## Parameter space

↑ **Parent:** [Statistical model](statistical-model.md)

The [parameter space](#parameter-space) of a [statistical model](statistical-model.md) is the set of allowed [statistical parameter](#statistical-parameter) values indexing its [probability distributions](probability-distribution.md). For an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) parametrized by its [mean](expected-value.md), $\Theta=(0,\infty)$; for a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution), $\Theta=[0,1]$. Intersecting a [confidence interval](statistical-inference.md#confidence-interval) with the known [parameter space](#parameter-space) cannot remove the true [statistical parameter](#statistical-parameter) and therefore preserves its [coverage probability](statistical-inference.md#coverage-probability).

## Parameter recovery

↑ **Parent:** [Statistical model](statistical-model.md)

Simulation of observations under known parameter values followed by refitting the model to assess whether those values can be recovered under the intended design. Recovery depends on information, noise and [identifiability](#identifiability); good recovery in an assumed model does not establish that the model describes the real mechanism.

## Mixed model

↑ **Parent:** [Statistical model](statistical-model.md)

A [statistical model](statistical-model.md) combining [fixed effects](statistical-modelling.md#fixed-effect) with [random effects](latent-variable.md#random-effect). The grouping structure determines the correlations represented by the model.

## Spatial Bernoulli infection model

↑ **Parent:** [Statistical model](statistical-model.md)

Given the currently infected set $I_t$ and susceptible set $S_t$, define $A_{it}(\eta)=\sum_{j\in I_t}K_\eta(d_{ij})$ and $P_{it}=1-e^{-\alpha A_{it}}$. Conditionally [independent](random-variable.md#independent-random-variables) new-infection indicators $Y_{it}$ have [likelihood](maximum-likelihood-estimation.md#likelihood-function)

$$
L(\alpha,\eta)=\prod_t\prod_{i\in S_t}(1-e^{-\alpha A_{it}(\eta)})^{Y_{it}}e^{-\alpha A_{it}(\eta)(1-Y_{it})}.
$$

A nonnegative infection intensity requires $\alpha\geq0$; an unrestricted [normal distribution](probability-distribution.md#normal-distribution) [prior distribution](bayesian-statistics.md#prior-probability) for $\alpha$ must therefore be restricted or replaced. With $K_\beta(d)=d^{-\beta}$ or $K_\gamma(d)=e^{-\gamma d}$ and positive distances, the conditional [posterior](bayesian-statistics.md#bayesian-posterior) kernels are not generally conjugate normal [probability densities](wave-function.md#probability-density). [Metropolis–Hastings algorithm](bayesian-statistics.md#metropolis-hastings-algorithm) updates, optionally on $\log\alpha$ with its [Jacobian determinant](multivariable-calculus.md#jacobian-determinant), provide a direct sampling method.

## Transformation model

↑ **Parent:** [Statistical model](statistical-model.md)

A [group action](group-action.md) on the sample space induces a compatible action on the parameter space, preserving the family of [probability laws](probability-distribution.md). In a transitive model every law arises by transforming a fixed reference law. A [location-scale model](#location-scale-family) is generated by $y\mapsto a+by$, $b>0$, with parameter action $(\mu,\sigma)\mapsto(a+b\mu,b\sigma)$.

### Equivariant estimator

↑ **Parent:** [Transformation model](#transformation-model)

An estimator respects the [group action](group-action.md) if the displayed identity holds. If it takes values in the transformation [group](group.md) itself, normalization $T(y)^{-1}y$ is a [maximal invariant](#maximal-invariant): equivariance proves invariance, and equality of normalized samples reconstructs the transformation between them. For estimates in a homogeneous parameter space with a nontrivial stabilizer, normalization is defined only modulo that stabilizer; quotienting the remaining action is essential.

### Maximal invariant

↑ **Parent:** [Transformation model](#transformation-model)

A statistic is invariant if $A(gy)=A(y)$; it is maximal when it also separates different [group orbits](group-action.md#orbit-group-theory). Consequently every invariant procedure factors through the [maximal invariant](#maximal-invariant), subject to the usual measurability conditions on the orbit space. Standardizing a sample by an [equivariant estimator](#equivariant-estimator) of location and positive scale gives a [maximal invariant](#maximal-invariant) for the positive affine [group](group.md).

#### Ranks as a maximal invariant under increasing transformations

↑ **Parent:** [Maximal invariant](#maximal-invariant)

On samples of distinct real observations, the labeled rank vector is a [maximal invariant](#maximal-invariant) for simultaneous strictly increasing bijections of the real line. Such transformations preserve every comparison. Conversely two samples with the same ranks can be matched by a piecewise linear increasing bijection through their corresponding ordered observations, with positive-slope tails. Under a common continuous [probability distribution](probability-distribution.md), every labeled ordering is equally likely by [exchangeability](probability-distribution.md#exchangeable-random-variables), giving distribution-free [rank tests](nonparametric-statistics.md#rank-test). This argument does not assume that all continuous distributions lie in one orbit of real-line homeomorphisms.

#### Invariant tests factor through a maximal invariant

↑ **Parent:** [Maximal invariant](#maximal-invariant)

If $T$ is a [maximal invariant](#maximal-invariant) for a [group action](group-action.md), an invariant test function is constant on each [group orbit](group-action.md#orbit-group-theory) and therefore equals $b\circ T$ for a function $b$ on the orbit space. Conversely every such function is invariant. Appropriate quotient measurability is understood. If the action is transitive on a null family of [probability distributions](probability-distribution.md), invariance also gives the same null law of $T$ under every member. Thus tests based on $T$ eliminate that null nuisance variation.

## Parametric statistical model

↑ **Parent:** [Statistical model](statistical-model.md)

A [statistical model](statistical-model.md) indexed by a parameter vector of fixed finite dimension is parametric. Examples include a [normal distribution](probability-distribution.md#normal-distribution) with unknown mean and variance and a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with unknown mean. Its [likelihood function](maximum-likelihood-estimation.md#likelihood-function) is the joint sample density or mass function, regarded as a function of the parameter at the observed sample.

## Location-scale family

↑ **Parent:** [Statistical model](statistical-model.md)

In a location-scale family, $Y=\mu+\sigma Z$ for a fixed base [probability distribution](probability-distribution.md) of $Z$, with $\mu\in\mathbb R$ and $\sigma>0$. Location translates observations, and scale multiplies their deviations. For an independent sample with a base density and at least two observations, the normalized residual vector $(Y_i-\bar Y)/s$, where $s^2=n^{-1}\sum_i(Y_i-\bar Y)^2$, is an [ancillary statistic](probability-and-statistics.md#ancillary-statistic). Indeed, $\bar Y=\mu+\sigma\bar Z$ and $s=\sigma s_Z$, making the residual vector a function of the base sample alone. This algebraic result needs no population moments.

### Log-transformed location-scale model

↑ **Parent:** [Location-scale family](#location-scale-family)

If $W$ has [probability density function](continuous-probability-distribution.md#probability-density-function) $f(w;q)$ and [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) $F_W(w;q)$, then $T=\exp(\alpha+\sigma W)$, $\sigma>0$, has density $f((\log t-\alpha)/\sigma;q)/(\sigma t)$ and distribution function $F_W((\log t-\alpha)/\sigma;q)$ for $t>0$. The factor $1/(\sigma t)$ follows from the [change-of-variables formula for a probability density](continuous-probability-distribution.md#change-of-variables-formula-for-a-probability-density). Upper truncation at $M$ divides the density by $F_W((\log M-\alpha)/\sigma;q)$.

### Conditional inference in a location-scale family

↑ **Parent:** [Location-scale family](#location-scale-family)

For normalized residuals $A_i=(Y_i-\bar Y)/s$, [Fisherian conditional inference](statistical-inference.md#fisherian-conditional-inference) uses the [conditional distribution](probability-theory.md#conditional-distribution) of $(\bar Y,s)$ given the observed $A=a$. For almost every attainable ancillary value, the joint conditional density of $\bar Y=m$ and $s=t>0$ is proportional to

$$
t^{n-2}\sigma^{-n}\prod_{i=1}^nf_0\!\left(\frac{m+ta_i-\mu}{\sigma}\right).
$$

The factor $t^{n-2}$ is the radial Jacobian on the $(n-1)$-dimensional centered residual space. After setting $u=(m-\mu)/\sigma$ and $v=t/\sigma$, the conditional density is proportional to $v^{n-2}\prod_i f_0(u+va_i)$, which is parameter-free. Conditioning on a continuous ancillary uses a [regular conditional distribution](probability-theory.md#regular-conditional-distribution), rather than division by the probability of a singleton ancillary value.

## Regression model

↑ **Parent:** [Statistical model](statistical-model.md)

A regression model specifies features of the [conditional distribution](probability-theory.md#conditional-distribution) of a response given predictor [covariates](#covariate), often a conditional mean or a full parametric density. [Linear regression](linear-regression.md) specifies a linear conditional mean; [logistic regression](generalized-linear-model.md#logistic-regression) specifies a logit-linear conditional probability for a binary response. The conditional comparison represented by a coefficient depends on which covariates are included.

### Interaction (statistics)

↑ **Parent:** [Regression model](#regression-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interaction_(statistics))

A statistical interaction means that the effect of one predictor depends on another on the chosen response scale. In a [linear regression](linear-regression.md), an [interaction term](#interaction-term) $\beta_3XZ$ changes the slope in $X$ to $\beta_1+\beta_3Z$. Whether interaction is present depends on the comparison scale; additive effects and multiplicative effects use different null contrasts. Comparing subgroup effects requires an [interaction contrast](normal-linear-model.md#interaction-contrast), rather than contrasting their separate significance labels.

#### Simple-effects analysis

↑ **Parent:** [Interaction (statistics)](#interaction-statistics)

Analysis of one factor's effect at a specified level of another factor, for example a cue-congruence difference separately at each delay. The [interaction](#interaction-statistics) compares those effects directly. One significant simple-effect test and one nonsignificant simple-effect test do not themselves establish an [interaction](#interaction-statistics); compare the estimates with the appropriate uncertainty and [multiple testing](statistical-hypothesis-test.md#multiple-hypothesis-testing) treatment.

#### Interaction plot

↑ **Parent:** [Interaction (statistics)](#interaction-statistics)

An interaction plot displays response means against levels of one factor, with separate lines for levels of another and optional panels for further factors. In an additive [linear regression](linear-regression.md), the difference between two lines is constant across the horizontal factor, so the population-mean lines are parallel. Changing line separations or crossings show a [statistical interaction](#interaction-statistics) on that response scale. Sample means may be nonparallel through noise, so the plot describes the effect pattern rather than replacing a formal [hypothesis test](statistical-hypothesis-test.md).

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

A two-factor interaction means that changing one factor has a different effect at different levels of another. For a two-level [factorial design](design-of-experiments.md#factorial-design), its sign column is $x_ix_j$, and four times its coefficient is the corresponding difference of differences. It can be confounded with other [factorial contrasts](design-of-experiments.md#factorial-contrast) in a [fractional factorial design](design-of-experiments.md#fractional-factorial-design).

##### Coupling constant (physics)

↑ **Parent:** [Interaction term](#interaction-term)

A coefficient multiplying an interaction term controls its strength relative to the chosen field normalization. Its [engineering dimension](critical-phenomenon.md#engineering-dimension) determines whether it is dimensionless, relevant or irrelevant. A renormalized [coupling constant](#coupling-constant-physics) constant is specified at a [renormalization scale](perturbative-quantum-field-theory.md#renormalization-scale); its change with that scale is described by the [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics).

##### Principle of marginality

↑ **Parent:** [Interaction term](#interaction-term)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principle_of_marginality)

A hierarchical [statistical model](statistical-model.md) that contains an [interaction term](#interaction-term) retains its associated lower-order effects. For two [categorical predictors](statistical-modelling.md#regression-factor) this means keeping both main effects when keeping their interaction. A nonsignificant averaged main effect may coexist with large opposite effects in different groups. Dropping its lower-order term while retaining the interaction can make the model depend on arbitrary factor coding.

## Statistical path

↑ **Parent:** [Statistical model](statistical-model.md)

A statistical path is a one-dimensional family of [probability measures](probability-space.md#probability-measure) inside a [statistical model](statistical-model.md), passing through a specified baseline $P$. A [differentiability in quadratic mean](#differentiability-in-quadratic-mean) condition gives its [score function](statistical-modelling.md#informant-function), the first-order direction of the family in square-root-density coordinates. The path must respect all restrictions of the [statistical model](statistical-model.md), including normalization and any fixed [moments](expected-value.md#moment).

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

Let $\delta_t=\sqrt{p_t}-\sqrt p=(t/2)g\sqrt p+r_t$, with $\|r_t\|_2=o(|t|)$. Since $p_t-p=2\sqrt p\,\delta_t+\delta_t^2$, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|p_t-p-tpg\|_1\leq2\|r_t\|_2+\|\delta_t\|_2^2=o(|t|)$. Thus [differentiability in quadratic mean](#differentiability-in-quadratic-mean) suffices to differentiate bounded density [integrals](integral.md), even when the density itself has no useful pointwise [derivative](calculus.md#derivative).

#### Mean-zero score identity under quadratic-mean differentiability

↑ **Parent:** [Differentiability in quadratic mean](#differentiability-in-quadratic-mean)

For a [differentiable-in-quadratic-mean path](#differentiability-in-quadratic-mean), normalization gives $\langle(\sqrt{p_t}-\sqrt p)/t,\sqrt{p_t}+\sqrt p\rangle=0$. The two factors converge in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) to $g\sqrt p/2$ and $2\sqrt p$. Continuity of the [inner product](inner-product.md) therefore gives $Pg=0$. This proves [score function](statistical-modelling.md#informant-function) centering without differentiating the density [integral](integral.md).

## Scale family

↑ **Parent:** [Statistical model](statistical-model.md)

A scale family rescales a fixed distribution by a positive parameter. The standardized variable $Y/\sigma$ has density $f$, independent of $\sigma$. This simplifies moments, simulations and the [Jeffreys prior for a scale parameter](statistical-modelling.md#jeffreys-prior-for-a-scale-parameter).

## Statistical parameter

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_parameter)

A [statistical parameter](#statistical-parameter) indexes a family of [probability distributions](probability-distribution.md) in a [statistical model](statistical-model.md). It is fixed in a frequentist sampling model; a [prior distribution](bayesian-statistics.md#prior-probability) makes it random for [Bayesian statistics](bayesian-statistics.md). Different [statistical parameter](#statistical-parameter) values should produce different observable distributions when [identifiability](#identifiability) is claimed.

### Nuisance parameter

↑ **Parent:** [Statistical parameter](#statistical-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nuisance_parameter)

A [nuisance parameter](#nuisance-parameter) is a [statistical parameter](#statistical-parameter) required to specify the distribution of observations but not itself the target of inference. A [profile likelihood](maximum-likelihood-estimation.md#profile-likelihood) maximizes over it; [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence) integrates over it using a proper [prior distribution](bayesian-statistics.md#prior-probability). These operations differ and need not give the same inference. A [baseline hazard](survival-analysis.md#baseline-hazard) in a [Cox proportional-hazards model](survival-analysis.md#cox-proportional-hazards-model) is an infinite-dimensional example.

#### Mixed log-likelihood derivative obstruction to parameter separation

↑ **Parent:** [Nuisance parameter](#nuisance-parameter)

On a common positive support, a factorization $f=\phi_0(x)\phi_C(x;\psi)\phi_S(x;\lambda)$ implies $\partial_\psi\partial_\lambda\log f=0$. Thus any nonzero mixed derivative prevents this exact separation. For $n$ independent [gamma distributed](continuous-probability-distribution.md#gamma-distribution) observations with shape $a$ and rate $b$, this mixed derivative is $n/b$, so exact separation of shape and rate into such factors is impossible.

## Covariate

↑ **Parent:** [Statistical model](statistical-model.md)

A covariate is an observed explanatory variable used to model the [conditional distribution](probability-theory.md#conditional-distribution) of a response. A vector of covariates can enter a [linear predictor](generalized-linear-model.md#linear-predictor), a treatment-effect adjustment or a [hazard multiplier](survival-analysis.md#hazard-multiplier). Conditioning on a covariate does not itself establish that its effect is causal.

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

In a [normal linear model](normal-linear-model.md) with an intercept and factor effects, set the effect of one factor level to zero. The intercept then denotes that reference level's mean, and the remaining effects are contrasts to it. The constraint removes redundant [statistical parameters](#statistical-parameter) without altering the fitted mean space.

## Location family

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Location_family)

A location family has distribution functions $F_\theta(x)=F_0(x-\theta)$, so changing the parameter translates the distribution without changing its shape.

### Location score

↑ **Parent:** [Location family](#location-family)

The location score is the [score function](statistical-modelling.md#informant-function) for translating a [probability density function](continuous-probability-distribution.md#probability-density-function) $f$. The minus sign comes from differentiating $f(y-\theta)$ in $\theta$. Under regular tail conditions, [integration by parts](calculus.md#integration-by-parts) gives $E_f\rho=0$ and $E_f(\varepsilon\rho)=1$. These identities determine projections of the [score function](statistical-modelling.md#informant-function) onto the span of the centered error.

### Single-observation location minimax bound

↑ **Parent:** [Location family](#location-family)

For a known mean-zero noise law with finite [variance](variance.md) $\sigma^2$, observing only $Y=a+\epsilon$ with unrestricted $a\in\mathbb R$ has [minimax risk](statistical-modelling.md#minimax-risk) $\sigma^2$ under [squared-error loss](statistical-inference.md#squared-error-loss). The observation itself attains this risk. For the lower bound, use a flat [prior distribution](bayesian-statistics.md#prior-probability) on $[-A,A]$ and condition an easier experiment on $|\epsilon|\leq M$. Away from the prior endpoints, the [Bayesian posterior](bayesian-statistics.md#bayesian-posterior) noise has its original truncated law. Let $A\to\infty$ and then $M\to\infty$ in the resulting [Bayes risk](statistical-inference.md#bayes-risk) lower bound. No [normal distribution](probability-distribution.md#normal-distribution) or density for the noise is required.

## Probabilistic graphical model

↑ **Parent:** [Statistical model](statistical-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_graphical_model)

A probabilistic graphical model represents factorization and conditional-independence structure using a graph whose vertices are random variables.

### Junction tree

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)

A junction tree connects the [maximal cliques](graph-theory.md#maximal-clique) of a [chordal graph](graph-theory.md#chordal-graph) into a [tree](tree-graph-theory.md) satisfying the [running intersection property](#running-intersection-property). Its edges carry separators equal to the intersections of the endpoint cliques. Assigning original factors to containing cliques permits exact [sum-product belief propagation](#sum-product-belief-propagation) without summing independently over the entire collection of variables.

#### Junction tree algorithm

↑ **Parent:** [Junction tree](#junction-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Junction_tree_algorithm)

The junction tree algorithm performs exact inference in a finite [probabilistic graphical model](#probabilistic-graphical-model). First moralize a [Bayesian network](#bayesian-network) if necessary; then apply [triangulation of an undirected graph](graph-theory.md#triangulation-of-an-undirected-graph), organize its [maximal cliques](graph-theory.md#maximal-clique) into a [junction tree](#junction-tree), and assign each original factor to one containing clique. Inward and outward [junction-tree sum-product messages](#junction-tree-sum-product-message) compute the [normalizing constant](continuous-probability-distribution.md#normalizing-constant) and [marginal distributions](probability-distribution.md#marginal-distribution). Its cost depends exponentially on the largest clique's number of variables, rather than necessarily on the total number of variables.

#### Junction-tree sum-product message

↑ **Parent:** [Junction tree](#junction-tree)

Assign each factor exactly once to a containing [clique](graph-theory.md#clique-graph-theory) and multiply the factors there into $\psi_i$. The displayed [sum-product belief propagation](#sum-product-belief-propagation) message sums out variables of $C_i$ outside the separator $S_{ij}=C_i\cap C_j$. By the [running intersection property](#running-intersection-property), eliminating all variables in the subtree on the $i$ side creates precisely this function of the separator. An inward pass computes the [normalizing constant](continuous-probability-distribution.md#normalizing-constant) at the root; an outward pass produces [marginal distributions](probability-distribution.md#marginal-distribution). For [pedigree likelihoods](genetics.md#pedigree-likelihood), observed genotypes and [penetrance](genetics.md#penetrance) factors simply multiply the relevant potentials.

#### Running intersection property

↑ **Parent:** [Junction tree](#junction-tree)

The running intersection property says that every variable belongs to a connected subtree of a [junction tree](#junction-tree). Equivalently, every clique along the path between two cliques contains their intersection. This ensures that eliminating variables on one side of a tree edge leaves a message depending only on its separator with the other side.

### Bayesian network

↑ **Parent:** [Probabilistic graphical model](#probabilistic-graphical-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayesian_network)

A Bayesian network consists of a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) $G$ whose nodes are [random variables](random-variable.md), together with [conditional distributions](probability-theory.md#conditional-distribution) satisfying $p(x)=\prod_jp(x_j\mid x_{\operatorname{pa}_G(j)})$. Its [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) encodes [conditional independence](random-variable.md#conditional-independence) constraints. For unrestricted binary variables it has $\sum_j2^{|\operatorname{pa}_G(j)|}$ free [conditional probabilities](probability-theory.md#conditional-probability). A [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) used this way need not have a causal interpretation.

#### Bayesian network structure score

↑ **Parent:** [Bayesian network](#bayesian-network)

For observations $\mathcal D$ and graph $G$, [Bayes' theorem](probability-theory.md#bayes-theorem) gives $p(G\mid\mathcal D)\propto\pi(G)\int p(\mathcal D\mid\theta_G,G)\pi(\theta_G\mid G)\,d\theta_G$. Here $\pi(G)$ is the graph [prior distribution](bayesian-statistics.md#prior-probability) and $\theta_G$ the local distribution [statistical parameters](#statistical-parameter). The integral is [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence); it averages over [nuisance parameters](#nuisance-parameter) with a proper [statistical parameter](#statistical-parameter) [prior distribution](bayesian-statistics.md#prior-probability). For [independent](random-variable.md#independent-random-variables) complete observations, the node-factorized [likelihood function](maximum-likelihood-estimation.md#likelihood-function) and [independence](random-variable.md#independent-random-variables) of local [statistical parameter](#statistical-parameter) [prior distributions](bayesian-statistics.md#prior-probability) make the evidence factor over nodes; suitable [conjugate priors](exponential-family.md#conjugate-prior) can make the local integrals analytic. With missing node observations, integrating out unobserved values can couple the local parameters, so [independence](random-variable.md#independent-random-variables) of local [prior distributions](bayesian-statistics.md#prior-probability) alone does not guarantee this factorization. Proper priors and coherent hyperparameters matter for comparing different graphs.

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

The max-product form of [belief propagation](#belief-propagation) replaces summation by maximization. On a tree, storing maximizing states while passing messages and then backtracking gives an exact [maximum a posteriori estimate](bayesian-statistics.md#maximum-a-posteriori-estimate).

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

On a graph, a binary configuration has probability proportional to $\exp(\alpha\sum_v x_v+\beta\sum_{\{v,w\}}x_vx_w)$, with each edge counted once. The full [conditional probability](probability-theory.md#conditional-probability) of a one is logistic with [linear predictor](generalized-linear-model.md#linear-predictor) $\alpha+\beta\sum_{w\sim v}x_w$. Local neighbor sums eliminate the need to evaluate the [normalizing constant](continuous-probability-distribution.md#normalizing-constant).

##### Gaussian-noise posterior for an autologistic image

↑ **Parent:** [Autologistic binary-image model](#autologistic-binary-image-model)

Independent unit-variance Gaussian observations with mean $x_v$ add $y_v-1/2$ to the local binary field. The [posterior distribution](bayesian-statistics.md#bayesian-posterior) [conditional probability](probability-theory.md#conditional-probability) is $\operatorname{logistic}(\alpha+\beta z_v+y_v-1/2)$. The neighbor interaction is unchanged, so checkerboard conditional independence and the same Gibbs schemes remain valid.

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

## ← Incoming links (62)

- [Ancillary statistic](probability-and-statistics.md#ancillary-statistic)
- [Bayes factor](bayesian-statistics.md#bayes-factor)
- [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence)
- [Bayesian posterior](bayesian-statistics.md#bayesian-posterior)
- [Bayesian statistics](bayesian-statistics.md)
- [Bernoulli sample sum as a sufficient statistic](probability-and-statistics.md#bernoulli-sample-sum-as-a-sufficient-statistic)
- [Box plot](probability-and-statistics.md#box-plot)
- [Capture-recapture model](statistical-modelling.md#capture-recapture-model)
- [Confidence interval](statistical-inference.md#confidence-interval)
- [Credible interval](bayesian-statistics.md#credible-interval)
- [Empirical distribution function](probability-distribution.md#empirical-distribution-function)
- [Expected frequency](probability-and-statistics.md#expected-frequency)
- [Finite contamination bias of normal location](robust-statistics.md#finite-contamination-bias-of-normal-location)
- [Fisher-Neyman factorization theorem](probability-and-statistics.md#fisher-neyman-factorization-theorem)
- [Huber score](robust-statistics.md#huber-score)
- [Kolmogorov-Smirnov statistic](statistical-inference.md#kolmogorov-smirnov-statistic)
- [Kolmogorov-Smirnov test](statistical-inference.md#kolmogorov-smirnov-test)
- [Kriging](statistical-modelling.md#kriging)
- [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence)
- [Laplace median robustness example](continuous-probability-distribution.md#laplace-median-robustness-example)
- [Linear regression model](linear-regression.md#linear-regression-model)
- [Maximum likelihood estimation](maximum-likelihood-estimation.md)
- [Mixed model](#mixed-model)
- [Mixture allocation indicator](statistical-modelling.md#mixture-allocation-indicator)
- [Nested measurements](design-of-experiments.md#nested-measurements)
- [Normal mean confidence interval and hypothesis test duality](statistical-inference.md#normal-mean-confidence-interval-and-hypothesis-test-duality)
- [Observed and latent mixture labels](statistical-modelling.md#observed-and-latent-mixture-labels)
- [Optimal experimental design](design-of-experiments.md#optimal-experimental-design)
- [Parameter space](#parameter-space)
- [Parametric statistical model](#parametric-statistical-model)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-2.md#section-i/1/solution)
- [Solution](past-exam-of-the-cognitive-neurology-course-of-the-university-of-oxford/2022.md#6/solution)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020.md#1/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#5/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#3/b/iii/solution)
- [Solution](past-exam-of-the-philosophy-of-science-supplementary-subject-of-the-university-of-oxford/2021.md#4/b/solution)
- [Principle of marginality](#principle-of-marginality)
- [Prior probability](bayesian-statistics.md#prior-probability)
- [Probability model](probability-theory.md#probability-model)
- [Regression factor](statistical-modelling.md#regression-factor)
- [Replication in experimental design](design-of-experiments.md#replication-in-experimental-design)
- [Responsibility curve for a two-Gaussian mixture](statistical-modelling.md#responsibility-curve-for-a-two-gaussian-mixture)
- [Sample mean sufficiency depends on the model](probability-and-statistics.md#sample-mean-sufficiency-depends-on-the-model)
- [Score factorization implies parameter orthogonality](statistical-modelling.md#score-factorization-implies-parameter-orthogonality)
- [Scoring rule](statistical-inference.md#scoring-rule)
- [Semi-log plot](calculus.md#semi-log-plot)
- [Statistical functional](statistical-inference.md#statistical-functional)
- [Statistical inference](statistical-inference.md)
- [Statistical modelling](statistical-modelling.md)
- [Statistical parameter](#statistical-parameter)
- [Statistical path](#statistical-path)
- [Statistical sample](statistical-inference.md#statistical-sample)
- [Strictly proper scoring rule](statistical-inference.md#strictly-proper-scoring-rule)
- [Sufficient statistic](probability-and-statistics.md#sufficient-statistic)
- [Uniform quantization error](electrical-engineering.md#uniform-quantization-error)
