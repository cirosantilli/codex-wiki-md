<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Five consequences of the [ancestral recombination graph](../../../../../../ancestral-recombination-graph.md) are:

- **[Linkage disequilibrium](../../../../../../linkage-disequilibrium.md) and its distance dependence.** Nearby sites often inherit the same local genealogy, so [mutations](../../../../../../mutation.md) on their shared ancestral branches produce correlated [alleles](../../../../../../allele.md). The chance of an ancestral breakpoint between sites increases with their genetic distance, reducing shared genealogy and, on average, [linkage disequilibrium](../../../../../../linkage-disequilibrium.md). This gives the genealogical explanation of the two-locus decay calculation.
- **[Haplotype blocks](../../../../../../haplotype-block.md) and [recombination hotspots](../../../../../../recombination-hotspot.md).** With a varying recombination map, the [ARG](../../../../../../ancestral-recombination-graph.md) has relatively few breakpoints within low-recombination regions and many near [recombination hotspots](../../../../../../recombination-hotspot.md). Long intervals can consequently retain a small number of common ancestral [haplotypes](../../../../../../haplotype.md), while genealogical relationships change more frequently across the intervening regions. This explains why LD blocks are heterogeneous rather than equally spaced units.
- **Mosaic inheritance and shared ancestral tracts.** Backward splits assign different pieces of one contemporary [chromosome](../../../../../../chromosome.md) to different ancestral [chromosomes](../../../../../../chromosome.md). Two sampled [chromosomes](../../../../../../chromosome.md) can therefore share a recent ancestor over one interval but not its neighbors. For a specified total of $m$ independent ancestral [meioses](../../../../../../meiosis.md), a tract of genetic length $d$ has approximately $md$ expected crossovers under a Poisson crossover model, so its [probability](../../../../../../probability.md) of remaining intact is $e^{-md}$. This relates long [IBD segments](../../../../../../identical-by-descent-segment.md) to recent common ancestry, while distinguishing tract-boundary sampling from length-biased sampling at a random genomic point.
- **Incompatible site patterns and four observed gametes.** Under an [infinite sites mutation model](../../../../../../infinite-sites-mutation-model.md) on a single rooted tree, the descendant sets of two [mutations](../../../../../../mutation.md) are nested or disjoint. They cannot cross, so all four [haplotypes](../../../../../../haplotype.md) $00,01,10,11$ cannot occur. Recombination permits different local trees: one site's derived clade can be $\{10,11\}$ and the other's $\{01,11\}$, producing all four without repeated [mutation](../../../../../../mutation.md). The [four-gamete test](../../../../../../four-gamete-test.md) therefore detects a failure of the unrecombined, single-mutation-per-site model. Recurrent [mutation](../../../../../../mutation.md) would be an alternative explanation if the infinite-sites assumption were dropped.
- **Variation in local diversity and [allele](../../../../../../allele.md) frequencies.** Coalescent mergers describe [genetic drift](../../../../../../genetic-drift.md); their random times produce different branch lengths and descendant-group sizes. Recombination makes these genealogies vary along the [chromosome](../../../../../../chromosome.md). Conditional on a local genealogy, its [segregating site](../../../../../../segregating-site.md) count is Poisson with [mean](../../../../../../expected-value.md) $\theta L/2$, so a longer tree tends to contain more variants. A [mutation](../../../../../../mutation.md) on a branch subtending $j$ of the $n$ samples appears at sample frequency $j/n$. Together, random branch lengths, descendant counts and [mutations](../../../../../../mutation.md) explain heterogeneous local diversity and the distribution of [allele](../../../../../../allele.md) frequencies without requiring selection.

<a id="4/v/image-different-local-genealogies-can-generate-all-four-haplotypes-with-one-mutation-per-site"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45-recombination-genealogies.png)

**[Figure 1](#4/v/image-different-local-genealogies-can-generate-all-four-haplotypes-with-one-mutation-per-site). Different local genealogies can generate all four haplotypes with one mutation per site**.

**Shared ancestry explains [correlation](../../../../../../pearson-correlation-coefficient.md); recombination makes ancestry a mosaic; [mutation](../../../../../../mutation.md) on the resulting branches converts genealogy into observed variation.** These explanations use the neutral ARG, with a variable recombination map where stated. Selection, population subdivision or changing population size can also be studied genealogically, but require extending the event model rather than being consequences of the constant-size panmictic neutral process alone.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
