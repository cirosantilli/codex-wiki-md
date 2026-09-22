# Rooted branch-set reduction

↑ **Parent:** [Graph minor](graph-minor.md)

Let $q\ge2$ be even, let $S=\{x_1,\ldots,x_q\}$, and suppose a [graph](graph-split.md) has $h$ disjoint nonempty [vertex](vertex-graph-theory.md) [sets](set-split.md) $C_1,\ldots,C_h$, where $h\ge d+3q/2$. Suppose each $G[C_i]$ is connected or every one of its [graph components](component-graph-theory.md) meets $S$, and each $C_i$ is adjacent to all but at most $d$ of the other $C_j$ not meeting $S$. Assume also that no [rooted separation of a graph](rooted-separation-of-a-graph.md) of order below $q$ avoids $d+1$ of these [sets](set-split.md). Then there are $m=h-q/2$ disjoint connected [vertex](vertex-graph-theory.md) [sets](set-split.md) $D_1,\ldots,D_m$ such that $x_i\in D_i$ for $1\le i\le q$ and each of these first $q$ [sets](set-split.md) is adjacent to all but at most $d$ of $D_{q+1},\ldots,D_m$.

Here adjacency of [sets](set-split.md) means existence of an [edge](edge-of-a-graph.md) between them. A [rooted separation of a graph](rooted-separation-of-a-graph.md) is $(A,B)$ with $A\cup B=V(G)$, $S\subseteq A$, no [edges](edge-of-a-graph.md) between $A\setminus B$ and $B\setminus A$, and order $|A\cap B|$. It avoids $C_i$ when $A\cap C_i=\varnothing$. We prove the reduction by [induction](mathematical-induction.md), first on the [vertex](vertex-graph-theory.md) count and then on the [edge](edge-of-a-graph.md) count; any counterexample chosen minimal in this ordering will be impossible.

We may delete [edges](edge-of-a-graph.md) joining two [vertices](vertex-graph-theory.md) of $S$. They cannot affect [rooted separations of a graph](rooted-separation-of-a-graph.md), since $S$ lies wholly on the first side. Within a branch [set](set-split.md), their deletion can only split a [graph component](component-graph-theory.md) into [graph components](component-graph-theory.md) each containing an endpoint in $S$, so the branch-set hypothesis also persists. An isolated [vertex](vertex-graph-theory.md) outside $S$ and all branch [sets](set-split.md) can be deleted. An isolated [vertex](vertex-graph-theory.md) $v\in S$ is also impossible, since $(S,V(G)\setminus\{v\})$ has order $q-1$ and avoids at least $h-q\ge d+q/2\ge d+1$ [sets](set-split.md). Thus in a minimal counterexample $S$ is independent, and every isolated [vertex](vertex-graph-theory.md) outside $S$ belongs to a singleton branch [set](set-split.md).

