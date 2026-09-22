# Matroid greedy algorithm

↑ **Parent:** [Matroid](matroid.md)

Assign each element of the finite [ground set](ground-set.md) a [real number](real-number.md) $w(e)$. The [matroid greedy algorithm](matroid-greedy-algorithm.md) sorts elements by nonincreasing weight, starts with the [empty set](empty-set.md), and admits an element exactly when the enlarged selection is a [matroid independent set](independent-set-of-a-matroid.md). Ties can be resolved arbitrarily. After all elements have been considered, the result is a [matroid basis](basis-of-a-matroid.md) of maximum total weight among all [matroid bases](basis-of-a-matroid.md). This holds even with negative weights: the task is to produce a full [matroid basis](basis-of-a-matroid.md). [Michel X. Goemans, Matroid optimization, section 5.2, pp. 5–6, greedy procedure and theorem 5.2](matroid-optimization-by-michel-goemans.md)

Maximizing weight over all [matroid independent sets](independent-set-of-a-matroid.md) is a different task when weights can be negative. For that task, skip negative elements; zero-weight additions are optional. With weights $w(a)=8$, $w(c)=-1$, $w(b)=-2$ in the [weighted three-vector matroid](weighted-three-vector-matroid.md), the heaviest [matroid basis](basis-of-a-matroid.md) is $\{a,c\}$ with weight $7$, while the heaviest [matroid independent set](independent-set-of-a-matroid.md) is $\{a\}$ with weight $8$. For nonnegative weights, every [matroid independent set](independent-set-of-a-matroid.md) can be extended to a [matroid basis](basis-of-a-matroid.md) without reducing weight, so the optimum values coincide.

**Proof outline.** Let $g_1,\ldots,g_r$ be the admitted elements in order, and order any competing [matroid basis](basis-of-a-matroid.md) $b_1,\ldots,b_r$ by nonincreasing weight. If $w(b_k)>w(g_k)$, exchange would let one of $b_1,\ldots,b_k$ augment $\{g_1,\ldots,g_{k-1}\}$. That element was considered before $g_k$ and, by heredity, was admissible even at that earlier stage, a contradiction. Hence $w(g_k)\geq w(b_k)$ for every $k$, and summing proves optimality. Rejected elements remain inadmissible as the selection grows, by heredity, so the final selection is maximal. The guarantee depends on the [matroid independence axioms](matroid-independence-axioms.md) and on weights adding independently across elements; interactions between chosen elements are a different objective.

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Graphic matroid](graphic-matroid.md)
- [Hereditary nonmatroid greedy obstruction](hereditary-nonmatroid-greedy-obstruction.md)
- [Matroid](matroid.md)
- [Matroid greedy algorithm](matroid-greedy-algorithm.md)
- [Weighted three-vector matroid](weighted-three-vector-matroid.md)
