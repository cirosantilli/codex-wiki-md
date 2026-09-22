<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a fixed [uniform hypergraph](../../../../../uniform-hypergraph.md) $H$ with $h$ [vertices](../../../../../vertex-graph-theory.md), uniformity $\ell$, and at least one [edge](../../../../../edge-of-a-graph.md), define its [Turán density](../../../../../turan-density.md) by

$$
\pi(H)=\lim_{n\to\infty}\frac{\operatorname{ex}(n,H)}{\binom n\ell},
$$

where $\operatorname{ex}(n,H)$ is the maximum [edge](../../../../../edge-of-a-graph.md) count of an $H$-free hypergraph. The limit exists: averaging the [edge](../../../../../edge-of-a-graph.md) count over all $m$-vertex subsets of an extremal $n$-vertex hypergraph, with $n\ge m\ge\ell$, shows that the displayed normalized extremal numbers are nonincreasing. Thus their limit is their infimum.

For [hypergraph supersaturation by sampling](../../../../../hypergraph-supersaturation-by-sampling.md), choose $m\ge h$ so that $\operatorname{ex}(m,H)/\binom m\ell\le\pi(H)+\epsilon/2$. The expected [edge](../../../../../edge-of-a-graph.md) count in a uniform $m$-vertex subset of $G$ is at least $(\pi(H)+\epsilon)\binom m\ell$. A subset containing no copy of $H$ has at most $(\pi(H)+\epsilon/2)\binom m\ell$ [edges](../../../../../edge-of-a-graph.md), while any subset has at most $\binom m\ell$. Hence at least an $\epsilon/2$ fraction of the subsets contain $H$. Every particular copy of $H$ lies in exactly $\binom{n-h}{m-h}$ such subsets, so their number is at least

$$
\frac\epsilon2\frac{\binom nm}{\binom{n-h}{m-h}}=\frac\epsilon2\frac{(n)_h}{(m)_h}\ge\frac{\epsilon}{2^{h+1}(m)_h}n^h
$$

for $n\ge N=\max(m,2h)$. Take

$$
\delta=\min\left\{\frac{\epsilon}{2^{h+1}(m)_h},\ \frac1{2N^h}\right\}.
$$

For $n<N$, the requested integer lower bound is zero; for $n\ge N$, the calculation proves it. **This positive $\delta$ depends only on $H$ and $\epsilon$.** If the density hypothesis is impossible there is nothing to prove. For an edgeless $H$, every $h$-set is already a copy and the conclusion follows directly.

For the edge-triangle objective, let $N(v)$ be the open neighbourhood of $v$ and define its local score

$$
s(v)=d(v)-c\,e(G[N(v)]).
$$

It counts the contribution to $k_2-ck_3$ of [edges](../../../../../edge-of-a-graph.md) and [triangles in a graph](../../../../../triangle-in-a-graph.md) containing $v$. If $u,v$ are nonadjacent, making $u$ a [false twin](../../../../../false-twin.md) of $v$ changes the objective by $s(v)-s(u)$, since no [edge](../../../../../edge-of-a-graph.md) or [triangle in a graph](../../../../../triangle-in-a-graph.md) uses both. More generally, partition [vertices](../../../../../vertex-graph-theory.md) into [false-twin classes](../../../../../false-twin-class.md), meaning equal open neighbourhoods. If distinct classes $U,V$ have no [edges](../../../../../edge-of-a-graph.md) between them, making every [vertex](../../../../../vertex-graph-theory.md) of $U$ a twin of a representative of $V$ changes the objective by $|U|(s(v)-s(u))$. Choose the direction with nonnegative change.

Among [graphs](../../../../../graph-split.md) maximizing the objective, choose one maximizing the sum of squared false-twin class sizes. The operation cannot split any old false-twin class and merges $U,V$, so it would strictly increase that secondary quantity. Therefore no two distinct classes can be nonadjacent. **An objective maximizer is a complete multipartite [graph](../../../../../graph-split.md).** This [edge-triangle symmetrization](../../../../../edge-triangle-symmetrization.md) works for every real $c$, with no assumption on its sign.

For positive part sizes $a_1,\ldots,a_q$, the correct multipartite formula is

$$
F(a_1,\ldots,a_q)=\sum_{i<j}a_ia_j-c\sum_{i<j<k}a_ia_ja_k.
$$

The first sum in the printed intermediate formula has inconsistent indices; the [edge](../../../../../edge-of-a-graph.md) count is the pairwise-product sum above. Fix two part sizes with sum $A$ and let $B$ be the sum of all other sizes. All terms varying with the pair have the form

$$
\text{constant}+(1-cB)a_ia_j.
$$

Choose a maximizing partition with the fewest nonempty parts. If $1-cB\le0$, merging those two parts cannot decrease $F$ and reduces the number of parts, a contradiction. Therefore this coefficient is positive for every pair. If two integer sizes differ by at least two, moving one [vertex](../../../../../vertex-graph-theory.md) from the larger to the smaller increases their product and hence $F$, again a contradiction. **All sizes differ by at most one, so a maximizer is a Turan [graph](../../../../../graph-split.md).** This is [balancing a multipartite edge-triangle objective](../../../../../balancing-a-multipartite-edge-triangle-objective.md).

Next maximize the same polynomial on the compact simplex of nonnegative real sizes summing to $n$, starting with at least two possible parts. Choose a maximizer with the smallest positive support. The merging argument still applies, and now varying two positive unequal sizes towards equality improves the product. Thus every positive size is $n/q$ for some integer $q$. A two-part choice has value $n^2/4>0$ when $n>0$, so $q\ge2$. The optimum is attained at rational sizes, and therefore

$$
\boxed{k_2(G)-ck_3(G)\le\binom q2(n/q)^2-c\binom q3(n/q)^3\quad\text{for some integer }q\ge2.}
$$

One may take the initial simplex to have $\max(n,2)$ coordinates, so it includes every multipartite [graph](../../../../../graph-split.md) obtained above; zero coordinates are discarded.

Set $c=9/(4n)$. Dividing the right side by $n^2$ gives

$$
\frac{(q-1)(q+6)}{8q^2}=\frac14-\frac{(q-2)(q-3)}{8q^2}\le\frac14,
$$

because $q$ is an integer at least two. Rearranging proves

$$
\boxed{k_3(G)\ge\frac{4n}{9}\left(k_2(G)-\frac{n^2}{4}\right).}
$$

Equality in the continuous calculation occurs at two or three equal parts, explaining the [triangle support line between bipartite and tripartite Turan graphs](../../../../../triangle-support-line-between-bipartite-and-tripartite-turan-graphs.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
