# Partition regularity of IP sets

↑ **Parent:** [IP set](ip-set.md)

Every [finite coloring](finite-coloring.md) of an [IP set](ip-set.md) has a color class that is an [IP set](ip-set.md). Here is a reduction to the ordinary [Hindman theorem](hindman-theorem.md). Given $\operatorname{FS}(x_i)$ in the original set, color an integer $n>0$ by the color of $\sum_{i\in\operatorname{supp}_2(n)}x_i$, where the support consists of positions of its nonzero digits in the [binary expansion](binary-expansion.md). The [Hindman theorem](hindman-theorem.md) produces $w_i>0$ with [monochromatic](monochromatic-set.md) $\operatorname{FS}(w_i)$. Replace the $w_i$ by consecutive, disjoint finite block sums $v_j$ with separated binary supports: after a block has been chosen, take $K$ above all previously used positions; two of $2^K+1$ partial sums of a fresh tail agree modulo $2^K$, so their positive difference supplies the next block sum divisible by $2^K$. Now binary addition of distinct $v_j$ has no carries. Therefore $y_j=\sum_{i\in\operatorname{supp}_2(v_j)}x_i$ generates a [monochromatic](monochromatic-set.md) [finite-sums set](finite-sums-set.md) in the original IP set.

## ↑ Ancestors (8)

1. [IP set](ip-set.md)
2. [Finite-sums set](finite-sums-set.md)
3. [Hindman theorem](hindman-theorem.md)
4. [Ramsey theory](ramsey-theory-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [IP set](ip-set.md)
- [IP-star filter](ip-star-filter.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-9/3/solution.md)
