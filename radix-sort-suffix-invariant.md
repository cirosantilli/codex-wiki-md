# Radix sort suffix invariant

↑ **Parent:** [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)

After $p$ passes, $0\le p\le d$, the [array](array-data-structure.md) is in nondecreasing order of $s_p(k)=k\bmod R^p$, the [integer](integer-split.md) represented by its $p$ lowest [numerical digits](numerical-digit.md). Equivalently it is ordered by the [tuple](finite-tuple.md) $(\delta_{p-1}(k),\ldots,\delta_0(k))$ under [lexicographic order](lexicographic-order.md), with the most significant processed [numerical digit](numerical-digit.md) first. Among equal suffixes it retains the original order of the complete [sorting records](sorting-record.md).

The [loop invariant](loop-invariant.md) has a simple [mathematical induction](mathematical-induction.md) proof. Before any pass, $s_0(k)=k\bmod1=0$ for every [sort key](sort-key.md), so the original [array](array-data-structure.md) satisfies it. Suppose it holds after $p$ passes. The next [stable digit sort](stable-digit-sort.md) puts smaller $\delta_p$ groups first and preserves the existing $s_p$ order within each tie. Since

$$
s_{p+1}(k)=R^p\delta_p(k)+s_p(k),\qquad 0\le s_p(k)<R^p,
$$

the new [array](array-data-structure.md) is ordered by $s_{p+1}$. Equal new suffixes have equal current [numerical digits](numerical-digit.md) and equal old suffixes, so their original order is also preserved. Every pass is a [permutation](permutation.md) of complete [sorting records](sorting-record.md), establishing [sorting permutation preservation](sorting-permutation-preservation.md). At termination $p=d$, the assumption $k<R^d$ gives $s_d(k)=k$: the invariant becomes whole-key [sortedness](sortedness.md), together with [stable sorting](stable-sorting.md).

## ↑ Ancestors (6)

1. [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
2. [Radix sort](radix-sort.md)
3. [Sorting algorithm](sorting-algorithm.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
