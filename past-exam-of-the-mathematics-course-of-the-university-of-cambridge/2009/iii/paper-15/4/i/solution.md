<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $G=\Lambda$ be the [martini lattice](../../../../../../martini-lattice.md) and $G^*$ its [planar dual graph](../../../../../../planar-dual-graph.md). Write $c=p_c^b(G)$ and $c^*=p_c^b(G^*)$. Both are periodic, connected, bounded-degree plane graphs with bounded face sizes. [Dual bond percolation](../../../../../../dual-bond-percolation.md) declares a dual bond open exactly when its crossing primal bond is closed, giving independent dual parameter $1-p$.

First, **$c+c^*\le1$**. Suppose instead that the sum exceeds $1$, and choose $1-c^*<p<c$. Both the primal model at $p$ and the dual model at $1-p$ are strictly subcritical. [Sharpness of the percolation transition](../../../../../../sharpness-of-the-percolation-transition.md) gives exponential connection-radius decay on each periodic graph, uniformly over its finitely many vertex types. A crossing of a rectangle of side lengths proportional to $R$ starts at one of $O(R)$ boundary vertices and travels distance of order $R$. A union bound therefore shows that each crossing [probability](../../../../../../probability.md) tends to zero. But [planar duality for rectangle crossings](../../../../../../planar-duality-for-rectangle-crossings.md) says that exactly one of an open primal left-to-right crossing and an open dual top-to-bottom crossing occurs, using the complementary boundary convention. Their [probabilities](../../../../../../probability.md) sum to $1$. This contradiction proves the first inequality.

For the opposite inequality, we need noncoexistence of primal and dual [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md). The four-fold version in Q3(iii) cannot be assumed without change: this decorated [honeycomb lattice](../../../../../../honeycomb-lattice.md) has three-fold rotation symmetry. Here is the necessary [three-fold symmetric primal-dual noncoexistence](../../../../../../three-fold-symmetric-primal-dual-noncoexistence.md) argument.

Assume both models percolate at complementary parameters $p,1-p$. For a large disc, the probability of having no exterior infinite arm is at most $\varepsilon$ in each model. Divide its boundary into six arcs by splitting each $120$-degree sector at the same relative angle. In the primal model let $a,b$ be the failure [probabilities](../../../../../../probability.md) for the two alternating arc types. Rotation symmetry and the [FKG inequality](../../../../../../fkg-inequality.md) give

$$
a^3b^3\le\varepsilon,\qquad ab\le\varepsilon^{1/3}.
$$

Slide the splitting point across one sector. Initially the first arc is empty; finally the second is empty. A jump occurs only when an arc gains or loses an edge-crossing point. An arm using that point requires its crossing bond to be open. The [FKG inequality](../../../../../../fkg-inequality.md) therefore ensures that a failure [probability](../../../../../../probability.md) changes by at most a factor $(1-p)^{-1}$ at a single jump: for a newly added arm event $L_x$, $\mathbb P(L_x^c)\ge1-p$ and $\mathbb P(L^c\cap L_x^c)\ge(1-p)\mathbb P(L^c)$. At the first reversal of the order of $a,b$, their ratio is consequently at most $(1-p)^{-2}$. At that splitting point,

$$
\max\{a,b\}\le(1-p)^{-1}\varepsilon^{1/6}.
$$

Thus every one of the six primal arcs has an exterior arm with [probability](../../../../../../probability.md) tending to $1$. On the same six arcs the dual failure [probabilities](../../../../../../probability.md) $a^*,b^*$ satisfy $a^*b^*\le\varepsilon^{1/3}$, so at least one dual arc type has failure at most $\varepsilon^{1/6}$; its three rotations have the same bound. Take two of those dual arcs separated by one arc, and the two intervening primal arcs. A union bound gives four alternating primal/dual infinite exterior arms with positive [probability](../../../../../../probability.md) when $\varepsilon$ is sufficiently small. The separation and finite-closure argument of Q3(iii), together with [percolation uniqueness on an amenable quasi-transitive graph](../../../../../../percolation-uniqueness-on-an-amenable-quasi-transitive-graph.md), gives a contradiction. This proves noncoexistence. The arc balancing is the extra step needed for three-fold symmetry; it is also developed in [Bollobás and Riordan's original paper on dual lattices](https://arxiv.org/abs/math/0606149).

If $c+c^*<1$, choose $c<p<1-c^*$. Both complementary models would then percolate, contradicting noncoexistence. Hence $c+c^*\ge1$. Combining the two inequalities proves **the dual threshold relation**:

$$
\boxed{p_c^b(\Lambda)+p_c^b(\Lambda^*)=1.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
