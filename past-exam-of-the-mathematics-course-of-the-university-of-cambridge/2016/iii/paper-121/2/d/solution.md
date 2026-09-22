<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [cardinal bound for an increasing chain of countable sets](../../../../../../cardinal-bound-for-an-increasing-chain-of-countable-sets.md) is $\boxed{|X|\leq\aleph_1}$. If $X$ is countable, there is nothing to prove. Otherwise choose $Y\subseteq X$ with $|Y|=\aleph_1$, and for every $y\in Y$ choose an index $i(y)$ such that $y\in X_{i(y)}$.

For any $i\in I$, its countable $X_i$ cannot contain all of $Y$, so choose $y\in Y\setminus X_i$. Since $I$ is a [linear order](../../../../../../linear-order.md), comparison of $i$ and $i(y)$ forces $i<i(y)$: the other direction would imply $y\in X_i$. Therefore $X_i\subseteq X_{i(y)}$. The selected family is cofinal among the original sets, and

$$
X=\bigcup_{y\in Y}X_{i(y)}.
$$

By [infinite cardinal arithmetic](../../../../../../infinite-cardinal-arithmetic.md), this union of $\aleph_1$ countable sets has [cardinality](../../../../../../cardinality.md) at most $\aleph_1$. No [well-order](../../../../../../well-order.md) or [cofinality](../../../../../../cofinality.md) assumption on $I$ was used; a [linear increasing union of countable sets](../../../../../../increasing-chain-of-countable-sets.md) has the same bound even for an arbitrary linear index order.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
