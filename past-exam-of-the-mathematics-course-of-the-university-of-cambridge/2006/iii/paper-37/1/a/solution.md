<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Orient the unique path from $s$ to $t$ in a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) $T$, and put $j^T_{xy}=1$ when it uses the [edge](../../../../../../edge-of-a-graph.md) from $x$ to $y$, $-1$ when it uses the reverse direction, and zero otherwise. Then the proposed current is $i_{xy}=\mathbb E j^T_{xy}$; set it to zero on nonedges. It is antisymmetric.

For each [tree](../../../../../../tree-graph-theory.md) path, every intermediate [graph vertex](../../../../../../vertex-graph-theory.md) has one incoming and one outgoing path [edge](../../../../../../edge-of-a-graph.md), while the source has one outgoing [edge](../../../../../../edge-of-a-graph.md) and the sink one incoming [edge](../../../../../../edge-of-a-graph.md). Hence

$$
\sum_y j^T_{xy}=1_{x=s}-1_{x=t}.
$$

Taking [expectations](../../../../../../expected-value.md) gives

$$
\boxed{\sum_y i_{xy}=1_{x=s}-1_{x=t},}
$$

the [Kirchhoff node law](../../../../../../kirchhoff-node-law.md) for a [unit flow](../../../../../../unit-flow.md).

To establish the [Kirchhoff cycle law](../../../../../../kirchhoff-cycle-law.md), it is not enough to check it separately for each [tree](../../../../../../tree-graph-theory.md) path: those path currents need not satisfy the voltage law on the original [graph](../../../../../../graph-split.md). Instead, let $\mathcal T$ be all [spanning trees](../../../../../../spanning-tree.md) and let $\mathcal F_{st}$ be all spanning forests with two components, one containing $s$ and the other $t$. For $F\in\mathcal F_{st}$ denote the source component by $C_s(F)$.

For an existing [edge](../../../../../../edge-of-a-graph.md) $xy$, deleting it from a [tree](../../../../../../tree-graph-theory.md) whose $s$-$t$ path uses $x\to y$ produces precisely a forest $F\in\mathcal F_{st}$ with $x\in C_s(F)$ and $y\notin C_s(F)$. Conversely, adding $xy$ to any such forest produces exactly that [tree](../../../../../../tree-graph-theory.md) and path orientation. This is a bijection. Applying it to both orientations gives

$$
i_{xy}=\frac1{|\mathcal T|}\sum_{F\in\mathcal F_{st}}\left(1_{x\in C_s(F)}-1_{y\in C_s(F)}\right).
$$

Define $h(x)=|\mathcal T|^{-1}\sum_F1_{x\in C_s(F)}$. Then $i_{xy}=h(x)-h(y)$ on every [edge](../../../../../../edge-of-a-graph.md). Since the resistances are one, this is [Ohm's law](../../../../../../ohm-s-law.md), and the voltage drops telescope around every oriented cycle:

$$
\boxed{\sum_{xy\text{ along a cycle}}i_{xy}=0.}
$$

Together with the node law, this proves that the mean tree-path current is the electrical unit current. This argument is the [mean spanning-tree path current](../../../../../../mean-spanning-tree-path-current.md) identity.

For clarity, these laws determine the current uniquely. The difference of two solutions is a potential gradient $k(x)-k(y)$ with zero divergence. Multiplying its divergence by $k(x)$ and summing over [graph vertices](../../../../../../vertex-graph-theory.md) gives $\sum_{\{x,y\}}(k(x)-k(y))^2=0$. Thus every difference current is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
