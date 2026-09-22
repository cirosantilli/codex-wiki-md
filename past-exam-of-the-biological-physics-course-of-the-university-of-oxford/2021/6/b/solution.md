<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [point mutation](../../../../point-mutation.md) changes an individual nucleotide position, introducing heritable sequence variation. Replication errors and spontaneous chemical damage are possible origins; [mutation](../../../../mutation.md) does not occur because a future change would be useful. [Natural selection](../../../../natural-selection.md) changes the frequencies of variants through their effects on reproduction, while [genetic drift](../../../../genetic-drift.md) causes random frequency changes, especially in small populations. A sequence difference fixed between lineages is a substitution; many new [mutations](../../../../mutation.md) disappear and never become substitutions. Under a simple neutral diploid model, $2N_e\mu$ new neutral variants per generation times fixation [probability](../../../../probability.md) $1/(2N_e)$ gives substitution rate $\mu$, motivating a [molecular clock](../../../../molecular-clock.md) for suitable neutral sites.

To infer a [phylogenetic tree](../../../../phylogenetic-tree.md), compare homologous, preferably orthologous sequences and align corresponding sites. A [nucleotide substitution model](../../../../nucleotide-substitution-model.md) converts observed sequence differences into estimated evolutionary branch lengths, allowing for multiple changes at one site. For example, in the equal-frequency, equal-rate [Jukes-Cantor model](../../../../jukes-cantor-model.md), a site changes to any alternative with rate $\mu/3$, where $\mu$ is its total substitution rate. The probability of matching its initial state after elapsed time $t$ is $1/4+(3/4)e^{-4\mu t/3}$. Thus for an evolutionary separation with expected substitutions per site $d$, the observed mismatch fraction is $p=(3/4)(1-e^{-4d/3})$ and

$$
\boxed{d=-\frac34\ln\left(1-\frac{4p}{3}\right).}
$$

For small $p$, $d\simeq p$; near saturation $p=3/4$, large evolutionary distances become difficult to distinguish. The correction does not rescue fully saturated data. Real analyses may allow unequal nucleotide frequencies, transition biases and variation of rates between sites.

Tree topology and branch lengths can be estimated using [maximum likelihood estimation](../../../../maximum-likelihood-estimation-split.md) or [Bayesian phylogenetic inference](../../../../bayesian-phylogenetic-inference.md), with support assessed from resampling or posterior uncertainty. A [gene tree](../../../../gene-tree.md) need not equal the [species tree](../../../../species-tree.md), because [incomplete lineage sorting](../../../../incomplete-lineage-sorting.md), [genetic recombination](../../../../genetic-recombination.md) and [horizontal gene transfer](../../../../horizontal-gene-transfer.md) can produce different histories. Rooting with an appropriate [outgroup](../../../../outgroup.md) establishes ancestral direction; pairwise differences alone do not supply a root.

Branch lengths measured in substitutions per site are not yet calendar times. Under a [strict molecular clock](../../../../strict-molecular-clock.md) with rate $\mu$ per site per year, a branch of duration $t$ has length $\mu t$; two contemporaneously sampled descendants separated at time $t$ have total path length $d=2\mu t$, hence $\boxed{t=d/(2\mu)}$. Calibration comes from independently dated constraints such as [fossil calibration](../../../../fossil-calibration.md), geological information or sufficiently informative sampling dates. A dated common ancestor is not automatically identical in age to the earliest observed fossil. A [relaxed molecular clock](../../../../relaxed-molecular-clock.md) permits branch-specific rates while imposing a statistical model on them.

Without an external temporal calibration or an independently known rate, multiplying all times by a constant and dividing all rates by that constant leaves expected sequence divergence unchanged. Absolute dates are therefore unidentifiable from sequence divergence alone. A useful time-calibrated [phylogenetic tree](../../../../phylogenetic-tree.md) reports uncertainty from sequence sampling, substitution models, rate variation, topology and calibration bounds, rather than displaying an unjustified exact date for each ancestor.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
