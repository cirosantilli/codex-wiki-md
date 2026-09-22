<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [linked graph](../../../../../linked-graph.md) is $k$-linked if it has at least $2k$ [vertices](../../../../../vertex-graph-theory.md) and, for every choice of distinct terminals $s_1,\ldots,s_k,t_1,\ldots,t_k$, it has pairwise vertex-disjoint [graph paths](../../../../../path-in-a-graph.md) joining $s_i$ to $t_i$ for all $i$. The pairing is prescribed, which is stronger than the unpaired conclusion of the [Menger theorem](../../../../../menger-theorem.md).

We prove the [rooted dense minor linkage](../../../../../rooted-dense-minor-linkage.md) step carefully. We first prove the [rooted branch-set reduction](../../../../../rooted-branch-set-reduction.md). Let $q\ge2$ be even, let $S=\{x_1,\ldots,x_q\}$, and suppose a [graph](../../../../../graph-split.md) has $h$ disjoint nonempty [vertex](../../../../../vertex-graph-theory.md) [sets](../../../../../set-split.md) $C_1,\ldots,C_h$, where $h\ge d+3q/2$. Suppose each $G[C_i]$ is connected or every one of its [graph components](../../../../../component-graph-theory.md) meets $S$, and each $C_i$ is adjacent to all but at most $d$ of the other $C_j$ not meeting $S$. Assume also that no [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) of order below $q$ avoids $d+1$ of these [sets](../../../../../set-split.md). Then there are $m=h-q/2$ disjoint connected [vertex](../../../../../vertex-graph-theory.md) [sets](../../../../../set-split.md) $D_1,\ldots,D_m$ such that $x_i\in D_i$ for $1\le i\le q$ and each of these first $q$ [sets](../../../../../set-split.md) is adjacent to all but at most $d$ of $D_{q+1},\ldots,D_m$.

Here adjacency of [sets](../../../../../set-split.md) means existence of an [edge](../../../../../edge-of-a-graph.md) between them. A [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) is $(A,B)$ with $A\cup B=V(G)$, $S\subseteq A$, no [edges](../../../../../edge-of-a-graph.md) between $A\setminus B$ and $B\setminus A$, and order $|A\cap B|$. It avoids $C_i$ when $A\cap C_i=\varnothing$. We prove the reduction by [induction](../../../../../mathematical-induction.md), first on the [vertex](../../../../../vertex-graph-theory.md) count and then on the [edge](../../../../../edge-of-a-graph.md) count; any counterexample chosen minimal in this ordering will be impossible.

We may delete [edges](../../../../../edge-of-a-graph.md) joining two [vertices](../../../../../vertex-graph-theory.md) of $S$. They cannot affect [rooted separations of a graph](../../../../../rooted-separation-of-a-graph.md), since $S$ lies wholly on the first side. Within a branch [set](../../../../../set-split.md), their deletion can only split a [graph component](../../../../../component-graph-theory.md) into [graph components](../../../../../component-graph-theory.md) each containing an endpoint in $S$, so the branch-set hypothesis also persists. An isolated [vertex](../../../../../vertex-graph-theory.md) outside $S$ and all branch [sets](../../../../../set-split.md) can be deleted. An isolated [vertex](../../../../../vertex-graph-theory.md) $v\in S$ is also impossible, since $(S,V(G)\setminus\{v\})$ has order $q-1$ and avoids at least $h-q\ge d+q/2\ge d+1$ [sets](../../../../../set-split.md). Thus in a minimal counterexample $S$ is independent, and every isolated [vertex](../../../../../vertex-graph-theory.md) outside $S$ belongs to a singleton branch [set](../../../../../set-split.md).

