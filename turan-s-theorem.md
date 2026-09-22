<h1 id="turan-s-theorem">Turán's theorem</h1>

↑ **Parent:** [Extremal graph theory](extremal-graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turán's_theorem)

How many [edges](edge-of-a-graph.md) can we retain while excluding a prescribed [clique](clique-graph-theory.md)? For [integers](integer-split.md) $r\geq1$ and $n\geq0$, every [simple graph](simple-graph.md) on $n$ [vertices](vertex-graph-theory.md) containing no [complete subgraph](clique-graph-theory.md) $K_{r+1}$ satisfies

$$
e(G)\leq t_r(n):=e(T_r(n)).
$$

Equality holds exactly for the [Turán graph](turan-graph.md) $T_r(n)$, up to [graph isomorphism](graph-isomorphism.md). Thus the [extremal number](extremal-number.md) is $\operatorname{ex}(n,K_{r+1})=t_r(n)$.[third electronic edition (2005), §7.1, printed p. 165, Theorem 7.1.1; replace the source's forbidden-clique parameter r by r+1](graph-theory-by-reinhard-diestel.md)

For example, $T_3(8)$ has [independent sets](independent-set-graph-theory.md) of sizes $3,3,2$ and $21$ [edges](edge-of-a-graph.md), as counted in [Turán graph](turan-graph.md). It contains [triangles in a graph](triangle-in-a-graph.md), but no four-[vertex](vertex-graph-theory.md) [clique](clique-graph-theory.md). Consequently any [simple graph](simple-graph.md) on eight [vertices](vertex-graph-theory.md) with $22$ [edges](edge-of-a-graph.md) contains $K_4$, while $21$ [edges](edge-of-a-graph.md) alone do not force one. Excluding larger [cliques](clique-graph-theory.md) permits denser [graphs](graph-split.md); [Mantel theorem](mantel-theorem.md) is precisely the first nontrivial case.

A short proof outline uses [Zykov symmetrization](zykov-symmetrization.md). If an extremizer is not a [complete multipartite graph](complete-multipartite-graph.md), it has [vertices](vertex-graph-theory.md) $x,y,z$ with $xy,xz$ absent and $yz$ present. If either $y$ or $z$ has larger [vertex degree](degree-graph-theory.md) than $x$, clone that [vertex](vertex-graph-theory.md) in place of $x$. Otherwise replace both $y,z$ by nonadjacent clones of $x$, gaining $2d(x)-d(y)-d(z)+1>0$ [edges](edge-of-a-graph.md). Both contradict extremality; balancing the resulting at most $r$ parts gives $T_r(n)$.[third electronic edition (2005), §7.1, printed pp. 166–167, vertex duplication and second proof of Theorem 7.1.1](graph-theory-by-reinhard-diestel.md)

The [vertex cloning in a graph](vertex-cloning-in-a-graph.md) step preserves [clique](clique-graph-theory.md) exclusion because any [clique](clique-graph-theory.md) using a clone can substitute its original [vertex](vertex-graph-theory.md); nonadjacent clones cannot occur together in a [clique](clique-graph-theory.md). At most $r$ parts can be nonempty, since selecting one [vertex](vertex-graph-theory.md) from each gives a [clique](clique-graph-theory.md). If fewer than $r$ parts are nonempty and one has at least two [vertices](vertex-graph-theory.md), splitting it creates more [edges](edge-of-a-graph.md), so it cannot be extremal. For $r=1$ the bound is zero. For $r\geq n$, the [Turán graph](turan-graph.md) is $K_n$, and the bound is the total $\binom n2$ possible [edges](edge-of-a-graph.md).

**Table of contents**

- [Edit-distance stability for clique-free graphs](edit-distance-stability-for-clique-free-graphs.md)
  - [Bipartite stability from few odd cycles](bipartite-stability-from-few-odd-cycles.md)
- [Turán graph](turan-graph.md)
  - [Triangle support line between bipartite and tripartite Turan graphs](triangle-support-line-between-bipartite-and-tripartite-turan-graphs.md)
- [Zykov symmetrization](zykov-symmetrization.md)
  - [Edge-triangle symmetrization](edge-triangle-symmetrization.md)
- [Quadratic Turan edge bound](quadratic-turan-edge-bound.md)
- [Rhombus-free edge bound](rhombus-free-edge-bound.md)
  - [Triangular prism graph](triangular-prism-graph.md)

## ↑ Ancestors (6)

1. [Extremal graph theory](extremal-graph-theory-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Chromatic polynomial determines a Turán graph](chromatic-polynomial-determines-a-turan-graph.md)
- [Mantel theorem](mantel-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/17f/solution.md)
- [Turán graph](turan-graph.md)
