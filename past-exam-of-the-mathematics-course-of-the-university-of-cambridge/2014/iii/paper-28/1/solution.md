<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Give each nearest-neighbor [edge](../../../../../edge-of-a-graph.md) of the [cubic lattice](../../../../../cubic-lattice.md) an independent [Bernoulli distribution](../../../../../bernoulli-distribution.md) state, open with [probability](../../../../../probability.md) $p$. The resulting [product measure](../../../../../product-measure.md) is denoted $\mathbb P_p$. In this [bond percolation](../../../../../bond-percolation-split.md) model, $C(0)$ is the [percolation cluster](../../../../../percolation-cluster.md) of the origin, and

$$
\theta_d(p)=\mathbb P_p(|C(0)|=\infty),\qquad
\boxed{p_c(d)=\inf\{p\in[0,1]:\theta_d(p)>0\}.}
$$

The uniform-label [monotone coupling of Bernoulli percolation](../../../../../monotone-coupling-of-bernoulli-percolation.md) shows that $\theta_d$ is increasing.

Let $c_n(d)$ count $n$-step [self-avoiding walks](../../../../../self-avoiding-walk.md) starting at the origin, with $c_0(d)=1$. Splitting a walk after $n$ steps, and discarding the avoidance constraint between the two pieces, gives $c_{n+m}(d)\leq c_n(d)c_m(d)$. The [Fekete lemma](../../../../../fekete-s-lemma.md) therefore gives the [connective constant](../../../../../connective-constant.md)

$$
\boxed{\mu(d)=\lim_{n\to\infty}c_n(d)^{1/n}
=\inf_{n\geq1}c_n(d)^{1/n}.}
$$

The [locally finite graph](../../../../../locally-finite-graph.md) structure means that an infinite [percolation cluster](../../../../../percolation-cluster.md) at the origin supplies an open [self-avoiding walk](../../../../../self-avoiding-walk.md) of every length. Each specified walk has $n$ distinct [edges](../../../../../edge-of-a-graph.md) and is open with [probability](../../../../../probability.md) $p^n$. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\theta_d(p)\leq c_n(d)p^n.
$$

For $p\mu(d)<1$ the right side tends to zero. Hence the [connective-constant lower bound for percolation](../../../../../connective-constant-lower-bound-for-percolation.md) is $p_c(d)\geq\mu(d)^{-1}$.

For the upper bound first work on the [square lattice](../../../../../square-lattice.md). A finite open [percolation cluster](../../../../../percolation-cluster.md) has an outer boundary containing a simple closed [graph cycle](../../../../../cycle-in-a-graph.md) of dual [edges](../../../../../edge-of-a-graph.md), all crossing closed primal [edges](../../../../../edge-of-a-graph.md). Such a [dual bond percolation](../../../../../dual-bond-percolation.md) circuit separates that cluster from infinity. Write $N_\ell$ for the number of simple dual circuits of length $\ell$ surrounding the origin. Each circuit meets the positive horizontal ray at distance at most $\ell$: its bounding box contains the origin and its diameter is bounded by its length. Choose such an intersection as an anchor and orient the circuit. Removing its last edge leaves a rooted [self-avoiding walk](../../../../../self-avoiding-walk.md) of length $\ell-1$ in the translated [square lattice](../../../../../square-lattice.md). Consequently, for an absolute constant $K$,

$$
N_\ell\leq K\ell c_{\ell-1}(2).
$$

The exact constant and this possible overcount do not matter. If $(1-p)\mu(2)<1$, the [root test](../../../../../root-test.md) gives

$$
\sum_{\ell\geq L}N_\ell(1-p)^\ell\longrightarrow0
\quad\text{as }L\longrightarrow\infty.
$$

A summable circuit count alone need not give a total sum below one. To use its tail correctly, let $B_R=[-R,R]^2\cap\mathbb Z^2$ and condition every [edge](../../../../../edge-of-a-graph.md) internal to $B_R$ to be open. This finite event has positive [probability](../../../../../probability.md). A closed dual circuit surrounding all of $B_R$ crosses no internal [edge](../../../../../edge-of-a-graph.md) of $B_R$, and so its closed-edge [probability](../../../../../probability.md) remains $(1-p)^\ell$ under this conditioning. Its length tends to infinity with $R$. Choose $R$ so large that the [union bound](../../../../../boole-s-inequality.md) for all such circuits is below one. With positive conditional [probability](../../../../../probability.md), none occurs.

On that event, $C(0)$ contains $B_R$ and cannot be finite: a finite cluster containing $B_R$ would have an enclosing closed dual circuit. Thus $\theta_2(p)>0$ whenever $p>1-\mu(2)^{-1}$. This is the [connective-constant Peierls bound](../../../../../connective-constant-peierls-bound.md), proved by excluding short circuits through the open-box conditioning. An embedded coordinate plane in the [cubic lattice](../../../../../cubic-lattice.md) has exactly the same [bond percolation](../../../../../bond-percolation-split.md) law as the [square lattice](../../../../../square-lattice.md), so $p_c(d)\leq p_c(2)$. Together,

$$
\boxed{\frac1{\mu(d)}\leq p_c(d)\leq1-\frac1{\mu(2)}.}
$$

There are $2d$ choices for the first step of a [self-avoiding walk](../../../../../self-avoiding-walk.md) and at most $2d-1$ thereafter, because immediate reversal is forbidden. Hence $c_n(d)\leq2d(2d-1)^{n-1}$ and $\mu(d)\leq2d-1$. In particular $\mu(2)\leq3$. Substituting with the correct directions of the inequalities gives

$$
\boxed{\frac1{2d-1}\leq p_c(d)\leq\frac23.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
