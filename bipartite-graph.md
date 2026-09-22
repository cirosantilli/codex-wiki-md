# Bipartite graph

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bipartite_graph)

A [bipartite graph](bipartite-graph.md) separates its [vertices](vertex-graph-theory.md) into two [independent sets](independent-set-graph-theory.md): every [edge](edge-of-a-graph.md) goes from one part to the other. Here $G=(V,E)$ is a finite [simple graph](simple-graph.md) and an [undirected graph](undirected-graph.md), with no [self-loops](loop-graph-theory.md) and no repeated [edges](edge-of-a-graph.md). The two parts $X,Y\subseteq V$ satisfy

$$
X\cap Y=\varnothing,\qquad X\cup Y=V,\qquad \{u,v\}\in E\Longrightarrow (u\in X,\ v\in Y)\ \text{or}\ (u\in Y,\ v\in X).
$$

Thus neither part contains an [edge](edge-of-a-graph.md). The parts need not have equal sizes, and some pairs across them may have no [edge](edge-of-a-graph.md); requiring every cross pair gives a [complete bipartite graph](complete-bipartite-graph.md). The [independent set](independent-set-graph-theory.md) and cross-[edge](edge-of-a-graph.md) definitions are equivalent.[Section 1.1, printed p. 3, independent vertices; Section 1.6, printed p. 17, bipartite and complete multipartite graphs](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

For example, the six-[vertex](vertex-graph-theory.md) [cycle graph](cycle-graph.md) $C_6$ with [edges](edge-of-a-graph.md) $12,23,34,45,56,61$ has parts $X=\{1,3,5\}$ and $Y=\{2,4,6\}$. Drawing the same [graph](graph-split.md) as a hexagon or in two columns changes neither its [edges](edge-of-a-graph.md) nor its [bipartite](bipartite-graph.md) property. An extra [isolated vertex](isolated-vertex.md) $z$ can go in either part.

<a id="bipartite-graph-independent-parts"></a>
![](bipartite-graph-independent-parts.png)

**[Figure 32](#bipartite-graph-independent-parts). The same six-cycle and isolated vertex drawn as a cycle and as two independent parts**.

We allow either part to be empty. Consequently a [graph](graph-split.md) with no [edges](edge-of-a-graph.md) is [bipartite](bipartite-graph.md), even when $V=\varnothing$; choose $X=V$, $Y=\varnothing$. Here "two colours" means two colours are available, with no requirement to use both. This convention explicitly includes the empty case, whereas definitions requiring two nonempty classes need an exception. For several [connected components of a graph](component-graph-theory.md), choose the two parts separately in each [graph component](component-graph-theory.md) and take their [unions](set-union.md). In a nonempty [connected graph](connected-graph.md) that is [bipartite](bipartite-graph.md), fixing one [vertex](vertex-graph-theory.md)'s colour forces all others along [graph paths](path-in-a-graph.md), so its two-colour assignment is unique up to swapping the colours. Each [graph component](component-graph-theory.md), including an [isolated vertex](isolated-vertex.md), can be swapped independently.

The [two-colourability criterion for bipartite graphs](two-colourability-criterion-for-bipartite-graphs.md) identifies these parts with the colour classes of a [proper vertex colouring](proper-vertex-coloring.md): assign colour $0$ to $X$ and colour $1$ to $Y$, so adjacent [vertices](vertex-graph-theory.md) have different colours. More surprisingly, the [odd-cycle characterization of bipartite graphs](odd-cycle-characterization-of-bipartite-graphs.md) turns a global requirement into one precise obstruction:

$$
G\text{ is bipartite}\quad\Longleftrightarrow\quad G\text{ contains no odd cycle}.
$$

This statement is for the finite [undirected graph](undirected-graph.md) and [simple graph](simple-graph.md) model above; a [graph cycle](cycle-in-a-graph.md) has distinct [vertices](vertex-graph-theory.md) except for the repeated starting [vertex](vertex-graph-theory.md). Along a [graph cycle](cycle-in-a-graph.md) in a [bipartite graph](bipartite-graph.md), colours alternate, so returning to the starting colour takes an [even number](even-number.md) of [edges](edge-of-a-graph.md). Therefore any [odd cycle](odd-cycle.md), whether or not other [edges](edge-of-a-graph.md) join its [vertices](vertex-graph-theory.md), prevents a [bipartite](bipartite-graph.md) split.[Section 1.6, Proposition 1.6.1 and proof, printed pp. 17–18](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

[Breadth-first search](breadth-first-search.md) supplies the converse constructively. Start an uncoloured [vertex](vertex-graph-theory.md) $s$ with colour $0$, and use a [FIFO queue](fifo-queue.md) to explore its [graph component](component-graph-theory.md). When an [edge](edge-of-a-graph.md) $uv$ first discovers $v$, give $v$ the opposite colour to $u$, record $u$ as its [parent in a rooted tree](parent-in-a-rooted-tree.md), and enqueue $v$. If both endpoints of any scanned [edge](edge-of-a-graph.md) already have the same colour, stop with a conflict. Restart from an uncoloured [vertex](vertex-graph-theory.md) until every [graph component](component-graph-theory.md) has been examined. If no conflict occurs, all [edges](edge-of-a-graph.md) cross the two colour classes, which are the required [independent sets](independent-set-graph-theory.md).[BipartiteX.java](algorithms-4th-edition-by-robert-sedgewick-and-others/bipartitex-java.md)

A conflict also explains the failure. In the [rooted tree](rooted-tree.md) produced by [breadth-first search](breadth-first-search.md), let $d(v)$ be the [graph distance](distance-graph-theory.md) from $s$. The colour of $v$ is its distance's [integer parity](parity-mathematics.md). An [edge](edge-of-a-graph.md) $uv$ in an [undirected graph](undirected-graph.md) satisfies $|d(u)-d(v)|\leq1$, so equal colours force $d(u)=d(v)$. Follow the two parent chains upward to their [lowest common ancestor](lowest-common-ancestor.md) $w$, discard the shared [graph path](path-in-a-graph.md) from $s$ to $w$, and join the remaining two [graph paths](path-in-a-graph.md) with the conflict [edge](edge-of-a-graph.md) $uv$. The result is a genuine [graph cycle](cycle-in-a-graph.md) with

$$
\bigl(d(u)-d(w)\bigr)+\bigl(d(v)-d(w)\bigr)+1=2\bigl(d(u)-d(w)\bigr)+1
$$

[edges](edge-of-a-graph.md), an [odd integer](odd-integer.md). The two branches have no shared [vertices](vertex-graph-theory.md) except $w$, so this is more than a [closed walk](closed-walk.md). This [odd cycle](odd-cycle.md) is a certificate that anyone can check directly, using only its listed [vertices](vertex-graph-theory.md) and [edges](edge-of-a-graph.md).

<a id="bipartite-graph-odd-cycle-certificate"></a>
![](bipartite-graph-odd-cycle-certificate.png)

**[Figure 33](#bipartite-graph-odd-cycle-certificate). A BFS colour conflict closes a five-cycle; the shared root path is excluded from the certificate**.

In the example, [breadth-first search](breadth-first-search.md) from $s$ gives $d(w)=1$, $d(a)=d(b)=2$, and $d(u)=d(v)=3$. The conflict [edge](edge-of-a-graph.md) $uv$ closes the [odd cycle](odd-cycle.md) $w,a,u,v,b,w$, with five [edges](edge-of-a-graph.md). The common [edge](edge-of-a-graph.md) $sw$ is excluded. Thus the same procedure returns either two [independent sets](independent-set-graph-theory.md) covering $V$, or an explicit [odd cycle](odd-cycle.md). With [adjacency lists](adjacency-list.md) and constant-time [FIFO queue](fifo-queue.md) operations, its [time complexity](time-complexity.md) is $O(|V|+|E|)$ in [Big O notation](big-o-notation.md), with $O(|V|)$ additional storage.[BipartiteX.java](algorithms-4th-edition-by-robert-sedgewick-and-others/bipartitex-java.md)

The two parts often have a practical meaning: workers and jobs, with an [edge](edge-of-a-graph.md) exactly when a worker can perform a job. A [matching in a graph](matching-graph-theory.md) chooses compatible worker–job pairs with no reused endpoint; merely being [bipartite](bipartite-graph.md) does not guarantee enough compatible pairs. [Hall's marriage theorem](hall-s-marriage-theorem.md) characterizes when every worker can be matched, and the [assignment problem](assignment-problem.md) adds costs to seek an optimal assignment. These connections make the [bipartite](bipartite-graph.md) structure useful after recognition, as the starting point for selecting [edges](edge-of-a-graph.md) under constraints.

**Table of contents**

- [Crown graph](crown-graph.md)
- [Biadjacency matrix](biadjacency-matrix.md)
- [Normalized adjacency operator of a bipartite graph](normalized-adjacency-operator-of-a-bipartite-graph.md)
- [Biregular graph](biregular-graph.md)
  - [Independent-set bound for biregular graphs](independent-set-bound-for-biregular-graphs.md)
  - [Quasirandom bipartite graph](quasirandom-bipartite-graph.md)
    - [Spectral discrepancy bound for a biregular graph](spectral-discrepancy-bound-for-a-biregular-graph.md)
    - [Centered four-cycle identity for a biregular graph](centered-four-cycle-identity-for-a-biregular-graph.md)
- [Half graph](half-graph.md)
  - [Boundary rank obstruction in a half graph](boundary-rank-obstruction-in-a-half-graph.md)
- [Odd-cycle characterization of bipartite graphs](odd-cycle-characterization-of-bipartite-graphs.md)
- [Complete bipartite graph](complete-bipartite-graph.md)
  - [Common neighbourhood from bipartite density](common-neighbourhood-from-bipartite-density.md)
  - [Star (graph theory)](star-graph-theory.md)
- [Two-colourability criterion for bipartite graphs](two-colourability-criterion-for-bipartite-graphs.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (91)

- [Alternating-cycle perturbation of a doubly stochastic matrix](alternating-cycle-perturbation-of-a-doubly-stochastic-matrix.md)
- [Antiferromagnetic Ising model](antiferromagnetic-ising-model.md)
- [Assignment problem](assignment-problem.md)
- [Biadjacency matrix](biadjacency-matrix.md)
- [Bipartite four-cycle count](bipartite-four-cycle-count.md)
- [Bipartite four-cycle density](bipartite-four-cycle-density.md)
- [Bipartite graph](bipartite-graph.md)
- [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
- [Bipartite Szemerédi regularity lemma](bipartite-szemeredi-regularity-lemma.md)
- [Bipartite vertex cover](bipartite-vertex-cover.md)
- [Biregular graph](biregular-graph.md)
- [Chromatic index bounds](chromatic-index-bounds.md)
- [Chromatic number](chromatic-number.md)
- [Common neighbourhood from bipartite density](common-neighbourhood-from-bipartite-density.md)
- [Dense bipartite common-neighbour lemma](dense-bipartite-common-neighbour-lemma.md)
- [Equality in Sperner theorem](equality-in-sperner-theorem.md)
- [Even-length walk generating function on a bipartite graph](even-length-walk-generating-function-on-a-bipartite-graph.md)
- [Flexible vertex in a balanced bipartite graph](flexible-vertex-in-a-balanced-bipartite-graph.md)
- [Four-step path lemma for a dense bipartite graph](four-step-path-lemma-for-a-dense-bipartite-graph.md)
- [Galvin theorem for bipartite list edge coloring](galvin-theorem-for-bipartite-list-edge-coloring.md)
- [Geometrical frustration](geometrical-frustration.md)
- [Graph form of the Balog-Szemerédi-Gowers theorem](graph-form-of-the-balog-szemeredi-gowers-theorem.md)
- [Graph minor](graph-minor.md)
- [Hypercube graph](hypercube-graph.md)
- [Independence number](independence-number.md)
- [Kernel-perfect directed graph](kernel-perfect-directed-graph.md)
- [List-chromatic index](list-chromatic-index.md)
- [Matching generating function](matching-generating-function.md)
- [Necessary conditions for a Hamilton cycle](necessary-conditions-for-a-hamilton-cycle.md)
- [Nested matching criterion for a regular subgraph](nested-matching-criterion-for-a-regular-subgraph.md)
- [Normalized adjacency operator of a bipartite graph](normalized-adjacency-operator-of-a-bipartite-graph.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/17f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/17f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/17f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/14i/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/14i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-109/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-212/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/15h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/17i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/17i/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/17g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/17g/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/17h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/17h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/17h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-122/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/2/solution.md)
- [Perfect matching](perfect-matching.md)
- [Permanent (mathematics)](permanent-mathematics.md)
- [Popular sum](popular-sum.md)
- [Random bipartite matching from empty-rectangle exclusion](random-bipartite-matching-from-empty-rectangle-exclusion.md)
- [Random cut lower bound](random-cut-lower-bound.md)
- [Regular pair of bipartite partitions](regular-pair-of-bipartite-partitions.md)
- [Restricted sumset](restricted-sumset.md)
- [Sidorenko conjecture](sidorenko-conjecture.md)
- [Simultaneously bipartite graph and complement](simultaneously-bipartite-graph-and-complement.md)
- [Staggered magnetization](staggered-magnetization.md)
- [Triangle replacement for self-avoiding walks](triangle-replacement-for-self-avoiding-walks.md)
- [Tripartite graph](tripartite-graph.md)
- [Two-colourability criterion for bipartite graphs](two-colourability-criterion-for-bipartite-graphs.md)
- [Two-sublattice Ising mean-field approximation](two-sublattice-ising-mean-field-approximation.md)
- [Vertex cover number](vertex-cover-number.md)
