<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Number the [natural numbers](../../../../../natural-number.md) from one. If the [power set](../../../../../power-set.md) could be enumerated as $A_1,A_2,\ldots$, form $D=\{j:j\notin A_j\}$. For each $j$, membership of $j$ in $D$ is opposite to its membership in $A_j$, so $D\ne A_j$. This contradicts completeness of the enumeration. Thus the [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md) proves that the [power set](../../../../../power-set.md) is an [uncountable set](../../../../../uncountable-set.md).

For a finite [subset](../../../../../subset.md) $A$, define $b(A)=\sum_{j\in A}2^{j-1}$. This is a nonnegative [integer](../../../../../integer.md) and the map is injective: if two finite [subsets](../../../../../subset.md) differ, let $k$ be their largest differing element. Its contribution $2^{k-1}$ exceeds the sum $1+2+\cdots+2^{k-2}$ of all smaller possible contributions, so their codes differ. There are infinitely many singleton [subsets](../../../../../subset.md). Hence the [countability of finite subsets of a countable set](../../../../../countability-of-finite-subsets-of-a-countable-set.md) here is countable infinitude.

To treat all [bijections](../../../../../bijection.md), associate to every [subset](../../../../../subset.md) $A\subseteq\mathbb N$ the [permutation](../../../../../permutation.md) that swaps $2j-1$ and $2j$ when $j\in A$, and fixes both when $j\notin A$. These disjoint pair swaps define a [bijection](../../../../../bijection.md) of $\mathbb N$. Different [subsets](../../../../../subset.md) give different [permutations](../../../../../permutation.md), so the map from the [power set](../../../../../power-set.md) into $X$ is injective. Therefore $X$ is an [uncountable set](../../../../../uncountable-set.md).

Every [finitely supported permutation](../../../../../finitely-supported-permutation.md) fixes all elements above some $k$. A [bijection](../../../../../bijection.md) fixing that tail must permute $\{1,\ldots,k\}$: it cannot send a smaller element into the fixed tail without violating injectivity. There are exactly $k!$ such [permutations](../../../../../permutation.md). Thus

$$
Y=\bigcup_{k\geq1}\{\sigma:\sigma(j)=j\text{ for every }j>k\}
$$

is a [countable union](../../../../../countable-union.md) of finite [sets](../../../../../set-split.md). Enumerate first by $k$, then by one of the finitely many [permutations](../../../../../permutation.md) at that $k$; duplicates can be omitted. Infinitely many distinct pair swaps belong to $Y$, so $Y$ is countably infinite. **The full family is uncountable, while the finitely supported family is countably infinite.**

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
