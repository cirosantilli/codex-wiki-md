<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [self-avoiding walk](../../../../../self-avoiding-walk.md) of length $n$ is a sequence of $n+1$ distinct [graph vertices](../../../../../vertex-graph-theory.md) joined consecutively by [edges](../../../../../edge-of-a-graph.md). Split a rooted [self-avoiding walk](../../../../../self-avoiding-walk.md) of length $m+n$ after $m$ steps. There are $\kappa_m$ possible prefixes; each remaining segment is a self-avoiding $n$-step walk from its current [graph vertex](../../../../../vertex-graph-theory.md), and forbidding intersections with the prefix can only reduce its count below $\kappa_n$. [Translation invariance](../../../../../translation-invariance.md) therefore gives

$$
\kappa_{m+n}\le\kappa_m\kappa_n.
$$

Apply the [Fekete lemma](../../../../../fekete-s-lemma.md), proved in Question 4(a), to $\log\kappa_n$. It gives $\log\mu=\inf_n n^{-1}\log\kappa_n$ and hence existence of the [connective constant](../../../../../connective-constant.md). Walks using only the $d$ positive coordinate directions never revisit a [graph vertex](../../../../../vertex-graph-theory.md), so there are at least $d^n$. A walk has $2d$ choices for its first step and at most $2d-1$ subsequently because immediate reversal is forbidden. Thus

$$
d^n\le\kappa_n\le2d(2d-1)^{n-1},\qquad\boxed{d\le\mu\le2d-1.}
$$

For independent [bond percolation](../../../../../bond-percolation-split.md), let $C(0)$ be the [percolation cluster](../../../../../percolation-cluster.md) of the origin, $\theta(p)=P_p(|C(0)|=\infty)$, and $p_c=\inf\{p:\theta(p)>0\}$. An [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) in a locally finite [graph](../../../../../graph-split.md) contains an open self-avoiding path of every length. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\theta(p)\le\kappa_np^n.
$$

When $p\mu<1$, the right-hand side tends to zero, since its $n$th root tends to $p\mu$. Hence the [connective-constant lower bound for percolation](../../../../../connective-constant-lower-bound-for-percolation.md) is

$$
\boxed{p_c\ge\mu^{-1}.}
$$

For the upper bound in two dimensions, use the square [planar dual graph](../../../../../planar-dual-graph.md). Call a dual [edge](../../../../../edge-of-a-graph.md) available when its crossing primal [edge](../../../../../edge-of-a-graph.md) is closed. Each dual [edge](../../../../../edge-of-a-graph.md) is available with [probability](../../../../../probability.md) $q=1-p$, independently. The [planar graph](../../../../../planar-graph.md) boundary lemma says that a finite primal [percolation cluster](../../../../../percolation-cluster.md) is enclosed by a [graph cycle](../../../../../cycle-in-a-graph.md) consisting of such [edges](../../../../../edge-of-a-graph.md): its external [edge](../../../../../edge-of-a-graph.md) boundary gives this [graph cycle](../../../../../cycle-in-a-graph.md). We show that $q\mu<1$ guarantees positive percolation [probability](../../../../../probability.md).

Let $N_n$ count enclosing [graph cycles](../../../../../cycle-in-a-graph.md) of length $n$. Because the origin lies inside their coordinate bounding box and their diameter is at most $n$, every such [graph cycle](../../../../../cycle-in-a-graph.md) has a [graph vertex](../../../../../vertex-graph-theory.md) within a box of side $2n+3$. From each possible root, the first $n-1$ [edges](../../../../../edge-of-a-graph.md) give a [self-avoiding walk](../../../../../self-avoiding-walk.md); the final closing [edge](../../../../../edge-of-a-graph.md) is then determined. Dropping the closure restriction gives the convenient bound

$$
N_n\le(2n+3)^2\kappa_{n-1}.
$$

Choose $\rho$ with $q\mu<\rho<1$. The connective-constant [limit of a sequence](../../../../../limit-of-a-sequence.md) implies $\kappa_{n-1}q^n\le C\rho^n$. Consequently the large-circuit tail

$$
\sum_{n\ge L}N_nq^n\longrightarrow0\qquad(L\to\infty)
$$

is summable.

Condition all primal [edges](../../../../../edge-of-a-graph.md) inside a large square $[-L,L]^2$ to be open; this event has positive [probability](../../../../../probability.md). The origin [percolation cluster](../../../../../percolation-cluster.md) then contains that square. If it is finite, its enclosing [graph cycle](../../../../../cycle-in-a-graph.md) has length at least $L$. A proposed [graph cycle](../../../../../cycle-in-a-graph.md) using a pinned-open [edge](../../../../../edge-of-a-graph.md) now has [conditional probability](../../../../../conditional-probability.md) zero; every other proposed [graph cycle](../../../../../cycle-in-a-graph.md) still has [probability](../../../../../probability.md) $q^n$ by [independence of random variables](../../../../../independent-random-variables.md). For $L$ large enough the [union bound](../../../../../boole-s-inequality.md) for the remaining [graph cycles](../../../../../cycle-in-a-graph.md) is less than one. There is therefore positive [conditional probability](../../../../../conditional-probability.md) that the origin [percolation cluster](../../../../../percolation-cluster.md) is infinite. This proves the [connective-constant Peierls bound](../../../../../connective-constant-peierls-bound.md) without needing the exact value of $p_c$:

$$
\boxed{p_c\le1-\mu^{-1}\quad(d=2).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
