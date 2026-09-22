<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

An [ancestral recombination graph](../../../../../../ancestral-recombination-graph.md), or [ARG](../../../../../../ancestral-recombination-graph.md), is the directed ancestry of a sample of chromosomal segments when ancestral lineages can both coalesce and undergo [genetic recombination](../../../../../../genetic-recombination.md). It records which ancestral material each lineage carries, the times of events and the recombination breakpoints. At any fixed genomic position, following only the ancestral material at that position gives a marginal [phylogenetic tree](../../../../../../phylogenetic-tree.md). Different positions can have different trees, while sharing substantial parts of their history. The graph is acyclic in time, although its underlying undirected graph can have loops because a lineage splits backwards and its ancestors can later rejoin.

For the standard neutral, constant-size, randomly mating diploid model, measure time in $2N_e$ generations and set $\rho=4N_e r$, where $r$ is the recombination rate across the whole segment. The backward process is a continuous-time [Markov jump process](../../../../../../markov-jump-process.md) on collections of lineages carrying ancestral material:

- Each unordered pair of current lineages coalesces at rate one. The parent lineage carries the union of their ancestral material, with common ancestry recorded at overlapping positions. With $k$ lineages the total coalescence rate is $\binom k2$. The full ARG permits a pair to merge even when its carried material is disjoint; such an event creates no merger in a local tree at that instant.
- A lineage splits into two parental lineages at a recombination breakpoint. With a uniform recombination map on a segment of normalized length one, the intensity of breakpoints along a fully ancestral lineage is $\rho/2$ per unit length. If a lineage carries only part of the segment, only cuts leaving ancestral material on both sides need be retained, giving rate $(\rho/2)b_i$, where $b_i$ is the span between its leftmost and rightmost ancestral positions. Material to the left goes to one parent and material to the right to the other. A gap within that span still permits a cut that separates two carried pieces.

For a state with $k$ lineages, independent exponential event clocks give total rate

$$
R=\binom k2+\frac\rho2\sum_{i=1}^k b_i.
$$

The next waiting time has [exponential distribution](../../../../../../exponential-distribution.md) with rate $R$; choose its event type in proportion to the corresponding rate. A coalescing pair is uniform among unordered pairs; a recombining lineage is selected with weight $b_i$ and its breakpoint is uniform over its active span. With a nonuniform genetic map, use the corresponding integrated intensity and map-weighted breakpoint distribution. Initially all sample lineages span the whole segment, so the initial rate is $\binom n2+n\rho/2$. Ancestral material no longer needed after its sample copies have found their local common ancestor can be pruned.

[Mutations](../../../../../../mutation.md) are placed independently on the resulting ancestral branches, with local rate $\theta/2$ in coalescent units for a locus having scaled [mutation](../../../../../../mutation.md) parameter $\theta$. Without recombination, the graph reduces to a single [Kingman's coalescent](../../../../../../kingman-s-coalescent.md) tree. With recombination, each individual locus still has that marginal coalescent distribution, but trees at different loci are dependent. **The ARG combines backward pairwise mergers with backward recombination splits; local trees are its position-specific projections.** The neutral two-locus construction is developed in [Hudson's two-locus model](https://home.uchicago.edu/~rhudson1/twolocus.pdf).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
