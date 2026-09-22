# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper30.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let each observation have dimension $p$, and define the [sample mean](../../../variance.md#sample-mean) and the divisor-$n$ [sample covariance matrix](../../../variance.md#sample-covariance-matrix) by

$$
\bar y=\frac1n\sum_{i=1}^ny_i,\qquad S=\frac1n\sum_{i=1}^n(y_i-\bar y)(y_i-\bar y)^T.
$$

The [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) gives the [log-likelihood](../../../statistical-modelling.md#log-likelihood)

$$
\ell(\mu,V)=-\frac{np}{2}\log(2\pi)-\frac n2\log\det V
-\frac12\sum_i(y_i-\mu)^TV^{-1}(y_i-\mu).
$$

Writing $y_i-\mu=(y_i-\bar y)+(\bar y-\mu)$ makes the cross terms vanish, and the last sum becomes $n\operatorname{tr}(V^{-1}S)+n(\bar y-\mu)^TV^{-1}(\bar y-\mu)$. Since $V$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), its minimum over the mean is at $\widehat\mu=\bar y$. Consequently

$$
\ell_p(V):=\max_\mu\ell(\mu,V)
=-\frac n2\log\det V-\frac n2\operatorname{tr}(V^{-1}S)+C.
$$

When $S$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), $\log\det(V^{-1}S)=\log\det S-\log\det V$. Thus

$$
\ell_p(V)=\frac n2\log\det(V^{-1}S)-\frac n2\operatorname{tr}(V^{-1}S)+C',
$$

where $C'$ depends on the data but not on $V$.

