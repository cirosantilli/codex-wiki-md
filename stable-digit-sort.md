# Stable digit sort

↑ **Parent:** [Radix sort](radix-sort.md)

A [stable digit sort](stable-digit-sort.md) applies [stable sorting](stable-sorting.md) to complete [sorting records](sorting-record.md) using one specified [numerical digit](numerical-digit.md) of their encoded [sort keys](sort-key.md). [Counting sort](counting-sort.md) can supply it; [stable record placement in counting sort](stable-record-placement-in-counting-sort.md) moves records without discarding their associated data. Stability concerns equal current [numerical digits](numerical-digit.md), even when the full [sort keys](sort-key.md) differ. This is the information-preservation step in [least-significant-digit radix sort](least-significant-digit-radix-sort.md).[Open Data Structures: An Introduction by Pat Morin; §11.2.1, associated-data and stability paragraphs; §11.2.2, least-significant passes and correctness paragraph after Figure 11.8](open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort.md)

An original two-record counterexample exposes the need for the tie rule. Start with $(42_A,41_B)$ at width three. A units pass gives $(041_B,042_A)$. Both tens [numerical digits](numerical-digit.md) are four. A deliberately unstable tens pass may reverse their tie and return $(042_A,041_B)$: it is sorted by the tens [numerical digit](numerical-digit.md), yet its two-position suffixes $42,41$ are decreasing. The final stable hundreds pass sees two zeros and keeps this wrong order. [Sorting permutation preservation](sorting-permutation-preservation.md) still holds, but [sortedness](sortedness.md) fails. Stability in the tens pass would have retained the units information.

With [counting sort](counting-sort.md) as the [stable digit sort](stable-digit-sort.md), each pass initializes $R$ counters, counts $n$ current [numerical digits](numerical-digit.md), constructs their [prefix sums](prefix-sum.md), and places $n$ complete [sorting records](sorting-record.md). Thus each pass costs $O(n+R)$, and $d$ passes cost $O(d(n+R))$ in [Big O notation](big-o-notation.md). Reuse the counters and two [arrays](array-data-structure.md) of record references between passes: auxiliary [space complexity](space-complexity.md) is $O(n+R)$, rather than $O(d(n+R))$. Assume constant-cost [numerical digit](numerical-digit.md) extraction, counter [arithmetic](arithmetic-split.md), [array](array-data-structure.md) indexing and record-reference movement; the bound counts these operations, not the cost of copying arbitrarily large payloads or performing arbitrary-precision [integer arithmetic](integer-arithmetic.md).

The benefit is avoiding a counter for every possible whole [sort key](sort-key.md): width $d$ has $R^d$ possibilities, while each pass needs only $R$ counters. A larger [radix](radix.md) reduces the number of passes for a fixed key range but enlarges the counter [array](array-data-structure.md). The [comparison sorting lower bound](comparison-sorting-lower-bound.md) does not apply to these direct [array indices](array-index.md); they reveal more than a two-way comparison. Nor does fixing $R$ make $d$ disappear: growing key width still increases work.

## ↑ Ancestors (5)

1. [Radix sort](radix-sort.md)
2. [Sorting algorithm](sorting-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Radix sort suffix invariant](radix-sort-suffix-invariant.md)
- [Stable digit sort](stable-digit-sort.md)
