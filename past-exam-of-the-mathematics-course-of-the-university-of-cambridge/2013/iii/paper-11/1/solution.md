<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a finite nonempty set $A$, its [additive energy](../../../../../additive-energy.md) is

$$
E(A,A)=\#\{(a_1,a_2,a_3,a_4)\in A^4:a_1+a_2=a_3+a_4\}
=\sum_s r_{A+A}(s)^2,
$$

where $r_{A+A}(s)$ counts ordered representations. Since $\sum_s r_{A+A}(s)=|A|^2$, [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) gives

$$
E(A,A)\geq\frac{|A|^4}{|A+A|}.
$$

Thus **$|A+A|\leq K|A|$ implies $E(A,A)\geq |A|^3/K$**: a small [doubling constant](../../../../../doubling-constant.md) forces many [additive quadruples](../../../../../additive-quadruple.md).

A polynomial form of the [Balog-Szemerédi-Gowers theorem](../../../../../balog-szemeredi-gowers-theorem.md) gives the converse after passing to a subset. There are absolute constants $c,C>0$ such that if $E(A,A)\geq\eta|A|^3$, $0<\eta\leq1$, then some $A'\subseteq A$ satisfies

$$
\boxed{|A'|\geq c\eta^C|A|,\qquad |A'+A'|\leq C\eta^{-C}|A'|.}
$$

The exponent and constants here need not be optimal.

Precisely, a [graph form of the Balog-Szemerédi-Gowers theorem](../../../../../graph-form-of-the-balog-szemeredi-gowers-theorem.md) states the following. If $A,B$ are finite sets of size $n$ in an [abelian group](../../../../../abelian-group.md), $\Gamma\subseteq A\times B$ has at least $\delta n^2$ edges, and its [restricted sumset](../../../../../restricted-sumset.md)

$$
A+_\Gamma B=\{a+b:(a,b)\in\Gamma\}
$$

has size at most $Kn$, then there are $A'\subseteq A$, $B'\subseteq B$ with $|A'|,|B'|\geq c\delta^C n$ and

$$
|A'+B'|\leq C\delta^{-C}K^C n.
$$

These are uniform absolute constants, valid for $0<\delta\leq1$ and $K\geq1$.

To apply this theorem to [additive energy](../../../../../additive-energy.md), let $n=|A|$ and retain the sums with $r_{A+A}(s)\geq\eta n/2$. The discarded sums contribute at most $(\eta n/2)\sum_s r(s)=\eta n^3/2$ to the [additive energy](../../../../../additive-energy.md). Since $r(s)\leq n$, the retained pairs number at least $\eta n^2/2$. There are at most $2n/\eta$ retained sums. They therefore define a [bipartite graph](../../../../../bipartite-graph.md) of density at least $\eta/2$ with [restricted sumset](../../../../../restricted-sumset.md) size at most $2n/\eta$. The graph theorem supplies large subsets $A',B'$ with polynomially bounded $|A'+B'|$.

For completeness, turn this cross-[sumset](../../../../../sumset.md) bound into a [doubling constant](../../../../../doubling-constant.md) bound. The [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) gives $|A'-A'|\leq |A'+B'|^2/|B'|$. If $D=|A'-A'|/|A'|$, the [Plünnecke inequality](../../../../../plunnecke-inequality.md), applied to the pair $A',-A'$, gives $|A'+A'|\leq D^2|A'|$. The minimal-growth proof below in Question 5 applies to arbitrary finite pairs and proves this particular expansion estimate as well. All losses are fixed powers of $\eta^{-1}$, proving the displayed converse after increasing $C$.

The requested [dense bipartite common-neighbour lemma](../../../../../dense-bipartite-common-neighbour-lemma.md) is a [dependent random choice](../../../../../dependent-random-choice.md) assertion. Call an ordered pair in $V^2$ bad when it has fewer than $\epsilon n$ [common neighbours](../../../../../common-neighbour.md). Choose $w\in W$ uniformly, and put $S=N(w)\subseteq V$. Then

$$
\mathbb E|S|=\delta m,\qquad \mathbb E|S|^2\geq\delta^2m^2.
$$

For each bad pair, the probability that both endpoints lie in $S$ is its number of [common neighbours](../../../../../common-neighbour.md) divided by $n$, which is less than $\epsilon$. Thus the expected number $b(S)$ of bad ordered pairs in $S^2$ is at most $\epsilon m^2$. Consequently

$$
\mathbb E\left[|S|^2-\frac{\delta^2}{2\epsilon}b(S)\right]\geq\frac{\delta^2m^2}{2}.
$$

Choose a neighbourhood $V'=S$ attaining at least this expectation. It has $|V'|\geq\delta m/\sqrt2\geq\delta m/2$, and

$$
b(V')\leq\frac{2\epsilon}{\delta^2}|V'|^2.
$$

Hence **at least the proportion $1-2\epsilon/\delta^2$ of its ordered pairs have at least $\epsilon n$ two-edge connections**. As usual these connections are counted by [common neighbours](../../../../../common-neighbour.md), including a return walk for a diagonal ordered pair; assume $\delta>0$, as the formula requires.

The relevance to the graph theorem is that many two-edge connections turn a sparse collection of permitted sums into additive control on a large vertex subset. On a connection $a\to b\to a'$, $a-a'=(a+b)-(a'+b)$ expresses a difference using two elements of the [restricted sumset](../../../../../restricted-sumset.md). The abundance of connections, followed by standard cleaning and further path counting, bounds the number of differences without throwing away most vertices. This is the role of [dependent random choice](../../../../../dependent-random-choice.md) in obtaining polynomial losses in the [graph form of the Balog-Szemerédi-Gowers theorem](../../../../../graph-form-of-the-balog-szemeredi-gowers-theorem.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
