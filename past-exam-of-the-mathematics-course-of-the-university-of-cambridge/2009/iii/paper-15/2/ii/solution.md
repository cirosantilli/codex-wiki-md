<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $q=1-p<1/2$. Declare a bond of the [planar dual graph](../../../../../../planar-dual-graph.md) open when its crossing primal bond is closed. These states have the independent [dual bond percolation](../../../../../../dual-bond-percolation.md) law with parameter $q$; the dual [square lattice](../../../../../../square-lattice.md) is a translate of the primal [square lattice](../../../../../../square-lattice.md). Part (i) supplies an $a=a(q)>0$ such that

$$
\mathbb P_q(|C_y^*|\ge m)\le e^{-am},\qquad m\ge2.
$$

In particular every dual cluster is finite almost surely.

Suppose the primal [percolation cluster](../../../../../../percolation-cluster.md) $C_0$ is finite. Fill its finite complementary holes. Every bond on the resulting outer boundary is closed, since an open bond leaving the cluster would reach another cluster vertex. The crossing dual bonds form a connected enclosing contour, possibly touching itself, contained in one dual cluster $K$. This is the [dual contour bound for a finite planar cluster](../../../../../../dual-contour-bound-for-a-finite-planar-cluster.md). If $m=|K|$, a connected set of $m$ square-lattice dual vertices has each coordinate width at most $m-1$. All vertices of $C_0$ lie inside the enclosing contour, so

$$
|C_0|\le m^2.
$$

Moreover the contour surrounds $0$ and the diameter of $K$ is at most $m-1$ in the graph distance. Thus every vertex of $K$ lies in the square of radius $m+1$ about $0$. There are at most $(2m+3)^2$ possible dual vertices in that square, with a harmless enlargement if a boundary convention requires it.

On $\{n\le|C_0|<\infty\}$ there is therefore an integer $m\ge\lceil\sqrt n\rceil$ and a dual vertex in that square whose dual cluster has size exactly $m$. The enclosing contour has at least four vertices. A union bound and part (i) give

$$
\mathbb P_p(n\le|C_0|<\infty)\le\sum_{m\ge\max\{4,\lceil\sqrt n\rceil\}}(2m+3)^2e^{-am}\le C_1 e^{-c_1\sqrt n},
$$

for constants $C_1,c_1>0$ depending only on $q$. The last estimate follows by bounding the polynomial factor by a constant times $e^{am/2}$ and summing a [geometric series](../../../../../../geometric-series.md). This explains the square root: an enclosing dual cluster must have size at least the square root of the primal volume.

For $p<1$, the [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md) and $p>p_c$ imply $\theta(p)>0$, so $v:=\mathbb P_p(|C_0|<\infty)=1-\theta(p)<1$. Choose $N$ with $\log C_1\le(c_1/2)\sqrt N$. For $n\ge N$ use the preceding bound; for $1\le n\le N$ use the bound $v$. The positive constant $b=\min\{c_1/2,-\log v/\sqrt N\}$ gives **the required conclusion**:

$$
\boxed{\mathbb P_p(n\le|C_0|<\infty)\le e^{-b\sqrt n}\quad(n\ge1).}
$$

For $p=1$ the event is empty, so any $b>0$ works.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
