<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $E_q$ be the event that all eight selected subjects carry two copies of the same specified ancestral copy $q$, and that no other generation-4 subject is [autozygous](../../../../../../autozygosity.md) at this [genetic locus](../../../../../../genetic-locus.md). The selected subjects occur in every sibship, so this event forces both generation-2 transmissions and all six relevant generation-3 transmissions. Applying the preceding conditional [probabilities](../../../../../../probability.md),

$$
P(E_q)=\frac14\frac1{64}\left(\frac14\right)^8\left(\frac34\right)^8
=\frac{3^8}{2^{40}}.
$$

Once all six parents carry $q$, their other copies come from the two unrelated outside [pedigree founders](../../../../../../founder-in-a-pedigree.md), one on each side of the [pedigree](../../../../../../pedigree.md). A child not receiving two $q$ copies therefore cannot become [autozygous](../../../../../../autozygosity.md) for a different founding copy. This verifies the “only” condition, rather than merely excluding [homozygosity](../../../../../../homozygosity.md) for $q$.

For the event $E$ without specifying which of the original four copies is shared, the four alternatives $E_q$ are disjoint: a selected child cannot simultaneously have both its copies descended from two different ancestral copies. Hence

$$
\boxed{P(E)=4P(E_q)=\frac{3^8}{2^{38}}.}
$$

All selected individuals are then [autozygous](../../../../../../autozygosity.md) for the same copy and mutually 2-IBD. The distinction from the $3/4$ [probability](../../../../../../probability.md) in the alternative interpretation of part (a) is precisely this disjointness.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
