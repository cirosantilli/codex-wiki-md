<h1 id="finite-set-example-of-the-johnson-lindenstrauss-lemma">Finite-set example of the Johnson–Lindenstrauss lemma</h1>

↑ **Parent:** [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)

Here is an original reproducible [finite set](finite-set.md) with 40 points and 512 coordinates. Let $e_1,\ldots,e_4$ be the first four [vectors](vector.md) of the [standard basis](standard-basis.md) of $\mathbb R^{512}$. With point indices $i=0,\ldots,39$, generate

$$
x_i=2e_{1+\lfloor i/10\rfloor}+\frac{z_i}{\sqrt{512}},
\qquad z_{ij}\sim N(0,1)\text{ independently}.
$$

The four groups have different centers, and the [standard normal random variables](standard-normal-random-variable.md) perturb all 512 coordinates. Generate the coordinates in row order using NumPy's PCG64 [pseudorandom number generator](pseudorandom-number-generator.md) with seed 20261013. Then keep this [finite set](finite-set.md) fixed. A second PCG64 stream with seed 424242 generates a $32\times512$ [matrix](matrix.md) of [independent random variables](independent-random-variables.md) with the [standard normal distribution](standard-normal-distribution.md); divide it by $\sqrt{32}$ to obtain the [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md).

For all 780 unordered pairs, compute the distance ratio $r_{ij}=\|Tx_i-Tx_j\|_2/\|x_i-x_j\|_2$. In this draw, its minimum is approximately $0.733010$ and its maximum $1.478785$, giving a maximum [relative error](relative-error.md) in [Euclidean distance](euclidean-distance.md) of about $0.478785$. The squared-distance ratios $r_{ij}^2$ instead range from approximately $0.537304$ to $2.186806$: their maximum [relative error](relative-error.md) is about $1.186806$. Thus this particular draw fails a 20% distance tolerance. The [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md) does not assert that every draw into 32 dimensions must succeed.

<a id="image-all-780-pairwise-euclidean-distances-for-one-gaussian-map-from-512-to-32-dimensions"></a>
![](johnson-lindenstrauss-pairwise-distance-distortion.png)

**[Figure 3](#image-all-780-pairwise-euclidean-distances-for-one-gaussian-map-from-512-to-32-dimensions). All 780 pairwise Euclidean distances for one Gaussian map from 512 to 32 dimensions**.

The two bands of original [Euclidean distances](euclidean-distance.md) distinguish pairs within a group from pairs between groups. Their spread after the [linear map](linear-map.md) shows why checking an average distance is insufficient: the [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md) controls every pair. The dashed 20% distance band is an illustrative tolerance, not a [confidence interval](confidence-interval.md) or a squared-distance band. The [affine hull](affine-hull.md) of 40 points has [dimension](dimension-vector-space.md) at most 39; 512 is the ambient coordinate count, and no full-dimensionality assumption is required. For this draw the [bi-Lipschitz distortion](bi-lipschitz-distortion.md) is approximately $1.478785/0.733010=2.017414$.

Now keep the same points and draw 48 fresh [Gaussian Johnson–Lindenstrauss transforms](gaussian-johnson-lindenstrauss-transform.md) for each target [dimension](dimension-vector-space.md) $k\in\{8,16,32,64,128\}$. NumPy's `SeedSequence(314159).spawn(240)` supplies distinct PCG64 streams, ordered first by target [dimension](dimension-vector-space.md), then by draw. Each stream generates a new $k\times512$ [random matrix](random-matrix.md), normalized by $1/\sqrt k$; no map is a row prefix of another map. Each plotted value is

$$
E(T)=\max_{i<j}\left|\frac{\|Tx_i-Tx_j\|_2}{\|x_i-x_j\|_2}-1\right|.
$$

<a id="image-maximum-relative-distance-error-over-independently-drawn-gaussian-maps-at-five-target-dimensions"></a>
![](gaussian-projection-target-dimension-distortion.png)

**[Figure 4](#image-maximum-relative-distance-error-over-independently-drawn-gaussian-maps-at-five-target-dimensions). Maximum relative distance error over independently drawn Gaussian maps at five target dimensions**.

The observed [median](median.md) maximum [relative errors](relative-error.md) in [Euclidean distance](euclidean-distance.md) are approximately $0.735$, $0.520$, $0.381$, $0.267$, and $0.184$, respectively. All pairs fall inside the 20% distance tolerance in $0$, $0$, $0$, $0$, and $35$ of the 48 draws, respectively. These are computations on one synthetic [finite set](finite-set.md), rather than optimal dimension bounds or measured physical data. The displayed [quantiles](quantile-function.md) describe the sampled maps; they do not certify a success [probability](probability.md) for other sets. Even at 128 dimensions, 13 of the sampled maps fail this tolerance.

The practical benefit is that each point acquires fewer coordinates while its pairwise [Euclidean distances](euclidean-distance.md) can remain useful. The choice of target [dimension](dimension-vector-space.md) balances compression, accuracy, and failure [probability](probability.md). For example, a conservative sufficient squared-distance tolerance $\varepsilon=0.2$ with $n=40$ and $\delta=0.05$ gives $k\geq1195$ by the explicit bound above. Here that exceeds the ambient [dimension](dimension-vector-space.md), so the [identity map](identity-function.md) is better for a certified guarantee. The much smaller dimensions in the plots illustrate observed behavior without claiming that this sufficient bound is sharp.

## ↑ Ancestors (8)

1. [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)
2. [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
3. [Metric embedding](metric-embedding-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
