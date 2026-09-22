# Local influence versus replacement breakdown

↑ **Parent:** [Influence function](influence-function.md)

The [influence function](influence-function.md) describes an infinitesimal change at a specified reference [probability distribution](probability-distribution.md). The [replacement breakdown point](replacement-breakdown-point.md) asks how many observations in a particular finite sample can be replaced before an [estimator](estimator.md) becomes unbounded. The [finite-sample maximum bias](finite-sample-maximum-bias.md) records the intervening changes. These are different questions: a bounded [influence function](influence-function.md) at one baseline is not a general bound over all [epsilon-contamination neighborhoods](epsilon-contamination-neighborhood.md), nor a proof of a positive [replacement breakdown point](replacement-breakdown-point.md).[Frank R. Hampel, The Influence Curve and Its Role in Robust Estimation, §4, p. 386: exact asymptotic curve supplemented by behavior at other distributions, especially empirical ones](the-influence-curve-and-its-role-in-robust-estimation-by-frank-r-hampel.md)

The [mean](expected-value.md) illustrates agreement between local and global fragility: its [gross-error sensitivity](gross-error-sensitivity.md) is infinite and one replacement can send the [sample mean](sample-mean.md) arbitrarily far. The [median](median.md) has finite [gross-error sensitivity](gross-error-sensitivity.md) under the stated positive-density assumptions, while its [sample median](sample-median.md) withstands fewer than about half the observations being replaced under ordinary tie conventions. Its population contamination bias above still diverges as $\varepsilon\uparrow1/2$ when the atom remains beyond the shifted [median](median.md). Here $x$ must also move outward; taking that limit with a fixed finite atom would invalidate the displayed [quantile](quantile-function.md) formula.

For scalar location with a fixed positive scale, the [Huber score](huber-score.md) has a direct global argument: if strictly more than half of the sample stays fixed, then beyond every retained observation by more than $ks$, their saturated scores outweigh all possible replaced scores. Every root therefore stays in a bounded interval. This is a separate finite-replacement argument; estimating scale changes its premises. A smooth bounded [influence function](influence-function.md) is valuable local protection, but global robustness also depends on the full estimating rule, scale choice, and root selection.

## ↑ Ancestors (7)

1. [Influence function](influence-function.md)
2. [Robust statistics](robust-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
