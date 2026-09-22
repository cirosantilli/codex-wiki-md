# Vertex-block concentration of maximum matching weight

↑ **Parent:** [McDiarmid's inequality](mcdiarmid-s-inequality.md)

Give a graph on $n$ labelled vertices independent edge weights in $[0,1]$, and let $W$ be the maximum total weight of a [matching](matching-graph-theory-split.md). Put each edge into the block of its lower-numbered endpoint. There are at most $n-1$ independent blocks. Every matching uses at most one edge from any block, since the block's edges share that endpoint. Changing a whole block therefore changes the weight of each fixed matching by at most one. Comparing the old and new maximizing matchings shows the same bound for $W$.

The Doob exposure [martingale](martingale-split.md) for these blocks has increments bounded by one, so [Azuma's inequality](azuma-s-inequality.md) gives

$$
P(|W-EW|\ge t)\le2\exp\left(-\frac{t^2}{2(n-1)}\right),\qquad n\ge2.
$$

The important feature is grouping independent edge coordinates into vertex-centred blocks. Exposing all edges separately would give a weaker denominator of order $n^2$ on a dense graph. Identical distributions are unnecessary; independence and the common range bound suffice.

## ↑ Ancestors (9)

1. [McDiarmid's inequality](mcdiarmid-s-inequality.md)
2. [Bounded differences property](bounded-differences-property.md)
3. [Concentration inequality](concentration-inequality.md)
4. [Probability inequality](probability-inequality-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2007/b/8/d/solution.md)
