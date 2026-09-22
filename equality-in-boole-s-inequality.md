<h1 id="equality-in-boole-s-inequality">Equality in Boole's inequality</h1>

↑ **Parent:** [Boole's inequality](boole-s-inequality.md)

For finitely many [events](event.md), or a [countable](countable-set.md) family with finite sum of individual [probabilities](probability.md), equality in the uncapped [union bound](boole-s-inequality.md) holds exactly when every pairwise [intersection](set-intersection.md) has [probability](probability.md) zero. Equivalently, at most one [event](event.md) occurs [almost surely](almost-sure-convergence.md). Pairwise [disjoint events](disjoint-events.md) give equality, but literal disjointness is stronger than necessary: shared outcomes of [probability](probability.md) zero do not change either side. For the capped bound, if the sum exceeds one, equality instead means that the [union](set-union.md) is an [almost sure event](almost-sure-event.md); overlap can then have positive [probability](probability.md).

The cap and the disjoint case are both sharp. If the individual [probabilities](probability.md) sum to at most one, put the [events](event.md) on separate pieces of a [sample space](sample-space.md) to attain their sum. The twelve-outcome disjoint example does this with two [events](event.md) of [probability](probability.md) $1/3$. If the sum exceeds one, a covering [union](set-union.md) can attain the cap: on the same twelve-outcome [sample space](sample-space.md), $A=\{1,\ldots,8\}$ and $B=\{5,\ldots,12\}$ have sum $4/3$ and exact [union](set-union.md) [probability](probability.md) one. These are sharpness examples, not an assertion that every overlapping family attains the bound. Positive-[probability](probability.md) [disjoint events](disjoint-events.md) are also not [independent events](independent-events.md), because their joint [probability](probability.md) is zero while the product of their individual [probabilities](probability.md) is positive.

## ↑ Ancestors (7)

1. [Boole's inequality](boole-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Overlap in the union bound](overlap-in-the-union-bound.md)
