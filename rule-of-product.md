# Rule of product

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rule_of_product)

For finite [sets](set-split.md), the number of ordered choices of one element from each is the product of the individual numbers of choices. More generally, if stage $j$ has exactly $n_j$ possible choices after every permitted history of earlier stages, the total number of full choice sequences is $\prod_j n_j$, by [mathematical induction](mathematical-induction.md) on the stages. This counts $b^a$ [functions](function-split.md) between sets of sizes $a,b$, and counts the [injective functions](injective-function.md) by the [falling factorial](falling-factorial.md) $b(b-1)\cdots(b-a+1)$ when $a\le b$.

With five people, choose a captain in five ways and a different deputy in four ways: **$5\cdot4=20$ ordered assignments**. The second choice depends on the first because the captain is excluded, but its number of permitted options is always four. The [rule of product](rule-of-product.md) therefore applies without any assumption about [independent events](independent-events.md). To count two-person teams instead, each [subset](subset.md) has two possible role assignments, so division by $2!=2$ gives ten teams. This division works because every team was counted equally often.

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Binomial theorem](binomial-theorem.md)
- [Cayley's formula](cayley-s-formula.md)
- [Combinatorics](combinatorics-split.md)
- [Exponential generating function](exponential-generating-function.md)
- [Factorial](factorial.md)
- [Generating function](generating-function.md)
- [Permutation](permutation.md)
- [Rule of product](rule-of-product.md)
