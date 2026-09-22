<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Maximum [likelihood](../../../../likelihood-function.md) and Bayesian phylogenetics can use the same model of sequence [evolution](../../../../evolution.md), but they answer different inferential questions: optimization of the [likelihood](../../../../likelihood-function.md) versus a posterior distribution over trees and other unknowns.** Let $D$ be a [sequence alignment](../../../../sequence-alignment.md), $T$ a [phylogenetic tree](../../../../phylogenetic-tree.md) topology, $\mathbf b$ its branch lengths in expected substitutions per site, and $\theta$ the parameters of a [nucleotide substitution model](../../../../nucleotide-substitution-model.md). Both methods can use

$$
L(T,\mathbf b,\theta)=P(D\mid T,\mathbf b,\theta).
$$

The [likelihood function](../../../../likelihood-function.md) sums over unobserved ancestral states, rather than choosing one ancestral sequence and treating it as observed. For conditionally independent sites it is a product of site likelihoods; transitions along a branch can be described by the [matrix exponential](../../../../matrix-exponential.md) $e^{Qb}$ of a [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md) rate matrix $Q$. The [phylogenetic pruning algorithm](../../../../phylogenetic-pruning-algorithm.md) computes the ancestral sums efficiently.[Journal of Molecular Evolution 17, pp. 368–376; likelihood calculation by summing over ancestral states](../../../../evolutionary-trees-from-dna-sequences-a-maximum-likelihood-approach-by-joseph-felsenstein.md)

With [maximum likelihood estimation](../../../../maximum-likelihood-estimation-split.md), one seeks

$$
(\widehat T,\widehat{\mathbf b},\widehat\theta)\in\arg\max_{T,\mathbf b,\theta}L(T,\mathbf b,\theta).
$$

In practice, the enormous discrete tree space requires searches and repeated optimization of continuous parameters; heuristic failure to find the best tree is a computational error distinct from statistical uncertainty. A tree's optimized [likelihood](../../../../likelihood-function.md) is not the [probability](../../../../probability.md) that it is correct. [bootstrap](../../../../bootstrapping-statistics.md) analyses resample alignment columns and repeat inference to assess support under the resampling procedure; their frequencies are not automatically [posterior probabilities](../../../../posterior-probability.md). Independence assumptions matter, because linked sites and heterogeneous loci can make simple column resampling an imperfect representation of replication.

In [Bayesian phylogenetic inference](../../../../bayesian-phylogenetic-inference.md),

$$
p(T,\mathbf b,\theta\mid D)=\frac{P(D\mid T,\mathbf b,\theta)\,\pi(T,\mathbf b,\theta)}{P(D)}.
$$

The [prior distribution](../../../../prior-probability.md) supplies weights on topologies, branch lengths and model parameters. Integrating over nuisance parameters gives

$$
P(T\mid D)\propto\int L(T,\mathbf b,\theta)\pi(T,\mathbf b,\theta)\,d\mathbf b\,d\theta.
$$

Thus a very narrow [likelihood](../../../../likelihood-function.md) peak can lose posterior support to a broader region with a slightly lower maximum. [maximum a posteriori estimation](../../../../maximum-a-posteriori-estimation.md) is another optimization and does not replace this integration. [Markov chain Monte Carlo](../../../../markov-chain-monte-carlo.md) provides dependent samples approximating the [posterior distribution](../../../../bayesian-posterior.md); a clade's [posterior probability](../../../../posterior-probability.md) is the posterior mass of trees containing that clade. The early likelihood-based Bayesian formulation explicitly distinguished these probabilities from bootstrap support.[Journal of Molecular Evolution 43, pp. 304–311; posterior probabilities of trees and comparison with bootstrap proportions](../../../../probability-distribution-of-molecular-evolutionary-trees-a-new-method-of-phylogenetic-inference-by-bruce-rannala-and-ziheng-yang.md)

Neither approach is protected against systematic error. Poor [sequence alignment](../../../../sequence-alignment.md), incorrect [orthology](../../../../orthology.md) assignments, compositionally heterogeneous sequences, and an inadequate substitution process can support a wrong tree with high apparent confidence. A [gene tree](../../../../gene-tree.md) can differ from a [species tree](../../../../species-tree.md) because of [incomplete lineage sorting](../../../../incomplete-lineage-sorting.md) or [introgression](../../../../introgression.md); extra sequence from that [gene](../../../../gene.md) does not automatically fix the mismatch. Model comparison, biological examination of the data and sensitivity to locus sampling are needed in both approaches. In Bayesian analyses, agreement among short chains is not proof of convergence: independent runs, adequate mixing between topologies and an appropriate [effective sample size of a Markov chain](../../../../effective-sample-size-of-a-markov-chain.md) should be checked. A [credible interval](../../../../credible-interval.md) and a [confidence interval](../../../../confidence-interval.md) also have different interpretations even if their numerical endpoints happen to resemble one another.

