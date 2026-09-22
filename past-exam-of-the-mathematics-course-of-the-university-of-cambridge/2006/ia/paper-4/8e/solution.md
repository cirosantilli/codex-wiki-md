<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

A [countable set](../../../../../countable-set.md) is one admitting an [injection](../../../../../injective-function.md) into $\mathbb N$; this includes finite sets and the empty set. An infinite [countable set](../../../../../countable-set.md) can equivalently be listed in a sequence indexed by $\mathbb N$.

For a [countable union of countable sets](../../../../../countable-union-of-countable-sets.md) $A=\bigcup_{i\geq1}A_i$, choose an [injection](../../../../../injective-function.md) $e_i:A_i\to\mathbb N$ for each nonempty $A_i$. Assign $x\in A$ the pair $(i,e_i(x))$, where $i$ is the least index with $x\in A_i$. This is an [injection](../../../../../injective-function.md) into $\mathbb N^2$. The pairs are countable by diagonal enumeration; explicitly, with natural numbers starting at one, the [Cantor pairing function](../../../../../cantor-pairing-function.md)

$$
(i,j)\longmapsto\frac{(i+j-2)(i+j-1)}2+j
$$

maps them bijectively to $\mathbb N$. Composing the two maps proves that the union is countable. Empty members contribute no elements.

To prove uncountability of the [power set](../../../../../power-set.md) $\mathcal P(\mathbb N)$, suppose all [subsets](../../../../../subset.md) could be listed as $A_1,A_2,\ldots$. Define

$$
D=\{n\in\mathbb N:n\notin A_n\}.
$$

For every $n$, $D$ differs from $A_n$ on whether it contains $n$. Thus $D$ is missing from the supposedly exhaustive list. This [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md) proves **$\mathcal P(\mathbb N)$ is uncountable**.

For increasing functions in the question's non-strict sense, encode every [subset](../../../../../subset.md) $A\subseteq\mathbb N$ by

$$
f_A(n)=n+\sum_{k=1}^{n}\mathbf1_A(k),\qquad f_A(0)=0
$$

where the value at zero is only a convenient auxiliary convention. Then

$$
f_A(n)-f_A(n-1)=1+\mathbf1_A(n).
$$

Each $f_A$ is even strictly increasing, hence is a [nondecreasing function](../../../../../nondecreasing-function.md) as required, and its successive differences recover $A$ uniquely. This is an [injection](../../../../../injective-function.md) from the uncountable [power set](../../../../../power-set.md) into the requested collection. Therefore **the increasing functions $\mathbb N\to\mathbb N$ form an [uncountable set](../../../../../uncountable-set.md)**.

For a decreasing function in the question's sense, $f$ is a [nonincreasing function](../../../../../nonincreasing-function.md) with positive integer values. Each strict decrease lowers its value by at least one, so there can be at most $f(1)-1$ strict decreases. There is consequently a final drop, after which the function is constant. Every such function is determined by a finite initial list whose final value repeats forever. The set of all these lists is contained in

$$
\bigcup_{N=1}^{\infty}\mathbb N^N,
$$

a countable union of [countable sets](../../../../../countable-set.md), hence countable by the result just proved. Thus **the decreasing functions $\mathbb N\to\mathbb N$ form a [countable set](../../../../../countable-set.md)**. These contrasting [cardinalities of monotone natural-number functions](../../../../../cardinalities-of-monotone-natural-number-functions.md) come from the absence of an upper bound for increasing values and the finite number of drops available to decreasing natural-number values. If the natural numbers include zero, the same proof uses the bound $f(1)$ instead.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
