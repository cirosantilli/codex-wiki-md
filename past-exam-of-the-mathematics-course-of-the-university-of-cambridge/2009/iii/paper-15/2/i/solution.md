<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We use three precise inputs. The [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md) says that independent [bond percolation](../../../../../../bond-percolation-split.md) on the [square lattice](../../../../../../square-lattice.md) has [percolation critical probability](../../../../../../percolation-critical-probability.md) $p_c=1/2$. [Sharpness of the percolation transition](../../../../../../sharpness-of-the-percolation-transition.md) says that, for every $p<p_c$, there are $c,C>0$ such that $\mathbb P_p(0\leftrightarrow\partial[-R,R]^2)\le Ce^{-cR}$ for all positive integers $R$. Finally, the [BK inequality](../../../../../../van-den-berg-kesten-inequality.md) says that increasing connection events with disjoint bond witnesses have joint [probability](../../../../../../probability.md) at most the product of their individual [probabilities](../../../../../../probability.md). All three statements concern the independent product law used here.

The sharpness bound implies finite [percolation susceptibility](../../../../../../percolation-susceptibility.md). Indeed, with $\tau(u,v)=\mathbb P_p(u\leftrightarrow v)$, summing over square shells gives

$$
\chi:=\mathbb E_p|C_0|=\sum_{v\in\mathbb Z^2}\tau(0,v)\le1+\sum_{R\ge1}8R\,Ce^{-cR}<\infty.
$$

A radius bound alone would give only a square-root exponential volume bound. To obtain the requested exponential volume bound, we prove the [tree-graph moment bound for a percolation cluster](../../../../../../tree-graph-moment-bound-for-a-percolation-cluster.md):

$$
\mathbb E_p|C_0|^k\le (2k-3)!!\,\chi^{2k-1},\qquad k\ge1,
$$

where $(-1)!!=1$.

Expand the left-hand side as a sum over ordered marked vertices $x_1,\ldots,x_k$ of the [probability](../../../../../../probability.md) that $0,x_1,\ldots,x_k$ belong to one open cluster. Whenever that event occurs, a finite open [tree](../../../../../../tree-graph-theory.md) connects the marked vertices. Delete unmarked leaves and suppress unmarked degree-two vertices. Treat a marked internal vertex as a leaf attached by a zero-length connection, and split any higher-degree branch into degree-three branch points, again with zero-length connections. This gives an abstract binary [tree](../../../../../../tree-graph-theory.md) with $k+1$ labelled leaves, $k-1$ branch points and $2k-1$ connections. Its nonempty connecting paths use disjoint sets of open bonds. Coincident marked vertices are allowed: their zero-length connections have empty witnesses.

There are $(2k-3)!!$ such binary [tree](../../../../../../tree-graph-theory.md) topologies. For example, the topology with two leaves is unique; inserting the next labelled leaf subdivides one of the $2k-1$ edges of a topology with $k+1$ leaves, giving the usual double-factorial recursion. For a fixed topology and fixed positions of all its vertices, the [BK inequality](../../../../../../van-den-berg-kesten-inequality.md) bounds the disjoint connection event by the product of the corresponding $\tau$ factors. Sum over all $x_i$ and all branch-point positions. Keep the root fixed, and successively sum a leaf away. Translation invariance gives $\sum_y\tau(z,y)=\chi$ at every step. The resulting sum is $\chi^{2k-1}$. Summing the topologies proves the bound.

Since $(2k-3)!!\le2^{k-1}(k-1)!$, expansion of the exponential, justified by [monotone convergence](../../../../../../monotone-convergence-theorem.md), gives

$$
\mathbb E_p e^{t|C_0|}\le1+\frac1{2\chi}\sum_{k\ge1}\frac{(2t\chi^2)^k}{k}=1-\frac1{2\chi}\log(1-2t\chi^2),\qquad 0<t<\frac1{2\chi^2}.
$$

Take $t=1/(4\chi^2)$ and write $M=1+\log2/(2\chi)$. [Markov's inequality](../../../../../../markov-inequality.md) yields $\mathbb P_p(|C_0|\ge n)\le Me^{-tn}$. To remove the prefactor, choose an integer $N\ge2$ with $tN\ge2\log M$. For $n\ge N$ the bound is at most $e^{-tn/2}$. For $2\le n\le N$, use

$$
\mathbb P_p(|C_0|\ge n)\le\mathbb P_p(|C_0|\ge2)=1-(1-p)^4=:u<1.
$$

For $0<p<1/2$, setting $a=\min\{t/2,-\log u/N\}>0$ therefore proves **the bound with unit prefactor**:

$$
\boxed{\mathbb P_p(|C_0|\ge n)\le e^{-a n}\quad(n\ge2).}
$$

At $p=0$, $|C_0|=1$ and any positive $a$ works.

## ↑ Ancestors (11)

1. [I](../i.md)
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
