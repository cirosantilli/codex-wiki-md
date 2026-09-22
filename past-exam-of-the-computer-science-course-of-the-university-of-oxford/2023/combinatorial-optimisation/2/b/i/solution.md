<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On fixed labelled [ground sets](../../../../../../ground-set.md) of [cardinality](../../../../../../cardinality.md) $1,2,3$, the numbers of [matroids](../../../../../../matroid.md) are respectively **$2,5,16$**.

For one element, the element is either a [loop of a matroid](../../../../../../loop-of-a-matroid.md) or a [nonloop](../../../../../../nonloop-of-a-matroid.md), giving two choices. For two elements, [rank of a matroid](../../../../../../rank-of-a-matroid.md) zero and two each give one possibility. At [rank of a matroid](../../../../../../rank-of-a-matroid.md) one, the [nonloops](../../../../../../nonloop-of-a-matroid.md) form any nonempty [subset](../../../../../../subset.md), giving $2^2-1=3$ more possibilities: total $1+3+1=5$.

For three elements, classify by the total [rank of a matroid](../../../../../../rank-of-a-matroid.md). At [rank of a matroid](../../../../../../rank-of-a-matroid.md) zero every element is a [matroid loop](../../../../../../loop-of-a-matroid.md); at [rank of a matroid](../../../../../../rank-of-a-matroid.md) three every [subset](../../../../../../subset.md) is a [matroid independent set](../../../../../../independent-set-of-a-matroid.md). At [rank of a matroid](../../../../../../rank-of-a-matroid.md) one, choose any nonempty [subset](../../../../../../subset.md) of [nonloops](../../../../../../nonloop-of-a-matroid.md); exactly the [empty set](../../../../../../empty-set.md) and their [singletons](../../../../../../singleton-mathematics.md) are [matroid independent sets](../../../../../../independent-set-of-a-matroid.md). This gives seven possibilities.

At [rank of a matroid](../../../../../../rank-of-a-matroid.md) two, either exactly two elements are [nonloops](../../../../../../nonloop-of-a-matroid.md), giving three choices for the remaining [loop of a matroid](../../../../../../loop-of-a-matroid.md), or all three are [nonloops](../../../../../../nonloop-of-a-matroid.md). In the latter case, pairs that are [matroid dependent sets](../../../../../../dependent-set-of-a-matroid.md) define [parallel elements of a matroid](../../../../../../parallel-elements-of-a-matroid.md). There can be no such pair, giving the [uniform matroid](../../../../../../uniform-matroid.md) $U_{2,3}$, or exactly one such pair, giving three choices. There cannot be exactly two such pairs: if $\{a,b\}$ and $\{a,c\}$ were [matroid dependent sets](../../../../../../dependent-set-of-a-matroid.md) but $\{b,c\}$ a [matroid independent set](../../../../../../independent-set-of-a-matroid.md), augmentation from $\{a\}$ to $\{b,c\}$ would fail. If all three pairs were [matroid dependent sets](../../../../../../dependent-set-of-a-matroid.md), the [rank of a matroid](../../../../../../rank-of-a-matroid.md) would be one. Hence [rank of a matroid](../../../../../../rank-of-a-matroid.md) two gives $3+1+3=7$ examples.

Every listed possibility satisfies augmentation: the only nontrivial comparison on three elements is from a [singleton](../../../../../../singleton-mathematics.md) to a two-element [matroid independent set](../../../../../../independent-set-of-a-matroid.md), and with at most one two-element [matroid dependent set](../../../../../../dependent-set-of-a-matroid.md) at least one addition works. The total is therefore $1+7+7+1=16$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
