<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The unrestricted identity needs qualification. A [Fano plane](../../../../../fano-plane.md) has seven [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md), so the complete three-[uniform hypergraph](../../../../../uniform-hypergraph.md) on six [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md) avoids it and has twenty edges, whereas the displayed balanced-part count is eighteen. On five [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md) the corresponding numbers are ten and nine. Thus the intended extremal theorem is the sufficiently-large-$n$ [Fano-plane Turán theorem](../../../../../fano-plane-turan-theorem.md). We describe its stability proof, including the exact counting step that upgrades an asymptotic result to equality.

Identify the Fano points with the nonzero vectors of $\mathbb F_2^3$, and its [hyperedges](../../../../../hyperedge.md) with triples summing to zero. It has no [Property B](../../../../../property-b.md). Indeed, a line-free set has at most four points: if a set $A$ of nonzero vectors contains no zero-sum triple and $a\in A$, the sets $A\setminus\{a\}$ and $a+(A\setminus\{a\})$ are disjoint subsets of the six nonzero vectors other than $a$, so $|A|\le4$. Moreover, if $|A|=4$, those two three-element sets partition those six vectors. Write $A=\{a,b,c,d\}$. The sum $b+c$ lies outside $A$, so belongs to $a+(A\setminus\{a\})$. It is neither $a+b$ nor $a+c$, and must therefore equal $a+d$. Thus $a+b+c+d=0$. The other three points have sum zero because the sum of all seven nonzero vectors is zero. They therefore form a line. In any two-colouring one colour has at least four points: if it contains a line we are done, and otherwise the other colour contains a line. This proves non-two-colourability.

Partition the host [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md) into sizes $a,b$ and take all triples meeting both parts. This [bipartite three-uniform hypergraph](../../../../../bipartite-three-uniform-hypergraph.md) has [Property B](../../../../../property-b.md) and is consequently Fano-free. Its edge count is

$$
a\binom b2+b\binom a2=\frac{ab(n-2)}2.
$$

The product $ab$ is maximized at balanced integer sizes. Writing

$$
b(n)=\binom n3-\binom{\lfloor n/2\rfloor}3-\binom{\lceil n/2\rceil}3,
$$

we have the exact lower bound $\operatorname{ex}(n,F)\ge b(n)$, and $b(n)=(3/4+o(1))\binom n3$.

The structural step is [Fano stability](../../../../../fano-stability.md): a Fano-free [hypergraph](../../../../../hypergraph-split.md) with density sufficiently close to $3/4$ has a bipartition with at most $\rho n^3$ internal triples, for any prescribed $\rho>0$. Its proof studies four [hypergraph link graphs](../../../../../hypergraph-link-graph.md) around a complete four-vertex three-uniform configuration. Colour a pair by the link [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md) containing it. Three perfect [matchings in a graph](../../../../../matching-graph-theory.md) on four other [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md), with distinct colours corresponding to a triple of the configuration, would complete a Fano copy. Thus these rainbow patterns are forbidden. The near-extremal total link degree forces, after removing a small exceptional set, an almost balanced pattern with pair multiplicity two within the two classes and four between them. Internal triple density bounded away from zero produces many complete tripartite six-vertex templates; the nearly complete links then supply three paired neighbours and complete a Fano plane. Consequently the internal triple density tends to zero. These are the main ingredients of the stability argument: link degree counting supplies the approximate partition, and the forbidden completion templates eliminate positive internal density.

To see concretely why stability gives the **exact** bound, suppose $e(H)\ge b(n)$, and first obtain high minimum [hypergraph vertex degree](../../../../../hypergraph-vertex-degree.md). Delete any vertex of degree at most $3m^2/8-2m$ when the current order is $m$. Directly from the formula for $b$, for large $m$,

$$
b(m)-b(m-1)>3m^2/8-2m+1.
$$