For the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator), consider the [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $Q=S^{1/2}V^{-1}S^{1/2}$, with positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $a_1,\ldots,a_p$. The part of the [profile likelihood](../../../statistical-modelling.md#profile-likelihood) depending on $V$ is $\frac n2\sum_j(\log a_j-a_j)$. The elementary inequality $\log a-a\leq-1$, with equality exactly at $a=1$, shows that the unique maximizing matrix is $Q=I$. Hence

$$
\boxed{\widehat\mu=\bar y,\qquad\widehat V=S.}
$$

The divisor is $n$, not the unbiased covariance divisor $n-1$. The regularity qualification matters: if $S$ is singular, the displayed logarithm of its determinant is not finite, and no positive-definite covariance maximizes the likelihood. Sending the fitted variance in a null direction of $S$ to zero makes the likelihood unbounded. For a nonsingular normal population, $S$ is positive definite almost surely when $n>p$, which is the setting of the large-sample test.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Under the diagonal covariance restriction, the [profile log-likelihood](../../../statistical-modelling.md#profile-log-likelihood) separates into $p$ terms,

$$
-\frac n2\sum_j\left(\log v_j+\frac{S_{jj}}{v_j}\right)+C.
$$

Differentiating each term gives the restricted [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) $\widehat V_0=D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. Both fitted trace terms equal $p$, so the [likelihood-ratio test statistic](../../../statistical-modelling.md#likelihood-ratio-test-statistic) is

$$
\boxed{W=2\{\ell_p(S)-\ell_p(D)\}
=n\log\frac{\prod_jS_{jj}}{\det S}=-n\log\det R,}
$$

where $R=D^{-1/2}SD^{-1/2}$ is the [sample correlation matrix](../../../variance.md#sample-correlation-matrix). The statistic is nonnegative by the [Hadamard inequality](../../../linear-algebra.md#hadamard-determinant-inequality); large values indicate dependence. Equivalently, the likelihood ratio is $(\det S/\det D)^{n/2}$ and rejection is for small values of this ratio.

For fixed $p$ and a positive-definite true covariance, the [Wilks theorem](../../../statistical-inference.md#wilks-theorem) says that twice the maximized log-likelihood difference for nested regular models converges under the null to a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with degrees of freedom equal to the dimension difference. The unrestricted covariance has $p(p+1)/2$ parameters and the restricted covariance has $p$; the unknown mean has the same $p$ parameters in both. Therefore the [Gaussian covariance diagonality likelihood-ratio test](../../../statistical-modelling.md#gaussian-covariance-diagonality-likelihood-ratio-test) of asymptotic level $\alpha$ is

$$
\boxed{\text{reject if }W>\chi^2_{p(p-1)/2,\,1-\alpha}.}
$$

Within the [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution), diagonal covariance also means independent coordinates.

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Treat the displayed entries as the lower triangle of a symmetric [sample covariance matrix](../../../variance.md#sample-covariance-matrix) $S$, in the order mechanics, vectors, algebra, analysis, statistics. Compute the [precision matrix](../../../variance.md#precision-matrix) $K=S^{-1}$. For a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution), conditioning on all remaining coordinates gives

$$
\widehat{\operatorname{Var}}(Y_j\mid Y_{-j})=\frac1{K_{jj}},\qquad
\widehat{\operatorname{Corr}}(Y_i,Y_j\mid Y_{-(i,j)})
=-\frac{K_{ij}}{\sqrt{K_{ii}K_{jj}}}.
$$

These identities follow by fixing the other coordinates in the quadratic form of the normal density and completing the square. For the second identity, the conditional [precision matrix](../../../variance.md#precision-matrix) for the retained pair is its $2\times2$ principal block; inverting that block gives the negative off-diagonal entry divided by the square root of the two diagonal entries.

Thus the two quantities to evaluate are

$$
\boxed{\frac1{K_{11}S_{11}}\simeq0.62,\qquad
-\frac{K_{54}}{\sqrt{K_{55}K_{44}}}\simeq0.25.}
$$

An equivalent procedure uses the [Schur complement covariance](../../../probability-and-statistics.md#schur-complement-covariance): regress mechanics on the other four variables, or regress analysis and statistics separately on the remaining three. The first residual [variance](../../../variance.md) is $S_{11}-S_{1,-1}S_{-1,-1}^{-1}S_{-1,1}$; the second result is the [partial correlation](../../../variance.md#partial-correlation) of the two residuals. No arithmetic is required to specify this method.

The model qualification is important: a covariance matrix alone determines linear-regression residual variances and [partial correlations](../../../variance.md#partial-correlation). Identifying them with conditional quantities independent of the observed conditioning values uses the [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) model, or another model with the same conditional moments; it does not follow for arbitrary distributions.

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Principal component analysis](../../../statistical-learning.md#principal-component-analysis) replaces correlated measurements by orthogonal linear coordinates ordered by their [variance](../../../variance.md). For centered observations collected in an $n\times p$ [matrix](../../../vector-space.md#matrix) $Z$, write the [sample covariance matrix](../../../variance.md#sample-covariance-matrix) as $S=Z^TZ/(n-1)$. A unit loading vector $a$ gives score vector $Za$ with sample [variance](../../../variance.md) $a^TSa$. The [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) is maximized by a unit [eigenvector](../../../linear-operator-theory.md#eigenvector) of $S$ for its largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

The subsequent [principal components](../../../statistical-learning.md#principal-component) maximize the same quadratic form subject to orthogonality to the earlier loading vectors. By the [spectral theorem](../../../hilbert-space.md#spectral-theorem), if $S=Q\Lambda Q^T$ with descending eigenvalues, the scores $ZQ$ have diagonal covariance $\Lambda$. Their fractions of explained [variance](../../../variance.md) are $\lambda_j/\sum_i\lambda_i$. Repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) identify an eigenspace rather than a unique axis.

Keeping the first $q$ [principal components](../../../statistical-learning.md#principal-component) gives the rank-$q$ reconstruction $\widehat Z=ZQ_qQ_q^T$. Its squared reconstruction error is

$$
\|Z-\widehat Z\|_F^2=(n-1)\sum_{j>q}\lambda_j.
$$

For any rank-$q$ orthogonal projection $P$, retained variance is $\operatorname{tr}(SP)=\sum_j\lambda_j q_j^TPq_j$. The weights $q_j^TPq_j$ lie in $[0,1]$ and sum to $q$, so this is at most the sum of the largest $q$ eigenvalues. Projecting onto any candidate reconstruction subspace is its best least-squares reconstruction; this proves the minimum-error property and agrees with the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition). Thus **PCA finds the linear subspace preserving the greatest variance, equivalently minimizing squared reconstruction error.** The upper-left sketch shows the first axis aligned with the elongated cloud; the second is perpendicular. A [scree plot](../../../statistical-learning.md#scree-plot) and substantive interpretability help choose $q$.

<a id="3/a/image-original-sketches-of-principal-components-classical-scaling-hierarchical-clustering-and-multivariate-mean-comparison"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30-multivariate-sketches.png)

**[Figure 1](#3/a/image-original-sketches-of-principal-components-classical-scaling-hierarchical-clustering-and-multivariate-mean-comparison). Original sketches of principal components, classical scaling, hierarchical clustering and multivariate mean comparison**.

These methods depend on measurement scale. A variable measured in large numerical units can dominate covariance-based [principal component analysis](../../../statistical-learning.md#principal-component-analysis); standardizing variables gives [principal component analysis on a correlation matrix](../../../statistical-learning.md#principal-component-analysis-on-a-correlation-matrix). Scores summarize patterns, but the method neither establishes causation nor guarantees that the largest-variance directions best predict a separate response.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

[Classical multidimensional scaling](../../../statistical-learning.md#classical-multidimensional-scaling) begins with a symmetric [dissimilarity matrix](../../../statistical-learning.md#dissimilarity-matrix) $D$, rather than necessarily with measured coordinates. Its aim is to find a low-dimensional Euclidean configuration representing those dissimilarities. Square the entries, not the matrix product, and define

$$
J=I-\frac1n\mathbf1\mathbf1^T,\qquad B=-\frac12J D^{(2)}J.
$$

For centered coordinates $X$, squared [Euclidean distances](../../../topological-analysis.md#euclidean-distance) satisfy $D_{ij}^2=B_{ii}+B_{jj}-2B_{ij}$ with $B=XX^T$. Multiplication on both sides by $J$ annihilates the two single-index terms, proving the double-centering formula.

If $B$ is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix), use its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) $B=U\Lambda U^T$ to construct

$$
\boxed{X_q=U_q\Lambda_q^{1/2}.}
$$

Keeping all positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) reproduces the original [Euclidean distances](../../../topological-analysis.md#euclidean-distance) exactly; their number is the minimal embedding dimension. Keeping fewer gives a low-rank approximation to the [Gram matrix](../../../linear-algebra.md#gram-matrix). It minimizes squared Gram-matrix error, often called strain, rather than necessarily the sum of squared errors in raw distances. Negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) signal that the dissimilarities cannot be represented exactly by Euclidean coordinates; discarding them produces an approximation whose adequacy should be inspected.

In the upper-right sketch, the supplied distances come from four points in a rectangle, and the two-dimensional reconstruction recovers that shape. The overall translation, rotation and reflection of the configuration are not identifiable from distances. **Classical scaling reconstructs centered geometry from pairwise distances.** If the input distances are computed from centered multivariate observations, classical scaling and [principal component analysis](../../../statistical-learning.md#principal-component-analysis) give the same score configuration up to an orthogonal transformation: their matrices $ZZ^T$ and $Z^TZ$ share the nonzero squared singular values.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[Agglomerative hierarchical clustering](../../../statistical-learning.md#agglomerative-hierarchical-clustering) starts with each observation as a singleton [cluster in cluster analysis](../../../statistical-learning.md#cluster-in-cluster-analysis), repeatedly joins the closest pair of current clusters, and continues until one remains. The input is a [dissimilarity matrix](../../../statistical-learning.md#dissimilarity-matrix), so choosing variable scales and a scientifically sensible dissimilarity is part of the analysis.

Different linkages define closeness differently:

$$
\begin{aligned}
d_{\mathrm{single}}(A,B)&=\min_{i\in A,j\in B}d_{ij},\\
d_{\mathrm{complete}}(A,B)&=\max_{i\in A,j\in B}d_{ij},\\
d_{\mathrm{average}}(A,B)&=\frac1{|A||B|}\sum_{i\in A,j\in B}d_{ij}.
\end{aligned}
$$

[Single-linkage clustering](../../../statistical-learning.md#single-linkage-clustering) can connect elongated chains through nearest neighbors; [complete-linkage clustering](../../../statistical-learning.md#complete-linkage-clustering) emphasizes compact clusters; [average-linkage clustering](../../../statistical-learning.md#average-linkage-clustering) averages all cross-pair distances. For Euclidean observations, [Ward minimum-variance clustering](../../../statistical-learning.md#ward-minimum-variance-clustering) instead chooses the smallest increase in within-cluster squared error,

$$
\Delta(A,B)=\frac{|A||B|}{|A|+|B|}\|\bar x_A-\bar x_B\|^2.
$$

This follows by expanding squared deviations around the merged mean and using the zero sums of within-cluster residuals.

A [dendrogram](../../../statistical-learning.md#dendrogram) plots merge heights. In the lower-left sketch, two close pairs first merge at small heights, then join across a much larger separation; a horizontal cut between these heights yields two groups. **The hierarchy gives nested partitions, not a uniquely established number of populations.** Examine sensitivity to scaling, linkage and ties; once an agglomerative merge is made, the method does not undo it. The absence of a probability model also means that a visually attractive [dendrogram](../../../statistical-learning.md#dendrogram) is not itself a significance test.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

[Multivariate analysis of variance](../../../linear-regression.md#multivariate-analysis-of-variance) tests differences between group mean vectors when each experimental unit has several correlated responses. For independent $p$-dimensional observations in $g$ groups, use a common positive-definite [covariance matrix](../../../variance.md#covariance-matrix) $\Sigma$ and the [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) model $Y_{ri}\sim N_p(\mu_r,\Sigma)$. The null hypothesis is equality of all $g$ means.

Write $n=\sum_rn_r$, group means $\bar y_r$, and the size-weighted grand mean $\bar y$. The within-group and between-group scatter matrices are

$$
E=\sum_{r,i}(y_{ri}-\bar y_r)(y_{ri}-\bar y_r)^T,
\qquad H=\sum_rn_r(\bar y_r-\bar y)(\bar y_r-\bar y)^T.
$$

Expanding deviations about the group means yields total scatter $T=E+H$, with zero cross terms. Under the null, orthogonal normal projections give independent [Wishart distributions](../../../probability-theory.md#wishart-distribution) $E\sim W_p(\Sigma,n-g)$ and $H\sim W_p(\Sigma,g-1)$.

With nonsingular $E$, the [Wilks lambda statistic](../../../linear-regression.md#wilks-lambda-statistic) is

$$
\boxed{\Lambda=\frac{\det E}{\det(E+H)}=\prod_j(1+\theta_j)^{-1},}
$$

where the nonnegative $\theta_j$ are [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $E^{-1/2}HE^{-1/2}$. Maximizing the common covariance under the two mean models gives the likelihood ratio $\Lambda^{n/2}$, so small $\Lambda$ indicates large group separation relative to within-group spread. For fixed $p,g$ and large group sizes, the [Wilks theorem](../../../statistical-inference.md#wilks-theorem) gives $-n\log\Lambda\Rightarrow\chi^2_{p(g-1)}$ under the null; a finite-sample reference distribution can also be used.

The lower-right sketch shows two elongated groups whose centroid difference lies nearly across, rather than along, their long axes. Their correlation makes this multivariate separation much clearer than either marginal mean shift alone. Nonsingular linear rescaling changes $E$ and $H$ by congruence, leaving the determinant ratio unchanged. **MANOVA measures mean separation against the full within-group covariance geometry.** Its interpretation requires independent observations and an adequate common-covariance model; separate coordinatewise tests discard that geometry and raise multiple-testing issues.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [balanced incomplete block design](../../../statistical-modelling.md#balanced-incomplete-block-design) has $t$ treatments and $b$ blocks, each containing $k$ distinct treatments with $1<k<t$. Every treatment occurs in $r$ blocks and every distinct treatment pair occurs together in $\lambda>0$ blocks. A [symmetric balanced incomplete block design](../../../statistical-modelling.md#symmetric-balanced-incomplete-block-design) has $b=t$, which implies $r=k$ by the first counting identity below.

For the separate even-order condition, let $N$ be the square treatment-by-block [incidence matrix of a set system](../../../extremal-set-theory.md#incidence-matrix-of-a-set-system) of a symmetric design. Its diagonal overlap counts are $r$ and its off-diagonal counts are $\lambda$, giving

$$
NN^T=(r-\lambda)I+\lambda J.
$$

The counting identities proved in the next slots show that $r=k$ and $r+(t-1)\lambda=r^2$. Consequently the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $NN^T$ are $r^2$ on the constant vector and $r-\lambda$ on its $(t-1)$-dimensional orthogonal complement. Taking [determinants](../../../linear-algebra.md#determinant) gives

$$
\det(N)^2=r^2(r-\lambda)^{t-1}.
$$

If $b=t$ is even, the exponent $t-1$ is odd. The exponent of every prime in $\det(N)^2$ and in $r^2$ is even; therefore its exponent in the positive integer $r-\lambda$ must be even. This proves the [even-order symmetric design square obstruction](../../../statistical-modelling.md#even-order-symmetric-design-square-obstruction):

$$
\boxed{r-\lambda\text{ is a perfect square}.}
$$

It is a necessary condition, not a sufficiency claim.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Count incidences of a treatment with a block containing it. Summing over blocks gives $bk$, while summing over treatments gives $tr$. Hence the [balanced incomplete block design](../../../statistical-modelling.md#balanced-incomplete-block-design) satisfies

$$
\boxed{bk=tr.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Fix one treatment. Each of its $r$ blocks supplies $k-1$ companion treatments, giving $r(k-1)$ incidences. Alternatively, each of the other $t-1$ treatments accompanies it in exactly $\lambda$ blocks. Thus

$$
\boxed{r(k-1)=\lambda(t-1).}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $N$ be the $t\times b$ [incidence matrix of a set system](../../../extremal-set-theory.md#incidence-matrix-of-a-set-system). The [balanced incomplete block design](../../../statistical-modelling.md#balanced-incomplete-block-design) overlap counts give $NN^T=(r-\lambda)I+\lambda J$. On the zero-sum subspace its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $r-\lambda=r(t-k)/(t-1)>0$; on the constant vector its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $r+(t-1)\lambda>0$. Therefore $NN^T$ has [matrix rank](../../../vector-space.md#matrix-rank) $t$. Since a product cannot have larger rank than either factor,

$$
\boxed{t=\operatorname{rank}(NN^T)\leq\operatorname{rank}(N)\leq b.}
$$

This proves [Fisher's inequality for block designs](../../../statistical-modelling.md#fisher-s-inequality-for-block-designs) directly. The incomplete, nontrivial hypotheses ensure the positive eigenvalue needed for this argument.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Symmetry forces $r=k$, and the pair-counting identity becomes $k(k-1)=2\cdot45=90$. Its only positive integral solution is $k=r=10$. Since the number of blocks is even, the [even-order symmetric design square obstruction](../../../statistical-modelling.md#even-order-symmetric-design-square-obstruction) requires $r-\lambda=8$ to be a square. It is not. **No design with these parameters exists.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The identities require $r=k$ and $k(k-1)=2\cdot3=6$, so $k=r=3$. Take treatments $1,2,3,4$ and the four blocks

$$
\boxed{\{1,2,3\},\quad\{1,2,4\},\quad\{1,3,4\},\quad\{2,3,4\}.}
$$

Each treatment is absent from exactly one block, hence occurs three times. Each pair is absent from the two blocks missing one of its members, hence occurs together in the other two. This is the required [symmetric balanced incomplete block design](../../../statistical-modelling.md#symmetric-balanced-incomplete-block-design); here $r-\lambda=1$ is indeed a square.

## 5

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Code the two levels of each factor as $\pm1$. For a factor subset $A$, its [factorial contrast](../../../statistical-modelling.md#factorial-contrast) column is the character $\chi_A(x)=\prod_{j\in A}x_j$. Products of columns correspond to symmetric differences of subsets, because $x_j^2=1$.

Let $G_1,\ldots,G_k$ be defining words whose incidence vectors are linearly independent over $\mathbb F_2$. Write $x_j=(-1)^{u_j}$, with $u_j\in\mathbb F_2$. Specifying signs $\chi_{G_i}(x)=s_i$ is then a rank-$k$ system of binary linear equations. Every one of its $2^k$ right-hand sides has $2^{n-k}$ solutions. Thus **$k$ independent defining contrasts split the full $2^n$ design into $2^k$ equal fractions.** Independence is necessary: dependent defining words do not yield $2^k$ distinct sets.

The [defining contrast subgroup](../../../statistical-modelling.md#defining-contrast-subgroup) has $2^k$ words. On a selected fraction its word $G$ has a constant sign $s_G$, so

$$
\chi_{AG}=s_G\chi_A.
$$

Hence the coefficients of $A$ and $AG$ cannot be estimated separately without assumptions or extra runs: this is [aliasing in a fractional factorial design](../../../statistical-modelling.md#aliasing-in-a-fractional-factorial-design). Conversely, averaging a character over the affine binary solution space vanishes unless its word is in the defining subgroup, so these signed subgroup cosets give all aliases. Here a lowercase treatment label records the factors at their high levels, and $(1)$ puts all five at their low levels; signs must be retained when listing aliases.

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

On these eight runs, $W=M$ and $SCT=-1$. The two independent defining words therefore give the full signed defining relation

$$
I=WM=-SCT=-SCWMT.
$$

Multiplying each desired [factorial contrast](../../../statistical-modelling.md#factorial-contrast) by its four words gives all aliases. In the following equalities a minus sign means opposite contrast columns:

$$
\begin{aligned}
S&=SWM=-CT=-CWMT,\\
C&=CWM=-ST=-SWMT,\\
W&=M=-SCWT=-SCMT,\\
M&=W=-SCMT=-SCWT,\\
T&=WMT=-SC=-SCWM,\\
ST&=SWMT=-C=-CWM.
\end{aligned}
$$

Thus two [main effects](../../../statistical-modelling.md#main-effect), $W$ and $M$, are inseparable even when every unwanted interaction vanishes. In addition, the important interaction $ST$ aliases with the [main effect](../../../statistical-modelling.md#main-effect) $C$. **Design (a) is unsuitable.** The seven-column [design matrix](../../../linear-regression.md#design-matrix) for the intercept, the five main effects and $ST$ has rank five, confirming the two independent estimability failures.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For this fraction, $SCW=-1$ and $SCMT=1$, so their product is $WMT=-1$. The signed defining relation is

$$
I=-SCW=SCMT=-WMT.
$$

The complete [factorial contrast](../../../statistical-modelling.md#factorial-contrast) alias classes are

$$
\begin{aligned}
S&=-CW=CMT=-SWMT,\\
C&=-SW=SMT=-CWMT,\\
W&=-SC=SCWMT=-MT,\\
M&=-SCWM=SCT=-WT,\\
T&=-SCWT=SCM=-WM,\\
ST&=-CWT=CM=-SWM.
\end{aligned}
$$

The five [main effects](../../../statistical-modelling.md#main-effect) and $ST$ occupy six distinct alias classes, and none aliases with the intercept. Every undesired two-factor term in these classes is assumed negligible, and all terms of order at least three are also assumed negligible. Thus **design (b) is suitable under the stated interaction assumptions**. Its intercept and six requested columns are mutually orthogonal, with $X^TX=8I_7$, so each coded regression coefficient is $\widehat\beta_A=8^{-1}\sum_{i=1}^8\chi_A(x_i)Y_i$. The corresponding high-minus-low [main effect](../../../statistical-modelling.md#main-effect) is $2\widehat\beta_A$.

There is one residual degree of freedom, but no replicated setting and therefore no separate [pure error](../../../statistical-modelling.md#pure-error) estimate. Suitability here means estimability under the stated model; it does not protect estimates from active interactions that the assumptions exclude.

## 6

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For the general [normal linear model](../../../statistical-modelling.md#normal-linear-model), minimizing $\|Y-X\beta\|^2$ gives the [least-squares normal equations](../../../linear-regression.md#normal-equations-for-linear-least-squares) $X^TX\widehat\beta=X^TY$. Full column rank makes $X^TX$ invertible, so

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
\mathbb E\widehat\beta=\beta,\qquad
\operatorname{Cov}(\widehat\beta)=\sigma^2(X^TX)^{-1}.}
$$

The mean and covariance follow by substituting $Y=X\beta+\epsilon$ and using $\mathbb E\epsilon=0$, $\operatorname{Cov}(\epsilon)=\sigma^2I$. Normal errors also give the exact multivariate normal distribution of this estimator.

Use [coded experimental variables](../../../statistical-modelling.md#coded-experimental-variable)

$$
\boxed{x_1=\frac{\xi_1-95}{5},\qquad x_2=\frac{\xi_2-37.5}{2.5}.}
$$

Their origin is the middle of the allowed rectangle, and the stated endpoints become $\pm1$. The four corners and $n_0$ center runs give mutually orthogonal columns $1,x_1,x_2$, with

$$
X^TX=\operatorname{diag}(4+n_0,4,4).
$$

Writing $\bar Y_0=n_0^{-1}\sum_{i=5}^{4+n_0}Y_i$ when $n_0>0$, the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimates are

$$
\boxed{\begin{aligned}
\widehat\beta_0&=\frac{\sum_{i=1}^{4+n_0}Y_i}{4+n_0},\\
\widehat\beta_1&=\frac{Y_1+Y_2-Y_3-Y_4}{4},\\
\widehat\beta_2&=\frac{Y_1-Y_2-Y_3+Y_4}{4}.
\end{aligned}}
$$

Their variances are $\sigma^2/(4+n_0)$, $\sigma^2/4$, $\sigma^2/4$, with zero covariances.

The repeated center runs estimate [pure error](../../../statistical-modelling.md#pure-error) without requiring the fitted mean surface to be correct:

$$
s_{\rm PE}^2=\frac{\sum_{i=5}^{4+n_0}(Y_i-\bar Y_0)^2}{n_0-1}\quad(n_0\geq2).
$$

They also permit a [center-point curvature contrast](../../../statistical-modelling.md#center-point-curvature-contrast). Let $\bar Y_F=(Y_1+Y_2+Y_3+Y_4)/4$ and $\widehat\gamma=\bar Y_F-\bar Y_0$. Under the first-order model, $\mathbb E\widehat\gamma=0$ and $\operatorname{Var}(\widehat\gamma)=\sigma^2(1/4+1/n_0)$. Under a quadratic surface, its expectation is $\beta_{11}+\beta_{22}$, since the linear and $x_1x_2$ terms average to zero. Thus

$$
\frac{\widehat\gamma^2}{s_{\rm PE}^2(1/4+1/n_0)}\sim F_{1,n_0-1}
$$

under the first-order normal model. With only one center run there is no pure-error degree of freedom. A zero center contrast does not exclude all curvature, because the two quadratic coefficients can cancel. The corners also estimate an interaction contrast; the full [Lack-of-fit F-test](../../../statistical-modelling.md#lack-of-fit-f-test) compares the first-order fit with the five setting means, with two lack-of-fit and $n_0-1$ pure-error degrees of freedom.

If the first-order model is adequate and $\widehat b=(\widehat\beta_1,\widehat\beta_2)^T\ne0$, [steepest ascent in response surface methodology](../../../statistical-modelling.md#steepest-ascent-in-response-surface-methodology) uses the unit coded direction $d=\widehat b/\|\widehat b\|$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) proves that it maximizes the predicted directional derivative. Run sequential settings $x=hd$ for increasing feasible $h$, corresponding to physical increments $(5hd_1,2.5hd_2)$ from the center. Stop or reduce the steps when measured yield ceases to improve, and refit locally near promising settings. Respect the allowed rectangle; if a boundary is reached, investigate feasible boundary directions rather than extrapolating outside it. A near-zero gradient offers no first-order ascent direction and calls for further modeling.

If curvature is indicated, add the four axial settings $(1,0),(-1,0),(0,1),(0,-1)$, together with further center replication. This face-centered [central composite design](../../../statistical-modelling.md#central-composite-design) stays inside the allowed physical ranges and separates the two squared coordinates, which the corners alone cannot do. Fit the full [quadratic regression](../../../linear-regression.md#quadratic-regression) surface

$$
m(x)=\beta_0+\beta_1x_1+\beta_2x_2+\beta_{11}x_1^2+\beta_{12}x_1x_2+\beta_{22}x_2^2.
$$

Write its fitted quadratic part as $x^TBx$, where $B_{11}=\widehat\beta_{11}$, $B_{22}=\widehat\beta_{22}$ and $B_{12}=B_{21}=\widehat\beta_{12}/2$. Its gradient and Hessian are $\widehat b+2Bx$ and $2B$. If $B$ is nonsingular, the stationary setting is

$$
\boxed{x_*=-\tfrac12B^{-1}\widehat b.}
$$

If $B$ is [negative definite](../../../linear-algebra.md#negative-definite-matrix) and $x_*$ is feasible, it is the fitted maximum. Otherwise compare feasible stationary settings, optima on each edge obtained from the restricted one-variable quadratic, and the corners. A singular or poorly determined $B$ calls for attention to ridge directions and more runs. Convert any chosen coded setting back using $\xi_1=95+5x_1$, $\xi_2=37.5+2.5x_2$, and confirm its yield experimentally. The fitted local surface guides the search; it does not establish an untested physical optimum.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
