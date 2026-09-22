<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

The convention in this question counts a point whenever every open [neighbourhood](../../../../../neighbourhood-mathematics.md) meets $A$, without excluding the point itself. These are [adherent points](../../../../../adherent-point.md), whose set is the [closure](../../../../../closure-topology.md) $\overline A$; they differ from [limit points](../../../../../limit-point.md) under the convention that requires a different point of $A$ in each neighbourhood.

If $A$ is a [closed set](../../../../../closed-set.md) and $x\notin A$, the [open set](../../../../../open-set.md) $X\setminus A$ is a neighbourhood of $x$ disjoint from $A$. Thus every adherent point lies in $A$. Conversely, if every adherent point lies in $A$, each $x\notin A$ has an open neighbourhood disjoint from $A$. Their union is $X\setminus A$, which is open. Hence **$A$ is closed exactly when it contains all the points specified in the question**.

The [interior of a set](../../../../../interior-topology.md) and [closure](../../../../../closure-topology.md) are

$$
\boxed{\operatorname{Int}(A)=\bigcup\{U:U\text{ open},\ U\subseteq A\},\qquad
\overline A=\bigcap\{F:F\text{ closed},\ A\subseteq F\}.}
$$

The neighbourhood description of the [closure](../../../../../closure-topology.md) follows because failure to be adherent is equivalent to lying in an open set disjoint from $A$.

For [closure of a connected set](../../../../../closure-of-a-connected-set.md), suppose $\overline A=U\sqcup V$ were a separation into two nonempty relatively open sets. Their intersections with the [connected subset](../../../../../connected-subset.md) $A$ would separate $A$ unless one intersection were empty. Say $A\subseteq U$. Choose $v\in V$ and an open set $O\subseteq X$ with $v\in O$ and $O\cap\overline A\subseteq V$. Since $v\in\overline A$, the set $O$ meets $A$, contradicting $A\subseteq U$. Thus **the closure of a connected set is connected**. The empty-set case holds directly.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
