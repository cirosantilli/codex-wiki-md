<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [topological graph](../../../../graph-topology.md) consisting of the ray $[0,\infty)$ with [vertices](../../../../vertex-graph-theory.md) $v_n=n$ and one oriented [graph loop](../../../../loop-graph-theory.md) $\ell_n$ attached at each $v_n$, for $n=0,1,2,\ldots$. Set the [base point](../../../../base-point.md) to $b=v_0$. This is a [connected](../../../../connected-space.md), [locally finite graph](../../../../locally-finite-graph.md); it is deliberately infinite.

Define [continuous maps](../../../../continuous-map.md) $f,g:X\to X$ by

$$
\begin{aligned}
f(t)&=t+1&&\text{on the ray},&
f(\ell_n(s))&=\ell_{n+1}(s),\\
g(t)&=\max(t-1,0)&&\text{on the ray},&
g(\ell_n(s))&=\begin{cases}b,&n=0,\\\ell_{n-1}(s),&n\geq1.\end{cases}
\end{aligned}
$$

Here each [graph loop](../../../../loop-graph-theory.md) is parametrized by $s\in[0,1]$ with its endpoints at the attaching [vertex](../../../../vertex-graph-theory.md). The formulas agree at every [vertex](../../../../vertex-graph-theory.md), and their restrictions to every closed [edge](../../../../edge-of-a-graph.md) are [continuous](../../../../continuous-function.md). The [weak topology of a CW complex](../../../../weak-topology-of-a-cw-complex.md) therefore makes $f,g$ [continuous maps](../../../../continuous-map.md). Directly on the ray and on each [graph loop](../../../../loop-graph-theory.md),

$$
\boxed{gf=\operatorname{id}_X.}
$$

We check the two [fundamental group](../../../../fundamental-group.md) maps at exactly the specified [base point](../../../../base-point.md)s. The ray is a [spanning tree](../../../../spanning-tree.md). At $b=v_0$ a [free basis of a group](../../../../free-basis-of-a-group.md) consists of $a_n$, obtained by going along the ray to $v_n$, following $\ell_n$, and returning. At $f(b)=v_1$, use the corresponding [free basis of a group](../../../../free-basis-of-a-group.md) $c_n$ with connecting [paths](../../../../continuous-path.md) starting at $v_1$; in particular $c_0$ travels backwards along the first [edge](../../../../edge-of-a-graph.md) before following $\ell_0$. The standard [spanning tree](../../../../spanning-tree.md) description applies to this infinite [topological graph](../../../../graph-topology.md) as well: every [loop](../../../../loop-topology.md) and every [homotopy](../../../../homotopy-split.md) between [based loops](../../../../based-loop.md) has [compact](../../../../compact-space.md) [image](../../../../image-of-a-function.md), so lies in a finite [subcomplex](../../../../simplicial-subcomplex.md).

The induced [group homomorphisms](../../../../group-homomorphism.md) are

$$
\boxed{f_*(a_n)=c_{n+1},\qquad
g_*(c_0)=1,\quad g_*(c_n)=a_{n-1}\ (n\geq1).}
$$

Thus $f_*$ misses $c_0$: words in $c_1,c_2,\ldots$ cannot equal $c_0$ by the [normal form for free groups and free product of groups](../../../../normal-form-for-free-groups-and-free-product-of-groups.md). Consequently $f_*$ is not [surjective](../../../../surjective-function.md). Meanwhile $c_0$ is a nontrivial [free group](../../../../free-group.md) element killed by $g_*$, so $g_*$ is not [injective](../../../../injective-function.md). **Neither induced map is a [group isomorphism](../../../../group-isomorphism.md)**, while [functoriality of the fundamental group](../../../../functoriality-of-the-fundamental-group.md) correctly gives $g_*f_*=\operatorname{id}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the topology and groups course of the University of Oxford](../../../split.md)
5. [Topology and groups course of the University of Oxford](../../../../topology-and-groups-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