Consider a [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) $(A,B)$ of order exactly $q$ avoiding at least $d+1$ branch [sets](../../../../../set-split.md), and put $S'=A\cap B$. Restrict to $G'=G[B]-E(G[S'])$ and $C'_i=C_i\cap B$. Each $C'_i$ is nonempty: any $C_i$ not itself avoided is adjacent to at least one of the $d+1$ avoided [sets](../../../../../set-split.md), and the endpoint of such an [edge](../../../../../edge-of-a-graph.md) in $C_i$ must lie in $B$. If a [graph component](../../../../../component-graph-theory.md) of $G'[C'_i]$ misses $S'$, it lies in $B\setminus A$ and is a whole [graph component](../../../../../component-graph-theory.md) of $G[C_i]$, with no [vertex](../../../../../vertex-graph-theory.md) of $S$. The original hypothesis then forces $G[C_i]$ to be connected and $C'_i=C_i$, entirely outside $A$. Thus each restricted [set](../../../../../set-split.md) is connected or all its [graph components](../../../../../component-graph-theory.md) meet $S'$. In particular every $C'_j$ missing $S'$ equals an original [set](../../../../../set-split.md) outside $A$, so all its required adjacencies from $C'_i$ persist.

A [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) $(A',B')$ of $G'$ avoiding $d+1$ restricted [sets](../../../../../set-split.md) lifts to $(A\cup A',B')$ in $G$, of the same order: an avoided restricted [set](../../../../../set-split.md) misses $S'$, hence is an original [set](../../../../../set-split.md) outside $A$. The [edges](../../../../../edge-of-a-graph.md) removed inside $S'$ do not obstruct lifting, since $S'\subseteq A'$. This proves the required separation hypothesis for $G'$. If $G'$ is smaller, [induction](../../../../../mathematical-induction.md) gives the desired connected [sets](../../../../../set-split.md) rooted at $S'$. Moreover $G[A]$ has $q$ disjoint [graph paths](../../../../../path-in-a-graph.md) from $S$ to $S'$, by the [Menger theorem](../../../../../menger-theorem.md). Indeed a separator of smaller order between these [sets](../../../../../set-split.md) would give a [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) of $G$ of smaller order still avoiding those $d+1$ original [sets](../../../../../set-split.md). Truncate the [graph paths](../../../../../path-in-a-graph.md) at their first visits to $S'$, label their endpoints accordingly, and adjoin each [graph path](../../../../../path-in-a-graph.md) to the corresponding rooted connected [set](../../../../../set-split.md). They meet $B$ only in their distinct endpoints, so this gives the desired [sets](../../../../../set-split.md) for $G$, a contradiction. Consequently in a minimal counterexample every such separation of order $q$ has $B=V(G)$ and $A=S$, an [independent set](../../../../../independent-set-graph-theory.md).

Now contract any [edge](../../../../../edge-of-a-graph.md) whose endpoints do not belong to two different branch [sets](../../../../../set-split.md). Its endpoints cannot both lie in $S$, so the image of $S$ still has size $q$. The branch-set conditions persist. If the contraction created a forbidden [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) of order below $q$, its lift would have order below $q$, except possibly when the contracted [vertex](../../../../../vertex-graph-theory.md) lies in its separator. In that case the lifted order increases by one and is at most $q$. Equality would put the contracted [edge](../../../../../edge-of-a-graph.md) inside $A$, contradicting the just-proved independence of $A$ for an order-$q$ separation avoiding $d+1$ [sets](../../../../../set-split.md). Thus the separation hypothesis also persists. Applying [induction](../../../../../mathematical-induction.md) in the contracted [graph](../../../../../graph-split.md) and expanding the contracted [vertex](../../../../../vertex-graph-theory.md) would produce the required disjoint connected [sets](../../../../../set-split.md). Hence **every [edge](../../../../../edge-of-a-graph.md) in a minimal counterexample joins two different branch [sets](../../../../../set-split.md)**.

Every [vertex](../../../../../vertex-graph-theory.md) outside the branch [sets](../../../../../set-split.md) would be isolated, since every [edge](../../../../../edge-of-a-graph.md) joins two branch [sets](../../../../../set-split.md); such an isolated [vertex](../../../../../vertex-graph-theory.md) could be deleted. Thus the branch [sets](../../../../../set-split.md) cover the [graph](../../../../../graph-split.md). Each nonsingleton branch [set](../../../../../set-split.md) is therefore an [independent set](../../../../../independent-set-graph-theory.md), and all its [vertices](../../../../../vertex-graph-theory.md) belong to $S$, because each of its singleton [graph components](../../../../../component-graph-theory.md) must meet $S$. Let $C$ be the union of the nonsingleton branch [sets](../../../../../set-split.md), and write $c=|C|\le q$. There is a [matching in a graph](../../../../../matching-graph-theory.md) from $C$ into $V(G)\setminus S$. Otherwise the [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) gives $X\subseteq C$ with neighbourhood $Y\subseteq V(G)\setminus S$ satisfying $|Y|<|X|$. Since $S$ is independent, $(S\cup Y,V(G)\setminus X)$ is a [rooted separation of a graph](../../../../../rooted-separation-of-a-graph.md) of order $q-|X|+|Y|<q$. It avoids every singleton branch [set](../../../../../set-split.md) outside $S\cup Y$, of which there are at least

$$
|V(G)|-q-|Y|\ge |V(G)|-q-c+1\ge h-\frac c2-q+1\ge h-\frac{3q}2+1\ge d+1.
$$

The penultimate counting bound uses that the nonsingleton [sets](../../../../../set-split.md) number at most $c/2$, so $|V(G)|-c\ge h-c/2$. This contradicts the separation hypothesis.

Use that [matching in a graph](../../../../../matching-graph-theory.md) to make a two-vertex connected [set](../../../../../set-split.md) for each terminal in $C$; terminals outside $C$ remain singleton [sets](../../../../../set-split.md). There are at least

$$
|V(G)|-q-c\ge h-\frac{3q}2=m-q
$$

unused [vertices](../../../../../vertex-graph-theory.md), all singleton original branch [sets](../../../../../set-split.md). Choose $m-q$ of them for the remaining $D_i$. Every rooted $D_i$ contains a singleton original branch [set](../../../../../set-split.md): either its terminal, or its terminal's matched [neighbour](../../../../../neighbour-of-a-vertex.md). That singleton misses at most $d$ of the selected nonterminal singleton [sets](../../../../../set-split.md). This constructs exactly the desired family, contradicting minimality and proving the branch-set reduction.

Return to the given $22k$-connected [graph](../../../../../graph-split.md). By the allowed assumption it has a [graph minor](../../../../../graph-minor.md) $H$ with $2\delta(H)\ge h+4k-1$, where $h=|H|$. Put $d=h-1-\delta(H)$. Then

$$
h\ge2d+4k+1.
$$

Take a branch-set model of $H$ and the $2k$ prescribed terminals as $S$. The branch [sets](../../../../../set-split.md) are connected and each misses at most $d$ of the others. The separation hypothesis holds with $q=2k$: a separation of order below $2k$ avoiding a branch [set](../../../../../set-split.md) would separate a surviving terminal from that [set](../../../../../set-split.md), contrary even to $2k$-connectivity. Since $h\ge d+3k$, the reduction applies. It produces $m=h-k$ [sets](../../../../../set-split.md) with $s_i\in D_i$, $t_i\in D_{k+i}$, each terminal [set](../../../../../set-split.md) missing at most $d$ of the $m-2k$ nonterminal [sets](../../../../../set-split.md). For each pair $D_i,D_{k+i}$ at least

$$
m-2k-2d=h-3k-2d\ge k+1
$$

nonterminal [sets](../../../../../set-split.md) are adjacent to both. Choose different such [sets](../../../../../set-split.md) for the $k$ pairs successively. The [connected graph](../../../../../connected-graph.md) property inside the three [sets](../../../../../set-split.md) and the two joining [edges](../../../../../edge-of-a-graph.md) give a [graph path](../../../../../path-in-a-graph.md) from $s_i$ to $t_i$; take a simple [graph path](../../../../../path-in-a-graph.md) within their union. Different [graph paths](../../../../../path-in-a-graph.md) use disjoint [sets](../../../../../set-split.md). We have proved

$$
\boxed{\kappa(G)\ge22k\ \Longrightarrow\ G\text{ is }k\text{-linked}.}
$$

In fact the argument proves the stronger transfer statement with $2k$-connectivity and the stated dense [graph minor](../../../../../graph-minor.md).

For the negative assertion, it suffices to give a value of $k$ for which the proposed general implication fails. Take $k=2$ and the [graph](../../../../../graph-split.md) on cyclic indices $0,\ldots,7$ in which two indices are adjacent when their cyclic distance is one or two. This is the [four-connected planar obstruction to two-linkage](../../../../../four-connected-planar-obstruction-to-two-linkage.md). Draw the even [cycle in a graph](../../../../../cycle-in-a-graph.md) $0,2,4,6$ as the outer square, the odd [cycle in a graph](../../../../../cycle-in-a-graph.md) $1,3,5,7$ as an inner square rotated by $45$ [degrees of vertices](../../../../../degree-graph-theory.md), and join each odd [vertex](../../../../../vertex-graph-theory.md) to the two neighbouring even [vertices](../../../../../vertex-graph-theory.md); the annulus is triangulated without crossings. The outer face has [vertices](../../../../../vertex-graph-theory.md) $0,2,4,6$ in this order.

<a id="3/image-a-four-connected-planar-graph-with-alternating-terminal-pairs-on-a-square-face"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9-antiprism.png)

**[Figure 1](#3/image-a-four-connected-planar-graph-with-alternating-terminal-pairs-on-a-square-face). A four-connected planar graph with alternating terminal pairs on a square face**.

Deleting at most three [vertices](../../../../../vertex-graph-theory.md) leaves the [graph](../../../../../graph-split.md) connected. In cyclic order, consecutive surviving [vertices](../../../../../vertex-graph-theory.md) are joined unless separated by a run of at least two deleted [vertices](../../../../../vertex-graph-theory.md). Disconnection requires two distinct such runs, hence at least four deletions. Conversely deleting the four [neighbours](../../../../../neighbour-of-a-vertex.md) of a [vertex](../../../../../vertex-graph-theory.md) isolates it, so the [vertex connectivity](../../../../../vertex-connectivity.md) is exactly four. Disjoint [graph paths](../../../../../path-in-a-graph.md) joining $0$ to $4$ and $2$ to $6$ cannot exist: both would lie in the closed disk complementary to the outer face, and their endpoints alternate on its boundary. A first such [graph path](../../../../../path-in-a-graph.md) is a crosscut of the disk; the [Jordan curve theorem](../../../../../jordan-curve-theorem.md) puts the other two endpoints on opposite sides, forcing the second [graph path](../../../../../path-in-a-graph.md) to meet it. Thus

$$
\boxed{\kappa(G)=4=3\cdot2-2,\qquad G\text{ is not }2\text{-linked}.}
$$

This is a counterexample to the unrestricted implication; no claim that the same construction works for every $k$ is needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
