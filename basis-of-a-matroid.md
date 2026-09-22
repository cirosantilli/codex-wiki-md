# Basis of a matroid

↑ **Parent:** [Matroid](matroid.md)

A [matroid basis](basis-of-a-matroid.md) is a [matroid independent set](independent-set-of-a-matroid.md) that is a [maximal element](maximal-element-of-a-partially-ordered-set.md) under inclusion of [subsets](subset.md): no additional element of the [ground set](ground-set.md) can be admitted. Maximum [cardinality](cardinality.md) means having the largest size among all [matroid independent sets](independent-set-of-a-matroid.md). Maximality tests whether this particular selection can grow; maximum size compares it with every selection. In a [matroid](matroid.md) the two conditions coincide, so all [matroid bases](basis-of-a-matroid.md) have a common size. They need not have equal weight. [Michel X. Goemans, Matroid optimization, section 5.1, p. 1, maximal independent sets and bases](matroid-optimization-by-michel-goemans.md)

**Proof outline.** If a maximal [matroid independent set](independent-set-of-a-matroid.md) $B$ were smaller than another [matroid independent set](independent-set-of-a-matroid.md) $J$, the [matroid independence axioms](matroid-independence-axioms.md) would admit an element of $J\setminus B$, contradicting maximality. Finiteness allows every [matroid independent set](independent-set-of-a-matroid.md) to grow to a [matroid basis](basis-of-a-matroid.md) by successive admissible additions. In a general [independence system](independence-system.md), maximal selections can have different sizes, as in the [hereditary nonmatroid greedy obstruction](hereditary-nonmatroid-greedy-obstruction.md).

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
