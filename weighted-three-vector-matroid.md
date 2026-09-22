# Weighted three-vector matroid

↑ **Parent:** [Linear matroid](linear-matroid.md)

Take labels $E=\{a,b,c\}$ and [vectors](vector.md) in the [real vector space](real-vector-space.md) $\mathbb R^2$:

$$
v_a=(1,0),\qquad v_b=(0,1),\qquad v_c=(1,1),
\qquad w(a)=8,\quad w(b)=5,\quad w(c)=6.
$$

Here is the complete independence check for all eight [subsets](subset.md). The [empty set](empty-set.md) is independent. Each of $\{a\},\{b\},\{c\}$ is independent because its [vector](vector.md) is nonzero. Every pair is independent: the [determinants](determinant.md) of the two-column [matrices](matrix.md) $[v_a\ v_b]$, $[v_a\ v_c]$, and $[v_b\ v_c]$ are respectively $1$, $1$, and $-1$. The triple is dependent because $v_c-v_a-v_b=0$. Therefore

$$
\mathcal I=\{\varnothing,\{a\},\{b\},\{c\},
\{a,b\},\{a,c\},\{b,c\}\}.
$$

Deleting elements from any listed [subset](subset.md) stays in this list, verifying heredity. Every exchange comparison has sizes $(0,1)$, $(0,2)$, or $(1,2)$. From the [empty set](empty-set.md), any element of the larger [matroid independent set](independent-set-of-a-matroid.md) works: this covers three singleton targets and three pair targets. From any singleton to any pair, every element of the pair outside the singleton works, since every resulting pair is independent. This covers all nine singleton-pair comparisons, including disjoint ones. There are no other comparisons: all fifteen ordered size-increasing pairs satisfy exchange.

<a id="image-three-vectors-have-three-independent-pairs-and-one-dependent-triple-the-heaviest-matroid-basis-is-a-c-with-weight-14"></a>
![](matroid-three-vector-independence.png)

**[Figure 3](#image-three-vectors-have-three-independent-pairs-and-one-dependent-triple-the-heaviest-matroid-basis-is-a-c-with-weight-14). Three vectors have three independent pairs and one dependent triple; the heaviest matroid basis is $\{a,c\}$ with weight $14$**.

The three [matroid bases](basis-of-a-matroid.md) are $\{a,b\}$, $\{a,c\}$, and $\{b,c\}$, all of [cardinality](cardinality.md) two, with weights $13$, $14$, and $11$. The [matroid greedy algorithm](matroid-greedy-algorithm.md) considers $a$, then $c$, then $b$: it admits $a$, admits $c$ because their [determinant](determinant.md) is nonzero, and rejects $b$ because the triple is dependent. The resulting [matroid basis](basis-of-a-matroid.md) $\{a,c\}$ has weight $8+6=14$, the largest of the three totals. Every singleton can grow, so none is maximal; the three pairs are both maximal and maximum in [cardinality](cardinality.md).

## ↑ Ancestors (6)

1. [Linear matroid](linear-matroid.md)
2. [Matroid](matroid.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Graphic matroid](graphic-matroid.md)
- [Matroid](matroid.md)
- [Matroid greedy algorithm](matroid-greedy-algorithm.md)
- [Rank of a matroid](rank-of-a-matroid.md)