Consider a [rooted separation of a graph](rooted-separation-of-a-graph.md) $(A,B)$ of order exactly $q$ avoiding at least $d+1$ branch [sets](set-split.md), and put $S'=A\cap B$. Restrict to $G'=G[B]-E(G[S'])$ and $C'_i=C_i\cap B$. Each $C'_i$ is nonempty: any $C_i$ not itself avoided is adjacent to at least one of the $d+1$ avoided [sets](set-split.md), and the endpoint of such an [edge](edge-of-a-graph.md) in $C_i$ must lie in $B$. If a [graph component](component-graph-theory.md) of $G'[C'_i]$ misses $S'$, it lies in $B\setminus A$ and is a whole [graph component](component-graph-theory.md) of $G[C_i]$, with no [vertex](vertex-graph-theory.md) of $S$. The original hypothesis then forces $G[C_i]$ to be connected and $C'_i=C_i$, entirely outside $A$. Thus each restricted [set](set-split.md) is connected or all its [graph components](component-graph-theory.md) meet $S'$. In particular every $C'_j$ missing $S'$ equals an original [set](set-split.md) outside $A$, so all its required adjacencies from $C'_i$ persist.

A [rooted separation of a graph](rooted-separation-of-a-graph.md) $(A',B')$ of $G'$ avoiding $d+1$ restricted [sets](set-split.md) lifts to $(A\cup A',B')$ in $G$, of the same order: an avoided restricted [set](set-split.md) misses $S'$, hence is an original [set](set-split.md) outside $A$. The [edges](edge-of-a-graph.md) removed inside $S'$ do not obstruct lifting, since $S'\subseteq A'$. This proves the required separation hypothesis for $G'$. If $G'$ is smaller, [induction](mathematical-induction.md) gives the desired connected [sets](set-split.md) rooted at $S'$. Moreover $G[A]$ has $q$ disjoint [graph paths](path-in-a-graph.md) from $S$ to $S'$, by the [Menger theorem](menger-theorem.md). Indeed a separator of smaller order between these [sets](set-split.md) would give a [rooted separation of a graph](rooted-separation-of-a-graph.md) of $G$ of smaller order still avoiding those $d+1$ original [sets](set-split.md). Truncate the [graph paths](path-in-a-graph.md) at their first visits to $S'$, label their endpoints accordingly, and adjoin each [graph path](path-in-a-graph.md) to the corresponding rooted connected [set](set-split.md). They meet $B$ only in their distinct endpoints, so this gives the desired [sets](set-split.md) for $G$, a contradiction. Consequently in a minimal counterexample every such separation of order $q$ has $B=V(G)$ and $A=S$, an [independent set](independent-set-graph-theory.md).

Now contract any [edge](edge-of-a-graph.md) whose endpoints do not belong to two different branch [sets](set-split.md). Its endpoints cannot both lie in $S$, so the image of $S$ still has size $q$. The branch-set conditions persist. If the contraction created a forbidden [rooted separation of a graph](rooted-separation-of-a-graph.md) of order below $q$, its lift would have order below $q$, except possibly when the contracted [vertex](vertex-graph-theory.md) lies in its separator. In that case the lifted order increases by one and is at most $q$. Equality would put the contracted [edge](edge-of-a-graph.md) inside $A$, contradicting the just-proved independence of $A$ for an order-$q$ separation avoiding $d+1$ [sets](set-split.md). Thus the separation hypothesis also persists. Applying [induction](mathematical-induction.md) in the contracted [graph](graph-split.md) and expanding the contracted [vertex](vertex-graph-theory.md) would produce the required disjoint connected [sets](set-split.md). Hence **every [edge](edge-of-a-graph.md) in a minimal counterexample joins two different branch [sets](set-split.md)**.

Every [vertex](vertex-graph-theory.md) outside the branch [sets](set-split.md) would be isolated, since every [edge](edge-of-a-graph.md) joins two branch [sets](set-split.md); such an isolated [vertex](vertex-graph-theory.md) could be deleted. Thus the branch [sets](set-split.md) cover the [graph](graph-split.md). Each nonsingleton branch [set](set-split.md) is therefore an [independent set](independent-set-graph-theory.md), and all its [vertices](vertex-graph-theory.md) belong to $S$, because each of its singleton [graph components](component-graph-theory.md) must meet $S$. Let $C$ be the union of the nonsingleton branch [sets](set-split.md), and write $c=|C|\le q$. There is a [matching in a graph](matching-graph-theory.md) from $C$ into $V(G)\setminus S$. Otherwise the [Hall marriage theorem](hall-s-marriage-theorem.md) gives $X\subseteq C$ with neighbourhood $Y\subseteq V(G)\setminus S$ satisfying $|Y|<|X|$. Since $S$ is independent, $(S\cup Y,V(G)\setminus X)$ is a [rooted separation of a graph](rooted-separation-of-a-graph.md) of order $q-|X|+|Y|<q$. It avoids every singleton branch [set](set-split.md) outside $S\cup Y$, of which there are at least

$$
|V(G)|-q-|Y|\ge |V(G)|-q-c+1\ge h-\frac c2-q+1\ge h-\frac{3q}2+1\ge d+1.
$$

The penultimate counting bound uses that the nonsingleton [sets](set-split.md) number at most $c/2$, so $|V(G)|-c\ge h-c/2$. This contradicts the separation hypothesis.

Use that [matching in a graph](matching-graph-theory.md) to make a two-vertex connected [set](set-split.md) for each terminal in $C$; terminals outside $C$ remain singleton [sets](set-split.md). There are at least

$$
|V(G)|-q-c\ge h-\frac{3q}2=m-q
$$

unused [vertices](vertex-graph-theory.md), all singleton original branch [sets](set-split.md). Choose $m-q$ of them for the remaining $D_i$. Every rooted $D_i$ contains a singleton original branch [set](set-split.md): either its terminal, or its terminal's matched [neighbour](neighbour-of-a-vertex.md). That singleton misses at most $d$ of the selected nonterminal singleton [sets](set-split.md). This constructs the desired family and completes the proof.

## ↑ Ancestors (6)

1. [Graph minor](graph-minor.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/3/solution.md)
- [Rooted dense minor linkage](rooted-dense-minor-linkage.md)
