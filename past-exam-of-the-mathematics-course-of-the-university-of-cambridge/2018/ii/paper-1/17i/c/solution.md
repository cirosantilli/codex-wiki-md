<h1 id="17i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First consider a $K_{t,t}$-free [bipartite graph](../../../../../../bipartite-graph.md) with parts $X,Y$, each of size at most $n$, and $m$ edges. Count pairs $(S,y)$ in which $S$ is a $t$-element subset of the [graph neighbourhood](../../../../../../graph-neighbourhood.md) of $y\in Y$. Any $t$ vertices of $X$ have at most $t-1$ common neighbours, since $t$ common neighbours would form the [complete bipartite graph](../../../../../../complete-bipartite-graph.md) $K_{t,t}$. Consequently

$$
\sum_{y\in Y}\binom{d(y)}t\leq(t-1)\binom{|X|}t.
$$

If the average [degree of a vertex](../../../../../../degree-graph-theory.md) is bounded in terms of $t$, then $m=O(n)$ and the required result is immediate. Otherwise, [convexity](../../../../../../convex-function.md) of $x\mapsto\binom xt$ and the preceding inequality give

$$
|Y|\binom{m/|Y|}t=O(n^t),
$$

and hence $m=O(n^{2-1/t})$. Every graph has a bipartite spanning subgraph containing at least half its edges, obtained by choosing a random bipartition. Applying the bipartite estimate to that subgraph proves the [Kővári–Sós–Turán theorem](../../../../../../kovari-sos-turan-theorem.md) in the required form:

$$
\boxed{\ \operatorname{ex}(n,K_{t,t})=O(n^{2-1/t}).\ }
$$

The stated "nice" subsets of the [finite cyclic group](../../../../../../finite-cyclic-group.md) $\mathbb Z_n$ are [Sidon sets](../../../../../../sidon-set.md). If

$$
a-b=c-d,
\qquad a\ne b,\qquad c\ne d,
$$

then $a+d=c+b$. Niceness forces $(a,b)=(c,d)$; the alternative pairing would force $a=b$. Thus the $|A|(|A|-1)$ ordered nonzero differences are distinct elements of the $n-1$ nonzero residue classes. Therefore

$$
|A|(|A|-1)\leq n-1,
$$

so

$$
\boxed{\ f(n)\leq\frac{1+\sqrt{4n-3}}2=O(\sqrt n).\ }
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17I](../../17i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