After deletions down to order $m$, the remaining [hypergraph](../../../../../hypergraph-split.md) therefore has at least $b(m)+n-m$ edges. It cannot reach $m=\lceil n^{1/3}\rceil$, since this exceeds $\binom m3$ for large $n$. The process stops at an order still tending to infinity, with [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) greater than $3m^2/8-2m$. If the high-minimum-degree case has at most $b(m)$ edges, any deletion gives a contradiction. Thus it suffices to treat that case; rename its order $n$.

Apply stability with a very small constant, for example $\rho=10^{-12}$, and choose a partition $A\sqcup B$ minimizing the number of internal [hyperedges](../../../../../hyperedge.md). Its part sizes are close to $n/2$, since its cross-part capacity is $|A||B|(n-2)/2$, and $e(H)\ge b(n)$ leaves at most $\rho n^3$ available compensation for any imbalance. In particular $||A|-n/2|,||B|-n/2|\le2\sqrt\rho n$ for large $n$. Optimality also gives

$$
e(L_H(x)[A])\le e(L_H(x)[B])\quad(x\in A),
$$

with the analogous inequality for $x\in B$: otherwise moving $x$ would reduce the internal count.

Suppose some $x\in A$ has more than $n^2/100$ edges in its same-side link. Its opposite-side link then has at least as many. Each link has a [matching in a graph](../../../../../matching-graph-theory.md) of size at least $\lfloor n/300\rfloor$: the endpoints of a maximal [matching in a graph](../../../../../matching-graph-theory.md) cover every edge, so a [matching in a graph](../../../../../matching-graph-theory.md) of size $s$ bounds the link edge count by $2sn$. For each choice of one [matching in a graph](../../../../../matching-graph-theory.md) edge in $A$ and two [matching in a graph](../../../../../matching-graph-theory.md) edges in $B$, the six [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md) plus $x$ would form a Fano plane if all transversal triples through the three pairs were present. Specifically take the three triples through $x$ and the four even-parity transversal triples. Hence at least one of these cross-part triples is missing. The [matchings in a graph](../../../../../matching-graph-theory.md) are disjoint, so different choices give different missing triples. There are at least

$$
s\binom s2\quad\text{such missing triples},\qquad s=\lfloor n/300\rfloor.
$$

For large $n$ this exceeds $\rho n^3$, contradicting the edge count: the missing cross triples already outweigh every internal triple. Thus every same-side link has at most $n^2/100$ edges.

If an internal triple $xyz\subseteq A$ remains, high [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) gives, for each of its [vertices of a hypergraph](../../../../../vertex-of-a-hypergraph.md),

$$
e(L_H(x)[B])>\frac{3n^2}{8}-2n-|A||B|-\frac{n^2}{100}
\ge\left(\frac18-\frac1{100}\right)n^2-2n.
$$

The intersection of the three opposite-side links therefore has at least their total edge count minus $2\binom{|B|}2$. Using $|B|\le(1/2+2\sqrt\rho)n$, this exceeds $|B|^2/3$ for large $n$. By the quadratic [Turan theorem](../../../../../turan-s-theorem.md) bound, their intersection contains $K_4$. Its three perfect [matchings in a graph](../../../../../matching-graph-theory.md), assigned to $x,y,z$, together with $xyz$ are the seven edges of a Fano plane. This is precisely [Fano completion through three matchings](../../../../../fano-completion-through-three-matchings.md), and gives a contradiction. The same argument excludes internal triples in $B$.

Thus the high-minimum-degree [hypergraph](../../../../../hypergraph-split.md) is genuinely bipartite, not merely approximately so, and has at most $b(n)$ edges. The deletion argument proves the same bound for the original [hypergraph](../../../../../hypergraph-split.md). Combining with the balanced construction yields

$$
\boxed{\operatorname{ex}(n,F)=\binom n3-\binom{\lfloor n/2\rfloor}3-\binom{\lceil n/2\rceil}3\quad\text{for all sufficiently large }n.}
$$

This proof description keeps the essential roles distinct: non-two-colourability gives the lower construction, link-graph stability gives an approximate partition, and the minimum-degree/[matching in a graph](../../../../../matching-graph-theory.md) argument removes the last internal edges. The ceiling in the final term is confirmed by the PDF; the converted TeX incorrectly repeats the floor.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
