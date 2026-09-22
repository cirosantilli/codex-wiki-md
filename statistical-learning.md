# Statistical learning

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Statistical_learning)

Statistical learning constructs predictive rules from data and studies their risk, generalization, and computational fitting.

**Table of contents**

- [Unsupervised learning](#unsupervised-learning)
  - [Multidimensional scaling](#multidimensional-scaling)
    - [Classical multidimensional scaling](#classical-multidimensional-scaling)
      - [Euclidean distance matrix criterion](#euclidean-distance-matrix-criterion)
  - [Sparse coding](#sparse-coding)
  - [Hebbian learning](#hebbian-learning)
    - [Quartic norm stabilization of Hebbian learning](#quartic-norm-stabilization-of-hebbian-learning)
    - [Oja's rule](#oja-s-rule)
      - [Stability and normalization of averaged Oja learning](#stability-and-normalization-of-averaged-oja-learning)
- [Cluster analysis](#cluster-analysis)
  - [Cluster in cluster analysis](#cluster-in-cluster-analysis)
  - [K-means clustering](#k-means-clustering)
  - [Jaccard index](#jaccard-index)
    - [Jaccard distance](#jaccard-distance)
  - [Dissimilarity matrix](#dissimilarity-matrix)
  - [Simple matching coefficient](#simple-matching-coefficient)
    - [Metric property of simple matching dissimilarity](#metric-property-of-simple-matching-dissimilarity)
  - [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)
    - [Ward minimum-variance clustering](#ward-minimum-variance-clustering)
    - [Average-linkage clustering](#average-linkage-clustering)
    - [Agglomerative clustering of nonmetric dissimilarities](#agglomerative-clustering-of-nonmetric-dissimilarities)
    - [Dendrogram](#dendrogram)
    - [Complete-linkage clustering](#complete-linkage-clustering)
    - [Single-linkage clustering](#single-linkage-clustering)
- [Validation set](#validation-set)
  - [Test set](#test-set)
- [Prediction error](#prediction-error)
  - [Test error](#test-error)
  - [Mean squared prediction error](#mean-squared-prediction-error)
- [Training error](#training-error)
  - [Prediction optimism](#prediction-optimism)
    - [Covariance formula for prediction optimism](#covariance-formula-for-prediction-optimism)
- [Data leakage](#data-leakage)
- [Dataset shift](#dataset-shift)
- [Regression function](#regression-function)
- [Principal component analysis](#principal-component-analysis)
  - [Principal component regression](#principal-component-regression)
  - [Scree plot](#scree-plot)
  - [Principal component loading](#principal-component-loading)
  - [Principal component](#principal-component)
    - [Principal component score](#principal-component-score)
  - [Explained variance of a principal component](#explained-variance-of-a-principal-component)
  - [Principal component analysis on a correlation matrix](#principal-component-analysis-on-a-correlation-matrix)
  - [Population principal component](#population-principal-component)
  - [Sample principal component](#sample-principal-component)
    - [Normalized sample principal component](#normalized-sample-principal-component)
- [Classification in statistical learning](#classification-in-statistical-learning)
  - [Misclassification rate](#misclassification-rate)
  - [Classification tree](#classification-tree)
    - [Cost-complexity tree pruning](#cost-complexity-tree-pruning)
    - [Classification-tree deviance](#classification-tree-deviance)
  - [Binary classification](#binary-classification)
    - [False positive rate](#false-positive-rate)
  - [Decision boundary](#decision-boundary)
    - [Bayes decision boundary](#bayes-decision-boundary)
  - [Majority vote](#majority-vote)
  - [Confusion matrix](#confusion-matrix)
  - [Classification and regression tree](#classification-and-regression-tree)
    - [Recursive partitioning](#recursive-partitioning)
      - [Surrogate split](#surrogate-split)
    - [Gini impurity](#gini-impurity)
    - [Random forest](#random-forest)
      - [Out-of-bag error](#out-of-bag-error)
  - [Conditional class probability](#conditional-class-probability)
  - [Risk consistency](#risk-consistency)
  - [K-nearest neighbors algorithm](#k-nearest-neighbors-algorithm)
    - [Bias and variance of a three-neighbour weighted smoother](#bias-and-variance-of-a-three-neighbour-weighted-smoother)
    - [One-nearest-neighbour classifier](#one-nearest-neighbour-classifier)
      - [One-nearest-neighbour asymptotic risk](#one-nearest-neighbour-asymptotic-risk)
        - [Bayes risk bound for one-nearest-neighbour classification](#bayes-risk-bound-for-one-nearest-neighbour-classification)
    - [Feature-measurable nearest-neighbour tie-breaking](#feature-measurable-nearest-neighbour-tie-breaking)
    - [L-nearest-neighbour classifier](#l-nearest-neighbour-classifier)
      - [One-nearest-neighbour classification](#one-nearest-neighbour-classification)
  - [Plug-in classifier excess-risk bound](#plug-in-classifier-excess-risk-bound)
  - [Support vector machine](#support-vector-machine)
    - [Kernel support vector machine](#kernel-support-vector-machine)
    - [Soft-margin support vector machine](#soft-margin-support-vector-machine)
      - [Kernel support-vector coefficient from hinge activity](#kernel-support-vector-coefficient-from-hinge-activity)
      - [Support-vector leave-one-out error bound](#support-vector-leave-one-out-error-bound)
      - [Dual support vectors and margin degeneracy](#dual-support-vectors-and-margin-degeneracy)
    - [Separating hyperplane](#separating-hyperplane)
    - [Slack variables of a support vector machine](#slack-variables-of-a-support-vector-machine)
    - [Support-vector-machine decision boundary](#support-vector-machine-decision-boundary)
    - [Support-vector-machine margin](#support-vector-machine-margin)
      - [Support-vector-machine margin boundaries](#support-vector-machine-margin-boundaries)
    - [Support vector](#support-vector)
  - [Perceptron](#perceptron)
- [Cross-validation](#cross-validation)
  - [Biased cross-validation for density bandwidth](#biased-cross-validation-for-density-bandwidth)
  - [Least-squares cross-validation for density bandwidth](#least-squares-cross-validation-for-density-bandwidth)
  - [Generalized cross-validation](#generalized-cross-validation)
  - [Leave-one-out cross-validation](#leave-one-out-cross-validation)
    - [Leave-one-out residual identity for a linear smoother](#leave-one-out-residual-identity-for-a-linear-smoother)
  - [K-fold cross-validation](#k-fold-cross-validation)
- [Neural network](#neural-network)
  - [Binary threshold unit](#binary-threshold-unit)
  - [Activation function](#activation-function)
  - [Hopfield network](#hopfield-network)
    - [Asynchronous Hopfield energy descent](#asynchronous-hopfield-energy-descent)
    - [Hebbian memory weights for a Hopfield network](#hebbian-memory-weights-for-a-hopfield-network)
  - [Feedforward neural network](#feedforward-neural-network)
    - [Four-input parity network](#four-input-parity-network)
    - [Hidden unit](#hidden-unit)
    - [Backpropagation](#backpropagation)
      - [Squared-error backpropagation](#squared-error-backpropagation)
      - [Sigmoid-softmax network gradients](#sigmoid-softmax-network-gradients)
  - [Sigmoid function](#sigmoid-function)
    - [Logistic function](#logistic-function)
  - [Rectified linear unit](#rectified-linear-unit)
  - [Gaussian error linear unit](#gaussian-error-linear-unit)
  - [Softmax function](#softmax-function)
    - [Softmax non-identifiability](#softmax-non-identifiability)
    - [Categorical cross-entropy loss](#categorical-cross-entropy-loss)
- [Overfitting](#overfitting)
- [Regularization](#regularization)
  - [Penalized least squares](#penalized-least-squares)
    - [Penalized least-squares estimator](#penalized-least-squares-estimator)
      - [Basic inequality for a penalized least-squares estimator](#basic-inequality-for-a-penalized-least-squares-estimator)
  - [Roughness penalty](#roughness-penalty)
  - [Early stopping](#early-stopping)

## Unsupervised learning

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unsupervised_learning)

Learning structure from data without supplied target labels. Examples include extracting [principal components](#principal-component), clustering and learning representations that efficiently reconstruct inputs.

### Multidimensional scaling

↑ **Parent:** [Unsupervised learning](#unsupervised-learning)

Construct low-dimensional coordinates representing a [dissimilarity matrix](#dissimilarity-matrix). Different methods preserve different features: [classical multidimensional scaling](#classical-multidimensional-scaling) approximates a centered [Gram matrix](linear-algebra.md#gram-matrix), while other methods minimize discrepancies between fitted and supplied distances or preserve distance ordering. The method and dimension determine what geometric claims the resulting display supports.

#### Classical multidimensional scaling

↑ **Parent:** [Multidimensional scaling](#multidimensional-scaling)

For a symmetric zero-diagonal [dissimilarity matrix](#dissimilarity-matrix) $D$, square each entry to obtain $D^{(2)}$ and put $H=I-\mathbf1\mathbf1^T/n$. Take the [eigenvectors](linear-operator-theory.md#eigenvector) of $G=-HD^{(2)}H/2$ corresponding to its largest positive [eigenvalues](linear-operator-theory.md#eigenvalue). Multiplying them by square roots of these [eigenvalues](linear-operator-theory.md#eigenvalue) gives coordinates. If $D$ contains [Euclidean distances](topological-analysis.md#euclidean-distance), $G$ is a centered [Gram matrix](linear-algebra.md#gram-matrix), so retaining all positive [eigenvalues](linear-operator-theory.md#eigenvalue) reconstructs those distances exactly. Retaining fewer approximates the [Gram matrix](linear-algebra.md#gram-matrix), not generally the sum of squared errors in raw distances. Negative [eigenvalues](linear-operator-theory.md#eigenvalue) signal failure of an exact Euclidean representation. Coordinates are unchanged in meaning by [orthogonal transformations](linear-algebra.md#orthogonal-transformation).

##### Euclidean distance matrix criterion

↑ **Parent:** [Classical multidimensional scaling](#classical-multidimensional-scaling)

For symmetric nonnegative $D$ with zero diagonal, a centered Euclidean realization implies $D_{ij}^2=G_{ii}+G_{jj}-2G_{ij}$ and hence the displayed double-centering identity. Conversely, if the double-centered matrix is [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix), factor it as $XX^T$. Its reconstructed squared distances equal the original squared distances: their difference has zero double-centering, so is of the form $\mathbf1 a^T+a\mathbf1^T$; the zero diagonal forces $a=0$. The minimum exact embedding dimension is $\operatorname{rank}G$.

### Sparse coding

↑ **Parent:** [Unsupervised learning](#unsupervised-learning)

Represent inputs accurately using few strongly active coefficients, for example by minimizing $\|x-Az\|^2/2+\lambda\sum_i|z_i|$. Learning basis functions on natural images can yield localized oriented filters resembling simple-cell receptive fields. This demonstrates one possible functional account of selectivity, not a proof that cortex implements that exact objective or learning algorithm.

### Hebbian learning

↑ **Parent:** [Unsupervised learning](#unsupervised-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hebbian_learning)

Activity-dependent strengthening associated with coactivation of an input and its postsynaptic output. The idealized update $\Delta w_i\propto yx_i$ requires normalization, competition or other constraints to prevent indefinite weight growth.

#### Quartic norm stabilization of Hebbian learning

↑ **Parent:** [Hebbian learning](#hebbian-learning)

With $y=w\cdot x$, the squared weight norm $s=|w|^2$ satisfies $\tau\dot s=2y^2(1-\alpha s^2)$. It moves monotonically toward $s_*=\alpha^{-1/2}$ without crossing it. Explicitly $(s-s_*)/(s+s_*)$ equals its initial value times $\exp[-(4\sqrt\alpha/\tau)\int_0^ty(u)^2\,du]$. Persistent excitation therefore drives $|w|$ to $\alpha^{-1/4}$; without excitation it can remain stationary. This nonlinear normalization avoids the unbounded amplification of unmodified [Hebbian learning](#hebbian-learning).

<h4 id="oja-s-rule">Oja's rule</h4>

↑ **Parent:** [Hebbian learning](#hebbian-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oja's_rule)

For a linear output $y=w^Tx$, the second term limits the growth produced by the Hebbian term. On the averaged dynamics with $C=\mathbb E[xx^T]$, $\tau\dot w=Cw-\alpha(w^TCw)w$. For $\alpha>0$, positive-eigenvalue equilibria have norm $1/\sqrt\alpha$ and align with eigenvectors of $C$. If inputs are centered, $C$ is their [covariance matrix](variance.md#covariance-matrix).

##### Stability and normalization of averaged Oja learning

↑ **Parent:** [Oja's rule](#oja-s-rule)

At the equilibrium $v_i/\sqrt\alpha$, linearization along orthonormal eigenvectors of $C$ gives the displayed rates, with the first equation applying to $j\ne i$. A simple positive largest eigenvalue makes its two normalized eigenvectors locally asymptotically stable; smaller eigenvalues have an unstable direction. Repeated largest eigenvalues give a manifold of equilibria with neutral directions. Generic convergence also needs a nonzero initial component in the largest eigenspace. The squared norm satisfies $\tau\,d\|w\|^2/dt=2(w^TCw)(1-\alpha\|w\|^2)$.

## Cluster analysis

↑ **Parent:** [Statistical learning](statistical-learning.md)

Cluster analysis groups observations using similarities or dissimilarities without supplied class labels. A distance choice specifies which features and scales matter. [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering) merges groups recursively, producing partitions at different resolutions rather than one intrinsically determined number of groups.

### Cluster in cluster analysis

↑ **Parent:** [Cluster analysis](#cluster-analysis)

A cluster in [cluster analysis](#cluster-analysis) is a nonempty group of observations treated as similar under the chosen representation and dissimilarity. A partition assigns each observation to exactly one cluster; [agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering) supplies a nested sequence of such partitions. An algorithmic cluster need not correspond to a distinct probabilistic population.

### K-means clustering

↑ **Parent:** [Cluster analysis](#cluster-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K-means_clustering)

For a prescribed number of groups, minimize within-cluster squared Euclidean distances. At fixed assignments, differentiating the objective gives the mean as the optimal centroid. At fixed centroids, assigning each point to a nearest centroid minimizes its contribution. Alternating these steps cannot increase the objective but can converge to a local optimum, so multiple starts are useful. Empty clusters and ties need an explicit handling rule. The method favors roughly spherical groups and depends on variable scaling.

### Jaccard index

↑ **Parent:** [Cluster analysis](#cluster-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jaccard_index)

The index measures similarity of finite sets by shared presence relative to total presence. For binary profiles it ignores joint absences, unlike the [simple matching coefficient](#simple-matching-coefficient). When both sets are empty, define the similarity to be one. The complementary [Jaccard distance](#jaccard-distance) measures dissimilarity.

#### Jaccard distance

↑ **Parent:** [Jaccard index](#jaccard-index)

The dissimilarity is the number of mismatched presences divided by the number of coordinates present in at least one profile. It differs from [normalized Hamming distance](coding-theory.md#normalized-hamming-distance) because coordinates absent from both profiles do not enter its denominator. Define the distance of two empty sets to be zero.

### Dissimilarity matrix

↑ **Parent:** [Cluster analysis](#cluster-analysis)

A dissimilarity matrix records pairwise separation of observations or profiles. Usually it is symmetric, nonnegative and zero on the diagonal. A [metric space](topological-analysis.md#metric-space) additionally requires the triangle inequality and separation of distinct profiles. [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering) can be applied to many dissimilarity matrices that are not Euclidean distance matrices; the claimed geometry must be checked separately.

### Simple matching coefficient

↑ **Parent:** [Cluster analysis](#cluster-analysis)

For binary vectors, this similarity counts agreements on both presences and absences. Its complement is the [normalized Hamming distance](coding-theory.md#normalized-hamming-distance). Whether joint absences should count as similarity depends on the application; rare-presence data may call for a different coefficient.

#### Metric property of simple matching dissimilarity

↑ **Parent:** [Simple matching coefficient](#simple-matching-coefficient)

The displayed distance is the [normalized Hamming distance](coding-theory.md#normalized-hamming-distance). Each coordinate mismatch between $x,z$ implies a mismatch between $x,y$ or $y,z$, so summing the indicator inequalities proves the triangle inequality. Nonnegativity, symmetry and separation follow immediately. It is a metric on profiles; on separately labelled individuals with identical profiles it is a [pseudometric](topological-analysis.md#pseudometric).

### Agglomerative hierarchical clustering

↑ **Parent:** [Cluster analysis](#cluster-analysis)

Start with singleton clusters and repeatedly merge the two clusters with the smallest chosen intercluster dissimilarity. [Single-linkage clustering](#single-linkage-clustering) uses the smallest cross-pair distance; [complete-linkage clustering](#complete-linkage-clustering) uses the largest. Merge heights and sensitivity to ties help assess a proposed number of groups.

#### Ward minimum-variance clustering

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)

Ward clustering merges the pair causing the smallest increase in within-cluster sum of squares. Expanding each cluster's squared deviations about the merged mean gives the displayed increase. Its Euclidean sum-of-squares interpretation must not be asserted for arbitrary non-Euclidean dissimilarities.

#### Average-linkage clustering

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)

Average linkage merges the pair with the smallest mean cross-pair dissimilarity. This differs from the minimum used by [single-linkage clustering](#single-linkage-clustering) and the maximum used by [complete-linkage clustering](#complete-linkage-clustering). The convention here weights individual cross-pairs equally; weighting already formed clusters equally is a different algorithm.

#### Agglomerative clustering of nonmetric dissimilarities

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)

The min and max cross-pair definitions of [single-linkage clustering](#single-linkage-clustering) and [complete-linkage clustering](#complete-linkage-clustering) remain meaningful for a symmetric nonnegative [dissimilarity matrix](#dissimilarity-matrix) that violates the triangle inequality. Such a calculation gives a valid algorithmic dendrogram, but does not turn the original matrix into Euclidean distances. A triangle-inequality counterexample identifies that source defect without requiring invented replacement data.

#### Dendrogram

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dendrogram)

A dendrogram displays successive cluster merges, with the height of each merge equal to its intercluster dissimilarity. Cutting at a height gives a partition. [Single-linkage clustering](#single-linkage-clustering) measures the closest cross-pair and can form chains, while [complete-linkage clustering](#complete-linkage-clustering) measures the farthest cross-pair and favors smaller within-cluster diameters.

#### Complete-linkage clustering

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)

The farthest cross-pair distance determines the next merge. It favors groups with small diameter and reduces the chaining effect of [single-linkage clustering](#single-linkage-clustering), but can be sensitive to isolated extreme observations. Ties can affect intermediate partitions.

#### Single-linkage clustering

↑ **Parent:** [Agglomerative hierarchical clustering](#agglomerative-hierarchical-clustering)

The nearest cross-pair distance determines the next merge. At a threshold, clusters are connected components of the graph joining pairs below that threshold. This handles nonconvex shapes but can join otherwise separate groups through a chain of intermediate observations.

## Validation set

↑ **Parent:** [Statistical learning](statistical-learning.md)

A validation set is held out from parameter fitting and used to choose models or tuning parameters. A separate test set is then needed for an unbiased final evaluation after selection.

### Test set

↑ **Parent:** [Validation set](#validation-set)

A test set is held out from both model fitting and model selection and is used once to estimate the final selected procedure's out-of-sample performance.

## Prediction error

↑ **Parent:** [Statistical learning](statistical-learning.md)

Prediction error is the expected loss of a fitted rule on a new observation from the target distribution.

### Test error

↑ **Parent:** [Prediction error](#prediction-error)

Test error is the average loss on an independent test set and estimates prediction error when the test set has not influenced model fitting or selection.

### Mean squared prediction error

↑ **Parent:** [Prediction error](#prediction-error)

For a predictor $\widehat f$ and an independent response $Y^*$ at covariate $X^*$, mean squared prediction error is $\mathbb E[(Y^*-\widehat f(X^*))^2]$.

## Training error

↑ **Parent:** [Statistical learning](statistical-learning.md)

Training error is the average loss evaluated on the same observations used to fit the prediction rule. Flexible fitting usually makes it optimistically biased for prediction error.

### Prediction optimism

↑ **Parent:** [Training error](#training-error)

Prediction optimism is the difference between expected squared prediction error on new independent responses at the training covariates and expected [training error](#training-error). Reusing responses to fit and assess a model tends to make training error too favorable. The [covariance formula for prediction optimism](#covariance-formula-for-prediction-optimism) measures this reuse without assuming a linear fitting rule.

// Target: probability-and-statistics.bigb

#### Covariance formula for prediction optimism

↑ **Parent:** [Prediction optimism](#prediction-optimism)

With fixed covariates and independent new responses having the same marginal distributions as the training responses, expanding squared losses cancels their second moments. Independence makes $\mathbb E(Y_i^{\mathrm{new}}\widehat Y_i)=\mathbb EY_i\mathbb E\widehat Y_i$, yielding the displayed identity. For a fixed [linear smoother](linear-regression.md#linear-smoother) $\widehat Y=HY$ with covariance $\sigma^2I$, it reduces to $2\sigma^2\operatorname{tr}(H)/n$, linking prediction optimism to [effective degrees of freedom](linear-regression.md#effective-degrees-of-freedom).

// Target: analysis.bigb

## Data leakage

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_leakage)

Data leakage occurs when information unavailable at prediction time, including information from nominally held-out observations, influences model fitting or selection. It makes estimated out-of-sample performance optimistically biased.

## Dataset shift

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dataset_shift)

Dataset shift means that the joint distribution of predictors and responses differs between training and deployment data.

## Regression function

↑ **Parent:** [Statistical learning](statistical-learning.md)

A regression function is a conditional expected response. For binary labels it equals the conditional probability of class one.

## Principal component analysis

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_component_analysis)

Principal component analysis finds orthogonal directions of greatest sample variance. Its first loading vector is a unit eigenvector corresponding to the largest eigenvalue of the sample covariance matrix.

### Principal component regression

↑ **Parent:** [Principal component analysis](#principal-component-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_component_regression)

Regress a response on selected [principal component scores](#principal-component-score) of centered predictors. If $X=UDV^T$ is a [singular value decomposition](linear-algebra.md#singular-value-decomposition) and the first $q$ positive-singular-value components are retained, the retained score matrix is $U_qD_q$ and the fitted coefficient in predictor coordinates is $V_qD_q^{-1}U_q^Ty$. The fitted centered response is $U_qU_q^Ty$: this follows by applying the [least-squares normal equations](linear-regression.md#normal-equations-for-linear-least-squares) to the orthogonal score columns. Truncating small singular directions limits variance amplification, but directions of large predictor variance need not be those best predicting the response; select $q$ using prediction assessment rather than explained predictor variance alone.

### Scree plot

↑ **Parent:** [Principal component analysis](#principal-component-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scree_plot)

A scree plot graphs ordered covariance or correlation [eigenvalues](linear-operator-theory.md#eigenvalue) against component number. A transition from a steep decline to a flatter tail suggests a dimension, but this is a diagnostic rather than a proof of the number of latent factors. In [factor analysis](statistical-modelling.md#factor-analysis), it should be combined with model fit, substantive interpretation and uncertainty assessment.

### Principal component loading

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

Two conventions occur for principal-component loadings: the unit [eigenvector](linear-operator-theory.md#eigenvector) $\ell_j$ defining a [principal component](#principal-component), and the scaled vector $r_j=\sqrt{\lambda_j}\ell_j$. For [principal component analysis on a correlation matrix](#principal-component-analysis-on-a-correlation-matrix), the entries of the latter are the correlations between each standardized variable and the component scaled to variance one. Indeed, $\operatorname{Cov}(Z,\ell_j^TZ)=C\ell_j=\lambda_j\ell_j$ and $\operatorname{Var}(\ell_j^TZ)=\lambda_j$. Thus $\|r_j\|^2=\lambda_j$, whereas $\|\ell_j\|=1$; reporting the convention avoids confusing component directions with correlations.

### Principal component

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

A principal component is the projection of centered data onto a unit [eigenvector](linear-operator-theory.md#eigenvector) of its [covariance matrix](variance.md#covariance-matrix). Ordering the components by their [eigenvalues](linear-operator-theory.md#eigenvalue) orders their variances. Repeated [eigenvalues](linear-operator-theory.md#eigenvalue) allow any [orthonormal basis](linear-algebra.md#orthonormal-basis) of the corresponding [eigenspace](linear-operator-theory.md#eigenspace).

#### Principal component score

↑ **Parent:** [Principal component](#principal-component)

A score is an observation's coordinate along a [principal component](#principal-component) direction. Center an observation by the fitted [sample mean](variance.md#sample-mean), apply the fitted variable scaling when using [principal component analysis on a correlation matrix](#principal-component-analysis-on-a-correlation-matrix), then take its [inner product](linear-algebra.md#inner-product) with the unit [principal component loading](#principal-component-loading) vector. New observations must use the training center and scaling. The score [variance](variance.md) equals the corresponding [eigenvalue](linear-operator-theory.md#eigenvalue) when the covariance normalization is consistent.

### Explained variance of a principal component

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

A [population principal component](#population-principal-component) explains the displayed fraction of total [variance](variance.md). The first $q$ components explain $\sum_{j\le q}\lambda_j/\sum_j\lambda_j$. Comparing covariance and correlation analyses requires different denominators: the original [variance](variance.md) sum for the former and the number of nonconstant standardized variables for the latter.

### Principal component analysis on a correlation matrix

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

For positive marginal [variances](variance.md), standardizing each variable to [variance](variance.md) one converts covariance-based [PCA](#principal-component-analysis) on $Z$ into correlation-based PCA on $X$. This makes the analysis insensitive to the original measurement units but changes the optimization criterion. Standardization gives small-variance variables the same marginal weight as large-variance variables; it is a modelling choice, not an automatic improvement.

### Population principal component

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

The [population principal components](#population-principal-component) are centered linear compounds along an orthonormal eigenbasis of the [covariance matrix](variance.md#covariance-matrix), ordered by decreasing [eigenvalue](linear-operator-theory.md#eigenvalue). They are uncorrelated and have [variances](variance.md) $\lambda_j$. Each successive direction maximizes [variance](variance.md) subject to unit length and orthogonality to earlier directions. Uncorrelatedness does not imply [independence](random-variable.md#independent-random-variables) unless additional distributional assumptions hold.

### Sample principal component

↑ **Parent:** [Principal component analysis](#principal-component-analysis)

Let the columns of a centered [design matrix](linear-regression.md#design-matrix) $X\in\mathbb R^{n\times p}$ be variables and write $X^TX=V\Lambda V^T$ by the [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices). The columns $u_i$ of $U=XV$ are the sample principal-component score vectors. They satisfy $u_i^Tu_j=\Lambda_{ij}$, so distinct score vectors have zero [sample covariance](variance.md#sample-covariance) and $u_i$ has [sample variance](statistical-inference.md#sample-variance) $\Lambda_{ii}/n$ under the divisor-$n$ convention.

#### Normalized sample principal component

↑ **Parent:** [Sample principal component](#sample-principal-component)

When $\Lambda_{ii}>0$, the normalized sample principal component $w_i=u_i/\sqrt{\Lambda_{ii}}$ has [Euclidean norm](functional-analysis.md#euclidean-norm) one. The vectors $w_i$ form an [orthonormal set](linear-algebra.md#orthonormal-set) spanning the [column space](vector-space.md#column-space) of a full-column-rank centered design matrix.

## Classification in statistical learning

↑ **Parent:** [Statistical learning](statistical-learning.md)

Classification predicts a discrete label from observed covariates.

### Misclassification rate

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

The misclassification rate is the expected [zero-one loss](foundations-of-mathematics.md#misclassification-loss) of a [classification in statistical learning](#classification-in-statistical-learning) rule. Its empirical version is the fraction of incorrectly labeled observations. Evaluation on the fitting sample gives a [training error](#training-error); evaluation on an independent [test set](#test-set) estimates [prediction error](#prediction-error). For a majority-class leaf of a [classification tree](#classification-tree), the training error count is $n_t-\max_kn_{tk}$, unlike [classification-tree deviance](#classification-tree-deviance), which also uses the fitted class [probabilities](probability-theory.md#probability).

### Classification tree

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

A classification tree partitions predictor space recursively and attaches a class probability vector to each terminal region. For a categorical response, a fitted leaf commonly uses its observed class proportions and predicts their largest entry. Binary numerical splits compare one coordinate with a threshold. Growing a tree greedily by reducing [classification-tree deviance](#classification-tree-deviance) gives an interpretable rule but does not globally optimize the tree. [Cost-complexity tree pruning](#cost-complexity-tree-pruning) and [cross-validation](#cross-validation) control complexity and assess [prediction error](#prediction-error).

#### Cost-complexity tree pruning

↑ **Parent:** [Classification tree](#classification-tree)

Pruning balances a tree's empirical loss $R(T)$ against the number of leaves. Increasing $\alpha$ favors a nested sequence of smaller subtrees, obtained by removing splits with the smallest effective cost per removed leaf. Choose complexity using [cross-validation](#cross-validation) or a [validation set](#validation-set), and assess the selected tree on a separate [test set](#test-set). The loss can be deviance or misclassification loss; the chosen convention must be specified.

#### Classification-tree deviance

↑ **Parent:** [Classification tree](#classification-tree)

Maximizing a node's multinomial likelihood gives class probabilities $\widehat p_{tk}=n_{tk}/n_t$. Twice the negative maximized log-likelihood relative to perfect classification is the displayed deviance, with $0\log0=0$. It equals twice the node size times its [Shannon entropy](information-theory.md#information-entropy). A split is chosen by maximizing $D(t)-D(t_L)-D(t_R)$, and tree deviance is the sum over terminal nodes. The training misclassification count is instead $\sum_t(n_t-\max_kn_{tk})$; the two criteria are different.

### Binary classification

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_classification)

[Classification in statistical learning](#classification-in-statistical-learning) with two possible labels. Given the [conditional probability](probability-theory.md#conditional-probability) $\eta(x)=\mathbb P(Y=1\mid X=x)$, a [Bayes classifier](statistical-inference.md#bayes-classifier) under [zero-one loss](foundations-of-mathematics.md#misclassification-loss) predicts one exactly when $\eta(x)\geq1/2$, with arbitrary decisions at ties.

#### False positive rate

↑ **Parent:** [Binary classification](#binary-classification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/False_positive_rate)

The [false positive rate](#false-positive-rate) is $\mathbb P(\text{positive result}\mid\text{truly negative class})$. In screening, it measures erroneous positives among genuinely disease-free individuals.

### Decision boundary

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_boundary)

A decision boundary is the subset of covariate space across which a classifier changes its predicted class.

#### Bayes decision boundary

↑ **Parent:** [Decision boundary](#decision-boundary)

For binary classification under zero-one loss, the Bayes decision boundary is the set on which the two conditional class probabilities are equal.

### Majority vote

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

A majority-vote ensemble predicts the class selected by more constituent classifiers than any other class.

### Confusion matrix

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Confusion_matrix)

A confusion matrix cross-tabulates true classes against predicted classes. Its diagonal entries count correct predictions and its off-diagonal entries describe the kinds of classification errors.

### Classification and regression tree

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

A classification and regression tree recursively splits covariate space into axis-aligned regions and assigns a constant prediction to each terminal region.

#### Recursive partitioning

↑ **Parent:** [Classification and regression tree](#classification-and-regression-tree)

Recursive partitioning repeatedly selects a split of one current region, then applies the same splitting rule independently to the resulting child regions.

##### Surrogate split

↑ **Parent:** [Recursive partitioning](#recursive-partitioning)

A surrogate split uses another predictor to approximate the left-versus-right assignments made by a tree node's primary split. It can route observations whose primary predictor is missing. Surrogates are ranked by agreement with the primary split on observations where both predictors are known, accounting for trivial majority assignments. This differs from simply filling a missing predictor with its [sample mean](variance.md#sample-mean).

#### Gini impurity

↑ **Parent:** [Classification and regression tree](#classification-and-regression-tree)

For class proportions $p_1,\ldots,p_K$ in a tree node, Gini impurity is $1-\sum_kp_k^2$. For two classes it is twice $p(1-p)$; omitting the constant factor does not change the selected split.

#### Random forest

↑ **Parent:** [Classification and regression tree](#classification-and-regression-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_forest)

A random forest aggregates deeply grown decision trees fitted to bootstrap samples, while restricting each split to a random subset of predictor coordinates. Classification uses a majority vote over the trees.

##### Out-of-bag error

↑ **Parent:** [Random forest](#random-forest)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Out-of-bag_error)

The out-of-bag error predicts each training observation using only trees whose bootstrap samples omitted it, then averages the resulting losses.

### Conditional class probability

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

The conditional class probability for class $k$ is

$$
p_k(x)=\mathbb P(Y=k\mid X=x).
$$

A [Bayes classifier](statistical-inference.md#bayes-classifier) selects a class maximizing this probability.

### Risk consistency

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

A sequence of classifiers $h_n$ is risk-consistent when its classification risk converges to the [Bayes risk](statistical-inference.md#bayes-risk) as the training sample size tends to infinity.

### K-nearest neighbors algorithm

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)

The K-nearest neighbors algorithm predicts from the labels or responses of the $K$ training observations closest to the query under a chosen distance.

#### Bias and variance of a three-neighbour weighted smoother

↑ **Parent:** [K-nearest neighbors algorithm](#k-nearest-neighbors-algorithm)

With fixed neighbor positions, independent equal-variance errors and weights $w,(1-w)/2,(1-w)/2$, the displayed [variance](variance.md) is minimized at $w=1/3$, with value $\sigma^2/3$. Its [bias](statistical-modelling.md#bias-of-an-estimator) is $w m_1+(1-w)(m_2+m_3)/2-m(x)$. Larger nearest-point weight often reduces smoothing bias, but neither the bias nor the variance is universally monotone over $0<w<1$. If the nearest point is the target, the squared bias is $(1-w)^2[(m_2+m_3)/2-m(x)]^2$.

// Target: probability-and-statistics.bigb

#### One-nearest-neighbour classifier

↑ **Parent:** [K-nearest neighbors algorithm](#k-nearest-neighbors-algorithm)

The [classifier](foundations-of-mathematics.md#classifier) that assigns the query the label of its closest training feature, using [feature-measurable nearest-neighbour tie-breaking](#feature-measurable-nearest-neighbour-tie-breaking). Its [misclassification risk](foundations-of-mathematics.md#misclassification-risk) need not converge to [Bayes risk](statistical-inference.md#bayes-risk), even with infinitely many [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) as [training data](foundations-of-mathematics.md#training-data).

##### One-nearest-neighbour asymptotic risk

↑ **Parent:** [One-nearest-neighbour classifier](#one-nearest-neighbour-classifier)

For [binary classification](#binary-classification), write $\eta(x)=\mathbb P(Y=1\mid X=x)$ and assume [feature-measurable nearest-neighbour tie-breaking](#feature-measurable-nearest-neighbour-tie-breaking). If $\mathbb E|\eta(X_{(1)}(X))-\eta(X)|\to0$, then the expected [conditional misclassification risk](foundations-of-mathematics.md#conditional-misclassification-risk) of the [one-nearest-neighbour classifier](#one-nearest-neighbour-classifier) tends to $\mathbb E[2\eta(X)(1-\eta(X))]$. Couple each label and an oracle label using one uniform variable. Their disagreement has the preceding expected absolute difference. The oracle and the test label are conditionally [independent](random-variable.md#independent-random-variables) [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) of parameter $\eta(X)$, so their disagreement [probability](probability-theory.md#probability) is exactly $2\eta(X)(1-\eta(X))$. The difference of [classification in statistical learning](#classification-in-statistical-learning) error probabilities is at most the coupling disagreement.

###### Bayes risk bound for one-nearest-neighbour classification

↑ **Parent:** [One-nearest-neighbour asymptotic risk](#one-nearest-neighbour-asymptotic-risk)

Under the hypotheses for the [one-nearest-neighbour asymptotic risk](#one-nearest-neighbour-asymptotic-risk), the limiting risk satisfies $R^*\leq R_\infty\leq2R^*$. Put $a=\min(\eta,1-\eta)$: then $a\leq2a(1-a)\leq2a$ since $0\leq a\leq1/2$. Integrate, using the definition of [Bayes risk](statistical-inference.md#bayes-risk). Constant $\eta=1/4$ gives limiting risk $3/8$ and [Bayes risk](statistical-inference.md#bayes-risk) $1/4$, so the lower comparison is not generally equality.

#### Feature-measurable nearest-neighbour tie-breaking

↑ **Parent:** [K-nearest neighbors algorithm](#k-nearest-neighbors-algorithm)

For a fixed query, order training features by their distances and break equal distances by a rule depending only on features, such as original index. If auxiliary uniforms are [independent](random-variable.md#independent-random-variables) of the features, the uniform selected by the resulting index remains uniform conditional on all features: sum over the possible selected indices. Label-dependent tie-breaking can invalidate [Bernoulli coupling by a shared uniform random variable](probability-and-statistics.md#bernoulli-coupling-by-a-shared-uniform-random-variable) and the usual [one-nearest-neighbour asymptotic risk](#one-nearest-neighbour-asymptotic-risk).

#### L-nearest-neighbour classifier

↑ **Parent:** [K-nearest neighbors algorithm](#k-nearest-neighbors-algorithm)

The L-nearest-neighbour classifier estimates each class probability by its empirical frequency among the $L$ nearest training covariates and predicts a class of greatest estimated probability.

##### One-nearest-neighbour classification

↑ **Parent:** [L-nearest-neighbour classifier](#l-nearest-neighbour-classifier)

One-nearest-neighbour classification assigns a query the label of its single nearest training observation. Under local regularity, its limiting conditional error is $1-\sum_kp_k(x)^2$.

### Plug-in classifier excess-risk bound

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)

For binary classification with posterior estimate $\widehat p_1$, the plug-in classifier satisfies

$$
R(\widehat C)-R(C^*)\leq2\mathbb E|\widehat p_1(X)-p_1(X)|.
$$

### Support vector machine

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Support_vector_machine)

A support vector machine chooses a separating decision function by trading a wide geometric margin against hinge-loss violations.

#### Kernel support vector machine

↑ **Parent:** [Support vector machine](#support-vector-machine)

A kernel support vector machine trains a [support vector machine](#support-vector-machine) using a [positive-definite kernel](probability-and-statistics.md#positive-semidefinite-kernel) instead of explicit feature coordinates. The [kernel trick](probability-and-statistics.md#kernel-trick) evaluates all required feature inner products through the training [Gram matrix](linear-algebra.md#gram-matrix); prediction is $\sum_i\alpha_i y_i k(x_i,x)+b$. Nonzero dual coefficients identify [support vectors](#support-vector). An unpenalized intercept supplies the dual equality $\sum_i\alpha_i y_i=0$. The [Reproducing kernel Hilbert space](probability-and-statistics.md#reproducing-kernel-hilbert-space) construction explains why a positive-semidefinite kernel defines valid feature geometry.

#### Soft-margin support vector machine

↑ **Parent:** [Support vector machine](#support-vector-machine)

For signed training labels, a linear soft-margin [support vector machine](#support-vector-machine) minimizes

$$
\frac12\lVert w\rVert^2+C\sum_i\xi_i,\qquad y_i(w^Tx_i+b)\geq1-\xi_i,\quad\xi_i\geq0,
$$

with $C>0$. Its [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) give $w=\sum_i\alpha_i y_ix_i$, $\sum_i\alpha_i y_i=0$, and $0\leq\alpha_i\leq C$.

##### Kernel support-vector coefficient from hinge activity

↑ **Parent:** [Soft-margin support vector machine](#soft-margin-support-vector-machine)

For the kernel [support vector machine](#support-vector-machine) objective $n^{-1}\sum_i(1-Y_i(\mu+K_i^T\alpha))_++\lambda\alpha^TK\alpha$, assume $Y_i\in\{-1,1\}$, $\lambda>0$, and that the [kernel matrix](probability-and-statistics.md#kernel-matrix) $K$ is invertible. The [subdifferential](convex-optimization.md#subdifferential) optimality equation gives

$$
\alpha_i=Y_it_i/(2n\lambda),\qquad t_i=\begin{cases}1&Y_i(\mu+K_i^T\alpha)<1,\\{}[0,1]&Y_i(\mu+K_i^T\alpha)=1,\\0&Y_i(\mu+K_i^T\alpha)>1.\end{cases}
$$

Thus strict margins greater than one force zero coefficients, while misclassified observations have nonzero coefficients. Invertibility matters: a singular [kernel matrix](probability-and-statistics.md#kernel-matrix) allows coefficient changes in its [null space](linear-algebra.md#kernel-of-a-linear-map) without changing the fitted [function](function.md) or objective.

##### Support-vector leave-one-out error bound

↑ **Parent:** [Soft-margin support vector machine](#soft-margin-support-vector-machine)

For a fixed $C$ in the unnormalized sum-of-slacks objective and unique training optimizers, deleting an observation with $\alpha_i=0$ preserves the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) and the fitted decision function. It is correctly classified when held out. Consequently [Leave-one-out cross-validation](#leave-one-out-cross-validation) makes at most $s$ errors, where $s$ counts positive dual coefficients. With geometric support vectors, counting all points of signed margin at most one also gives the bound, without a nondegeneracy assumption.

##### Dual support vectors and margin degeneracy

↑ **Parent:** [Soft-margin support vector machine](#soft-margin-support-vector-machine)

A dual [support vector](#support-vector) has $\alpha_i>0$. Every such point has signed margin at most one, but a point exactly on the margin can have $\alpha_i=0$ in a degenerate solution. If $\alpha_i=0$, complementary slackness forces $\xi_i=0$, so the point is correctly classified with margin at least one.

#### Separating hyperplane

↑ **Parent:** [Support vector machine](#support-vector-machine)

For signed observations $(x_i,y_i)$, an affine hyperplane with score $f(x)=\alpha+x^T\beta$ is separating when $y_if(x_i)>0$ for every observation.

#### Slack variables of a support vector machine

↑ **Parent:** [Support vector machine](#support-vector-machine)

The slack variables satisfy $\xi_i\geq\max\{0,1-y_if(x_i)\}$ and quantify margin violations.

#### Support-vector-machine decision boundary

↑ **Parent:** [Support vector machine](#support-vector-machine)

For a linear score $f(x)=\alpha+x^T\beta$, the decision boundary is $f(x)=0$.

#### Support-vector-machine margin

↑ **Parent:** [Support vector machine](#support-vector-machine)

For a linear support vector machine, the geometric margin lies between $f(x)=-1$ and $f(x)=1$ and has width $2/\lVert\beta\rVert$.

##### Support-vector-machine margin boundaries

↑ **Parent:** [Support-vector-machine margin](#support-vector-machine-margin)

The two margin boundaries of a linear support vector machine are the parallel hyperplanes $f(x)=1$ and $f(x)=-1$.

#### Support vector

↑ **Parent:** [Support vector machine](#support-vector-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Support_vector)

A support vector is a training observation on or inside the fitted margin; it has a nonzero dual coefficient and can affect the fitted boundary.

### Perceptron

↑ **Parent:** [Classification in statistical learning](#classification-in-statistical-learning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perceptron)

The perceptron is an online linear classifier that adds a misclassified observation's signed feature vector to its current parameter vector.

## Cross-validation

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-validation)

Cross-validation estimates predictive performance by repeatedly fitting on one part of the data and evaluating on held-out observations.

### Biased cross-validation for density bandwidth

↑ **Parent:** [Cross-validation](#cross-validation)

Subtract the diagonal variance contribution from the derivative estimate's squared norm, then insert the result into [asymptotic mean integrated squared error](statistical-modelling.md#asymptotic-mean-integrated-squared-error). The expected curvature estimate equals $R(f'')+O(h^2)$, apart from a negligible finite-n term. This makes the resulting criterion asymptotically correct even though it is not an exactly unbiased estimate of integrated risk. Under standard conditions its selector is ratio-consistent with the optimal bandwidth and has relative fluctuation order $n^{-1/10}$.

### Least-squares cross-validation for density bandwidth

↑ **Parent:** [Cross-validation](#cross-validation)

Minimize the displayed criterion using a [Leave-one-out cross-validation](#leave-one-out-cross-validation) estimate in the second term. Its expectation is the exact [mean integrated squared error](statistical-modelling.md#integrated-mean-squared-error) minus $R(f)$, which does not depend on h. With standard smoothness and appropriate search ranges, the chosen bandwidth is asymptotically optimal. Its relative fluctuations are ordinarily of order $n^{-1/10}$, considerably larger than the estimation error achievable by well-chosen plug-in pilots.

### Generalized cross-validation

↑ **Parent:** [Cross-validation](#cross-validation)

For a fixed [linear smoother](linear-regression.md#linear-smoother), generalized cross-validation replaces the individual leverage corrections of [Leave-one-out cross-validation](#leave-one-out-cross-validation) by their average. It selects smoothing parameters by minimizing the displayed criterion. It approximates a predictive error criterion; it is not a universal exact estimate of future error and requires care when observation errors are dependent.

### Leave-one-out cross-validation

↑ **Parent:** [Cross-validation](#cross-validation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leave-one-out_cross-validation)

Leave-one-out cross-validation performs one fit with each observation held out in turn and averages the held-out losses.

#### Leave-one-out residual identity for a linear smoother

↑ **Parent:** [Leave-one-out cross-validation](#leave-one-out-cross-validation)

If a linear smoother has fitted vector $\widehat Y=HY$, its residual after fitting without observation $i$ is

$$
Y_i-\widehat Y_{-i,i}=\frac{Y_i-\widehat Y_i}{1-H_{ii}}.
$$

The identity follows from a [block matrix inverse](linear-algebra.md#block-matrix-inverse) or a rank-one inverse update.

### K-fold cross-validation

↑ **Parent:** [Cross-validation](#cross-validation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K-fold_cross-validation)

K-fold cross-validation partitions observations into $K$ folds, trains $K$ times while holding out one fold at a time, and combines the held-out losses.

## Neural network

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neural_network)

A neural network composes affine maps with nonlinear activation functions and learns their weights from data.

### Binary threshold unit

↑ **Parent:** [Neural network](#neural-network)

A [binary threshold unit](#binary-threshold-unit) outputs one when its weighted input reaches its threshold and zero otherwise. Its hard threshold is not differentiable, so ordinary [backpropagation](#backpropagation) cannot directly train the exact threshold model. Smooth [activation functions](#activation-function) can approximate its computation.

### Activation function

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Activation_function)

An [activation function](#activation-function) converts a unit's weighted input to its output. A [sigmoid function](#sigmoid-function), hyperbolic tangent or rectifier can give nonlinear features. Replacing all hidden [activation functions](#activation-function) by the identity collapses consecutive affine layers into a single affine map, removing the representational benefit of those hidden layers.

### Hopfield network

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopfield_network)

A recurrent network with symmetric interactions and an energy function. In the binary version, units take values $\pm1$, self-couplings are zero, and asynchronous threshold updates can retrieve stored patterns from incomplete or corrupted cues. Fixed points are local energy minima, which need not be the intended memories or global minima.

#### Asynchronous Hopfield energy descent

↑ **Parent:** [Hopfield network](#hopfield-network)

For symmetric zero-diagonal weights and zero thresholds, update one binary unit to the sign of its current field, retaining it at a zero field. The displayed energy change is negative on every actual flip. There are finitely many states, so a fair asynchronous update schedule eventually reaches a fixed point that is a minimum against single-unit flips. Synchronous updates can instead cycle, and local minima need not be global minima.

#### Hebbian memory weights for a Hopfield network

↑ **Parent:** [Hopfield network](#hopfield-network)

For $M$ binary units and desired patterns $\xi^\mu$, use these symmetric weights and set $w_{ii}=0$. For one pattern, the field at that pattern is $(M-1)\xi_i/M$, so it is stable. Several patterns add cross-talk terms; storage by this rule alone does not guarantee stability of every arbitrary collection of patterns.

### Feedforward neural network

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feedforward_neural_network)

A feedforward neural network composes layers without directed cycles, passing each layer's activations only to later layers.

#### Four-input parity network

↑ **Parent:** [Feedforward neural network](#feedforward-neural-network)

Let $S$ be the number of active inputs. Four [hidden units](#hidden-unit) $h_m=H(S-m+1/2)$, $m=1,2,3,4$, detect successively larger counts. A [binary threshold unit](#binary-threshold-unit) with weights $(1,-1,1,-1)$ on these features and threshold $1/2$ returns one precisely for $S=1,3$. Each hidden input weight is one. This computes parity with a single hidden layer, but representability does not guarantee easy learning by [backpropagation](#backpropagation).

#### Hidden unit

↑ **Parent:** [Feedforward neural network](#feedforward-neural-network)

A [hidden unit](#hidden-unit) transforms input information before the final output rather than directly representing a supplied target. Nonlinear hidden features can make a classification linearly separable in feature space even when it is not separable in the original input coordinates.

#### Backpropagation

↑ **Parent:** [Feedforward neural network](#feedforward-neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backpropagation)

Backpropagation applies the [chain rule](calculus.md#chain-rule) from a neural network's output toward its input to compute the gradient of a loss with respect to every parameter.

##### Squared-error backpropagation

↑ **Parent:** [Backpropagation](#backpropagation)

For squared loss $E=\sum_k(t_k-z_k)^2/2$, let $e_k=(t_k-z_k)g_k'(x_k)$ and $e_j=g_j'(x_j)\sum_kw_{jk}e_k$. The [chain rule](calculus.md#chain-rule) gives $\partial E/\partial w_{jk}=-e_kz_j$ and $\partial E/\partial w_{ij}=-e_jz_i$. A [gradient descent](numerical-analysis.md#gradient-descent) step of size $\eta$ uses $\Delta w_{jk}=\eta e_kz_j$ and $\Delta w_{ij}=\eta e_jz_i$, with every derivative evaluated at the same pre-update weights.

##### Sigmoid-softmax network gradients

↑ **Parent:** [Backpropagation](#backpropagation)

For hidden activations $h_j=\sigma(b_j+\sum_rW_{jr}x_r)$ and class probabilities $p_c=\operatorname{softmax}_c(a+Vh)$, a one-hot label $t$ has [log-likelihood](statistical-modelling.md#log-likelihood) $\ell=\sum_ct_c\log p_c$. Put $\delta_c=t_c-p_c$ and $\Delta_j=h_j(1-h_j)\sum_cV_{cj}\delta_c$. Then

$$
\partial_{a_c}\ell=\delta_c,\quad\partial_{V_{cj}}\ell=\delta_ch_j,\quad\partial_{b_j}\ell=\Delta_j,\quad\partial_{W_{jr}}\ell=\Delta_jx_r.
$$

These follow from the [chain rule](calculus.md#chain-rule) and give single-observation [stochastic gradient descent](numerical-analysis.md#stochastic-gradient-descent) updates for the negative [log-likelihood](statistical-modelling.md#log-likelihood).

### Sigmoid function

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sigmoid_function)

The sigmoid function

$$
\sigma(x)=\frac{1}{1+e^{-x}}
$$

is a smooth activation function with derivative $\sigma'(x)=\sigma(x)(1-\sigma(x))$.

#### Logistic function

↑ **Parent:** [Sigmoid function](#sigmoid-function)

The standard logistic function maps a [log odds](statistical-modelling.md#log-odds) $z$ to probability $1/(1+e^{-z})$. More generally, its translated and scaled form is $L/(1+e^{-k(x-x_0)})$.

### Rectified linear unit

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rectified_linear_unit)

The rectified linear unit activation is $\operatorname{ReLU}(x)=\max(x,0)$.

### Gaussian error linear unit

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_error_linear_unit)

The Gaussian error linear unit activation is $\operatorname{GELU}(x)=x\Phi(x)$, where $\Phi$ is the [standard normal distribution function](probability-theory.md#standard-normal-distribution-function).

### Softmax function

↑ **Parent:** [Neural network](#neural-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Softmax_function)

For logits $z_1,\ldots,z_K$, the softmax probabilities are $p_k=e^{z_k}/\sum_je^{z_j}$.

#### Softmax non-identifiability

↑ **Parent:** [Softmax function](#softmax-function)

Adding the same scalar-valued function of the input to every class logit leaves all softmax probabilities unchanged. A reference-class constraint removes this common-shift non-identifiability.

#### Categorical cross-entropy loss

↑ **Parent:** [Softmax function](#softmax-function)

For one-hot label $y$ and predicted class probabilities $p$, categorical cross-entropy is $-\sum_ky_k\log p_k$, the negative categorical log-likelihood.

## Overfitting

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Overfitting)

Overfitting occurs when further adaptation improves training performance while degrading performance on new data.

## Regularization

↑ **Parent:** [Statistical learning](statistical-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regularization)

Regularization restricts or penalizes model fitting to improve generalization.

### Penalized least squares

↑ **Parent:** [Regularization](#regularization)

For $\lambda\geq0$, a full-column-rank [design matrix](linear-regression.md#design-matrix) $B$, and a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) $\Omega$, minimize $\|y-B\beta\|^2+\lambda\beta^T\Omega\beta$. Differentiation gives $(B^TB+\lambda\Omega)\widehat\beta=B^Ty$. The fitted-value matrix is $B(B^TB+\lambda\Omega)^{-1}B^T$, whose trace measures the [effective degrees of freedom](linear-regression.md#effective-degrees-of-freedom).

#### Penalized least-squares estimator

↑ **Parent:** [Penalized least squares](#penalized-least-squares)

A penalized least-squares estimator balances squared error with a nonnegative penalty $J$. The [Lasso](probability-and-statistics.md#lasso) uses the coefficient $\ell_1$ [norm](functional-analysis.md#norm); [graph total variation denoising](inverse-problem.md#graph-total-variation-denoising) uses the $\ell_1$ [norm](functional-analysis.md#norm) of endpoint differences. The choice of normalization of the squared loss changes the numerical tuning parameter.

##### Basic inequality for a penalized least-squares estimator

↑ **Parent:** [Penalized least-squares estimator](#penalized-least-squares-estimator)

For the identity design and $y=\theta^*+z$, comparing the minimizing objective at $\widehat\theta$ with its value at $\theta^*$ and expanding the squared [Euclidean norm](functional-analysis.md#euclidean-norm) proves the displayed inequality, with $h=\widehat\theta-\theta^*$. This deterministic inequality does not assume any [probability distribution](probability-theory.md#probability-distribution) for the noise. A bound on the noise inner product turns it into a statistical error estimate.

### Roughness penalty

↑ **Parent:** [Regularization](#regularization)

A [roughness penalty](#roughness-penalty) penalizes variation of derivatives, such as $\int(m^{\prime\prime})^2$. The second-derivative penalty vanishes precisely on [affine functions](vector-space.md#affine-function) and is represented in a chosen basis by a [roughness penalty matrix](statistical-modelling.md#roughness-penalty-matrix).

### Early stopping

↑ **Parent:** [Regularization](#regularization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Early_stopping)

Early stopping halts iterative fitting near the best validation performance, limiting adaptation to training noise.

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)
