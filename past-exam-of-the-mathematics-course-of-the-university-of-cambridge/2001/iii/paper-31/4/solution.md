<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The all-to-one [shortest path problem](../../../../../shortest-path-problem.md) asks for the minimum length $v_i$ of a [directed path](../../../../../directed-path.md) from every [vertex](../../../../../vertex-graph-theory.md) $i$ to the root $n$, with $v_n=0$ and $v_i=\infty$ if no such [directed path](../../../../../directed-path.md) exists. Positive [directed edge](../../../../../directed-edge.md) lengths allow [directed cycles](../../../../../directed-cycle.md) to be deleted, so a shortest [directed path](../../../../../directed-path.md), when one exists, uses at most $n-1$ [directed edges](../../../../../directed-edge.md). Its optimality equations are

$$
v_i=\min_{(i,j)\in A}(c_{ij}+v_j),\qquad i\ne n.
$$

A [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) initializes $d_n^{(0)}=0$ and other labels to infinity, then repeats

$$
d_i^{(k)}=\min\left\{d_i^{(k-1)},\min_{(i,j)\in A}(c_{ij}+d_j^{(k-1)})\right\},
$$

keeping the root label zero. Induction on $k$ proves that $d_i^{(k)}$ is the least length among [directed paths](../../../../../directed-path.md) using at most $k$ [directed edges](../../../../../directed-edge.md): either the old best [directed path](../../../../../directed-path.md) remains, or the first [directed edge](../../../../../directed-edge.md) is followed by a [directed path](../../../../../directed-path.md) with at most $k-1$ [directed edges](../../../../../directed-edge.md). Thus $n-1$ rounds give the exact distances. An in-place variant repeatedly relaxes $d_i\leftarrow\min(d_i,c_{ij}+d_j)$; each decreased label triggers further incoming-arc relaxations. It terminates when no finite label can improve. The [Bellman inequalities](../../../../../bellman-inequalities.md) then telescope along each [directed path](../../../../../directed-path.md) to show the labels are lower bounds on all [directed path](../../../../../directed-path.md) lengths, while every finite label represents a discovered [directed path](../../../../../directed-path.md) and is an upper bound on the optimum. This proves correctness. The method is a [label-correcting shortest-path algorithm](../../../../../label-correcting-shortest-path-algorithm.md): a processed label can be revised many times. Full scans cost $O(n|A|)$.

Let $d=\min_{i\ne n}c_{in}$ and choose $j$ attaining it. Every [directed path](../../../../../directed-path.md) from a nonroot [vertex](../../../../../vertex-graph-theory.md) to $n$ has a final [directed edge](../../../../../directed-edge.md) costing at least $d$, and all preceding [directed edges](../../../../../directed-edge.md) have positive lengths. Therefore every $v_k\ge d$. The direct [directed edge](../../../../../directed-edge.md) from $j$ to $n$ has length $d$, so

$$
\boxed{v_j=c_{jn}=d\le v_k\quad(k\ne n).}
$$

If no incoming root [directed edge](../../../../../directed-edge.md) exists, all these distances are infinite and there is no finite next [vertex](../../../../../vertex-graph-theory.md) to settle.

The all-to-one [Dijkstra algorithm](../../../../../dijkstra-algorithm.md) sets the root's label to zero and all others to infinity. Repeatedly choose an unsettled [vertex](../../../../../vertex-graph-theory.md) $j$ with least finite label, make that label permanent, and relax every incoming [directed edge](../../../../../directed-edge.md) $(i,j)$ of an unsettled [vertex](../../../../../vertex-graph-theory.md):

$$
d_i\leftarrow\min\{d_i,c_{ij}+d_j\}.
$$

Store the corresponding successor $j$ whenever the label improves. Stop when all [vertices](../../../../../vertex-graph-theory.md) are settled or every remaining label is infinite. This applies the usual source version to the reversed [graph](../../../../../graph-split.md); relaxing outgoing original [directed edges](../../../../../directed-edge.md) would solve the wrong direction of the problem.

For its correctness, inductively assume every settled distance is exact. Any [directed path](../../../../../directed-path.md) from an unsettled [vertex](../../../../../vertex-graph-theory.md) to the root must first enter the settled set at some [vertex](../../../../../vertex-graph-theory.md) $w$, through an [directed edge](../../../../../directed-edge.md) $(z,w)$. That [directed edge](../../../../../directed-edge.md) has already been relaxed, so $d_z\le c_{zw}+v_w$. The newly selected label $d_j$ is no greater than $d_z$. The [directed path](../../../../../directed-path.md)'s preceding nonnegative lengths therefore make its total length at least $d_j$. On the other hand, $d_j$ itself is the length of a discovered [directed path](../../../../../directed-path.md). Hence $d_j=v_j$, and it can never need correction. This is a [label-setting shortest-path algorithm](../../../../../label-setting-shortest-path-algorithm.md). Straight array selection costs $O(n^2+|A|)$.

For four [vertices](../../../../../vertex-graph-theory.md) and root 4, the full symbolic execution is as follows. After settling 4, the tentative labels are $(c_{14},c_{24},c_{34},0)$. Select

$$
j\in\operatorname*{argmin}_{i\in\{1,2,3\}}c_{i4},
$$

set $v_j=c_{j4}$, and update the two other labels to $d_i=\min\{c_{i4},c_{ij}+c_{j4}\}$. Select the smaller of those labels at [vertex](../../../../../vertex-graph-theory.md) $k$, set $v_k=d_k$, then for the last [vertex](../../../../../vertex-graph-theory.md) $\ell$ set

$$
\boxed{v_\ell=\min\{c_{\ell4},c_{\ell j}+c_{j4},c_{\ell k}+v_k\}.}
$$

The stored successors give the corresponding shortest routes; infinity conventions handle missing [directed edges](../../../../../directed-edge.md) and disconnected [vertices](../../../../../vertex-graph-theory.md).

**The supplied PDF contains no visible network diagram or [directed edge](../../../../../directed-edge.md) lengths in the space for this example, and the converted TeX omits the diagram as well. Numerical distances and route choices cannot be determined from the supplied data.** The symbolic run above gives the exact four-node calculation once those lengths are available; no network has been guessed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