Time inference adds a particularly strong role for assumptions. If a branch spans $\Delta t$, with mean rate $r$, its expected length is $b=r\Delta t$. Without an external absolute-time anchor, scaling every time by $c$ and every rate by $1/c$ [leaves](../../../../leaf.md) the sequence [likelihood](../../../../likelihood-function.md) unchanged. Even a very long alignment can identify branch lengths accurately without identifying an absolute calendar scale. For example, a lineage length $b=0.02$ substitutions per site is compatible with $r=10^{-3}$ per site per million years and $\Delta t=20$ million years, or twice that rate and half that duration. This is an [identifiability](../../../../identifiability.md) issue, not merely a shortage of sampled bases.

In [Bayesian divergence-time inference](../../../../bayesian-divergence-time-inference.md), a schematic joint analysis is

$$
p(T,\mathbf t,\mathbf r,\theta\mid D,F)\propto
P(D\mid T,\mathbf t,\mathbf r,\theta)\,
\pi(T,\mathbf t,\mathbf r,\theta\mid F),
$$

where $F$ is fossil information already used to construct the conditional prior. An alternative generative analysis includes a fossil-sampling [likelihood](../../../../likelihood-function.md) explicitly; the same fossil evidence must not be counted twice. A [strict molecular clock](../../../../strict-molecular-clock.md) equates rates across branches; a [relaxed molecular clock](../../../../relaxed-molecular-clock.md) allows variation, whose distribution and correlations also require specification. A narrow rate prior favors particular absolute ages, and a strong rate-smoothing assumption can redistribute inferred time among branches. A [birth-death process](../../../../birth-death-process.md) prior on the tree encodes assumptions about lineage origination, extinction and sampling; it is not a neutral choice just because it is mathematically convenient.

[fossil calibration](../../../../fossil-calibration.md) must separate a fossil's geological age from the age of the lineage split it constrains. A confidently placed crown fossil gives a minimum age for the relevant crown, whereas a stem fossil does not automatically set that crown minimum. Uncertain placement and the incompleteness of the record complicate upper bounds. [hard calibration bounds](../../../../hard-calibration-bound.md) assign zero probability outside the permitted range; enough sequence cannot overcome a zero prior. [soft calibration bounds](../../../../soft-calibration-bound.md) allow small tail probabilities, exposing rather than eliminating the possibility of conflict. Multiple-calibration analyses demonstrate that changing the treatment of bounds changes inferred times and uncertainty.[Molecular Biology and Evolution 23, pp. 212–226; hard versus soft bounds and the divergence-time prior](../../../../bayesian-estimation-of-species-divergence-times-under-a-molecular-clock-using-multiple-fossil-calibrations-with-soft-bounds-by-ziheng-yang-and-bruce-rannala.md)

Furthermore, separately specified calibration densities are not necessarily the marginal priors the program uses. The rule that an ancestor must be older than its descendant truncates their joint possibilities. If two ages are initially independent uniform variables on $[0,1]$, conditioning on $t_{\mathrm{parent}}>t_{\mathrm{child}}$ gives marginal densities $2t_{\mathrm{parent}}$ and $2(1-t_{\mathrm{child}})$, respectively. Neither remains uniform. Combining tree-process priors, calibration densities and ordering constraints can therefore introduce substantial information unintentionally.[Sections on node ordering and the realized joint prior; recommendation to sample the prior with a fixed likelihood](../../../../conceptual-issues-in-bayesian-divergence-time-estimation-by-bruce-rannala.md)

The practical response is to run the analysis without sequence information to inspect the effective [prior distribution](../../../../prior-probability.md), then compare it with the [posterior distribution](../../../../bayesian-posterior.md). Repeat under defensible calibration tails, rate models, tree priors and fossil placements; report which ages change and whether the data sharpen relative ages more than absolute ages. Examine [prior predictive checks](../../../../prior-predictive-check.md) and [posterior predictive checks](../../../../posterior-predictive-check.md), and keep numerical mixing diagnostics separate from biological model adequacy. **Priors can legitimately supply the time information missing from sequences, but narrow posterior ages are persuasive only when that information and its sensitivity are explicit.**

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper plm3](../../paper-plm3-split.md)
3. [2025](../../split.md)
4. [Past exam of the plant Sciences course of the University of Cambridge](../../../split.md)
5. [Plant Sciences course of the University of Cambridge](../../../../plant-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
