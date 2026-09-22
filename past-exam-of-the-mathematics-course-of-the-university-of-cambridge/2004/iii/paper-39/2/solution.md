<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Linkage disequilibrium](../../../../../linkage-disequilibrium.md) means that [alleles](../../../../../allele.md) at different [genetic loci](../../../../../genetic-locus.md) are associated in population [haplotypes](../../../../../haplotype.md). For two biallelic loci,

$$
D=p_{AB}-p_Ap_B,\qquad r^2=\frac{D^2}{p_A(1-p_A)p_B(1-p_B)}.
$$

The first quantity measures departure from independent allele frequencies; the second is the squared [allelic correlation](../../../../../allelic-correlation.md). [Standardized linkage disequilibrium](../../../../../standardized-linkage-disequilibrium.md) $D'$ instead compares $D$ to its possible range at the given frequencies. High $|D'|$ can coexist with low $r^2$, so it need not make one [genetic marker](../../../../../genetic-marker.md) a good predictor of another. [Genetic linkage](../../../../../genetic-linkage.md) is a different notion: it describes within-family transmission and the [recombination fraction](../../../../../recombination-fraction.md).

The chromosome-21 study of [Patil and colleagues, Science 2001](https://pubmed.ncbi.nlm.nih.gov/11721056/) found consecutive [single-nucleotide polymorphisms](../../../../../single-nucleotide-polymorphism.md) organized into regions with comparatively few common [haplotypes](../../../../../haplotype.md); typically three haplotypes accounted for over 80% of the sampled chromosomes within a block. Such [haplotype blocks](../../../../../haplotype-block.md) can be represented efficiently by [tag SNPs](../../../../../tag-snp.md). Strong association within blocks and weaker association across boundaries give a useful description, though block boundaries depend on allele frequencies, population history, sampling and the operational definition of a block. They do not divide chromosomes into regions where [genetic recombination](../../../../../genetic-recombination.md) is respectively impossible and certain.

The ancestry explanation uses an [ancestral recombination graph](../../../../../ancestral-recombination-graph.md). Going backwards, ancestral lineages coalesce, while a [genetic recombination](../../../../../genetic-recombination.md) event splits one lineage's ancestral material into contributions from two parents. At a fixed genomic position, retaining only its ancestry gives a [phylogenetic tree](../../../../../phylogenetic-tree.md) with the appropriate coalescent law. Nearby positions often retain much of the same tree; mutations on shared branches then produce correlated allele states. Breakpoints can change the local tree, weakening that shared history.

Under a simple random-mating two-locus model, [linkage-disequilibrium decay under recombination](../../../../../linkage-disequilibrium-decay-under-recombination.md) gives $D_{t+1}=(1-r)D_t$. Actual populations also undergo [genetic drift](../../../../../genetic-drift.md), [population bottlenecks](../../../../../population-bottleneck.md), [mutation](../../../../../mutation.md) and migration, which can create or preserve association. Recombination rates themselves vary along chromosomes: [McVean and colleagues, Science 2004](https://pubmed.ncbi.nlm.nih.gov/15105499/) inferred strong local variation from sequence data. These observations motivate an ancestry model with spatially varying recombination, rather than treating physical distance as the only determinant of [linkage disequilibrium](../../../../../linkage-disequilibrium.md).

For fine mapping, a typed [genetic marker](../../../../../genetic-marker.md) can show [genetic association](../../../../../genetic-association.md) because it is correlated with a nearby causal [genetic variant](../../../../../genetic-variant.md). [Linkage-disequilibrium marker tagging](../../../../../linkage-disequilibrium-marker-tagging.md) makes a sparse first-stage scan possible, but several variants in one block can produce nearly indistinguishable association patterns. Historical recombination and diverse local genealogies can narrow the interval when denser genotyping is available.

An [ancestral recombination graph](../../../../../ancestral-recombination-graph.md) turns that intuition into a likelihood calculation. One can place a proposed disease-origin event on a local ancestral branch and integrate over possible graphs, mutation histories and unobserved [haplotypes](../../../../../haplotype.md). The local [phylogenetic tree](../../../../../phylogenetic-tree.md) then relates disease-bearing chromosomes and predicts which markers should remain associated. In a [Bayesian inference](../../../../../bayesian-statistics.md), uncertainty in ancestry, mutation location and demographic parameters enters the [posterior distribution](../../../../../bayesian-posterior.md) rather than being replaced by one guessed tree. Whole-graph inference is computationally demanding, and approximate or pairwise methods often supply practical estimates.

The useful distinction is between finding an associated region and identifying its causal variant. Strong [linkage disequilibrium](../../../../../linkage-disequilibrium.md) improves marker coverage but can limit resolution inside the associated region. [Population stratification](../../../../../population-stratification.md), ascertainment, rare variants and misspecified population history can also mislead an association analysis. Combining fine mapping with independent biological evidence is therefore stronger than interpreting an association peak as proof of causation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
