<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The empty family satisfies the bound, so assume $\mathcal F$ is nonempty and choose a [graph](../../../../../../graph-split.md) according to the [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md) $F\in\mathcal F$. Let $Y$ be its [random vector](../../../../../../random-vector.md) of [edge](../../../../../../edge-of-a-graph.md) indicators, indexed by $E=\binom{[n]}2$. Then its [information entropy](../../../../../../information-entropy.md) is $H(Y)=\log_2|\mathcal F|$.

For each [vertex](../../../../../../vertex-graph-theory.md) $v$, put $S_v=\{e\in E:v\in e\}$, so $Y_{S_v}$ records the [graph neighbourhood](../../../../../../graph-neighbourhood.md) of $v$. The possible [graph neighbourhoods](../../../../../../graph-neighbourhood.md) form an [intersecting family](../../../../../../intersecting-family.md) of subsets of $[n]\setminus\{v\}$: the [graph intersection](../../../../../../graph-intersection.md) of any two members of $\mathcal F$ has no [isolated vertex](../../../../../../isolated-vertex.md) at $v$. A subset and its complement cannot both occur. Pairing the $2^{n-1}$ subsets into complementary pairs gives at most $2^{n-2}$ possible [graph neighbourhoods](../../../../../../graph-neighbourhood.md). The [maximum entropy on a finite alphabet](../../../../../../maximum-entropy-on-a-finite-alphabet.md) therefore gives

$$
H(Y_{S_v})\leq n-2.
$$

This argument applies for $n\geq2$. For $n=1$ the assumed nonempty family cannot exist, since its only possible [graph](../../../../../../graph-split.md) has an [isolated vertex](../../../../../../isolated-vertex.md).

Each [edge](../../../../../../edge-of-a-graph.md) belongs to exactly two of the sets $S_v$. To obtain the needed instance of [Shearer inequality](../../../../../../shearer-s-inequality.md) directly from the preceding compression argument, repeatedly apply a [union-intersection compression](../../../../../../union-intersection-compression.md) to incomparable members of the [multiset](../../../../../../multiset.md) $(S_v)_{v=1}^n$. Each such step strictly increases $\sum_S|S|^2$, by

$$
2|A\setminus B|\,|B\setminus A|>0.
$$

The potential is bounded and integer-valued, so the process terminates in a chain under inclusion. Coordinate multiplicities stay equal to two, so, for $E\ne\varnothing$, the terminal chain consists of two copies of $E$ and $n-2$ empty sets. The [compression of an entropy sum](../../../../../../compression-of-an-entropy-sum.md) now gives

$$
2H(Y)\leq\sum_v H(Y_{S_v})\leq n(n-2).
$$

Exponentiating proves **the [entropy bound for graphs with isolated-vertex-free intersections](../../../../../../entropy-bound-for-graphs-with-isolated-vertex-free-intersections.md)**:

$$
\boxed{|\mathcal F|\leq2^{n(n-2)/2}=2^{n^2/2-n}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
