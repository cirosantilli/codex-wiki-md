<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $\varepsilon>0$ and a finite [epsilon-net](../../../../../../metric-epsilon-net.md) $x_1,\ldots,x_N$ in $X$. Choose a Borel map $r:X\to\{x_1,\ldots,x_N\}$ with $d(x,r(x))\leq\varepsilon$, for example the nearest point with ties broken by index. Its cells $A_i$ give discrete [probability measures](../../../../../../probability-measure.md) with masses $p_i=P(A_i)$ and $q_i=Q(A_i)$. Let

$$
W_\varepsilon=\min\left\{\sum_{i,j}d(x_i,x_j)\pi_{ij}:\pi_{ij}\geq0,\ \sum_j\pi_{ij}=p_i,\ \sum_i\pi_{ij}=q_j\right\}.
$$

The feasible set is nonempty and compact, so the minimum exists. Pushing any [coupling](../../../../../../coupling.md) forward by $(r,r)$ changes its cost by at most $2\varepsilon$, hence $W_\varepsilon\leq W+2\varepsilon$. Conversely, lift a discrete [coupling](../../../../../../coupling.md) by the measure

$$
\sum_{i,j:\,p_iq_j>0}\pi_{ij}\,
\frac{P|_{A_i}}{p_i}\otimes\frac{Q|_{A_j}}{q_j}.
$$

Terms with zero row or column masses vanish. This lift has marginals $P,Q$, and its cost differs by at most $2\varepsilon$. Therefore

$$
|W-W_\varepsilon|\leq2\varepsilon.
$$

Here is the finite [linear programming duality](../../../../../../linear-programming-duality.md) proof. Write $d_{ij}=d(x_i,x_j)$ and consider the [convex cone](../../../../../../convex-cone.md)

$$
C=\left\{\left((\sum_j\pi_{ij})_i,(\sum_i\pi_{ij})_j,\sum_{i,j}d_{ij}\pi_{ij}+s\right):\pi_{ij}\geq0,\ s\geq0\right\}.
$$

It is closed and finitely generated. One elementary justification of closedness is to reduce each nonnegative representation to linearly independent generators, eliminating a coefficient along any linear dependence; after choosing a subsequence using the same subset of generators, their independent coordinates have bounded, convergent coefficients whenever the represented vectors converge. For $\eta>0$, the point $(p,q,W_\varepsilon-\eta)$ lies outside $C$. Separation from this closed [convex cone](../../../../../../convex-cone.md) gives coefficients $(a,b,\tau)$ with

$$
\tau\geq0,\qquad a_i+b_j+\tau d_{ij}\geq0,\qquad
\sum_i a_ip_i+\sum_j b_jq_j+\tau(W_\varepsilon-\eta)<0.
$$

If $\tau=0$, summing the middle inequalities against any feasible $\pi$ contradicts the last one. Thus $\tau>0$, and $f_i=-a_i/\tau$, $g_j=-b_j/\tau$ obey $f_i+g_j\leq d_{ij}$ with dual objective greater than $W_\varepsilon-\eta$. The weak inequality already proved gives the reverse bound. Letting $\eta\downarrow0$ proves finite strong duality.

Reduce this discrete dual to a single [Lipschitz function](../../../../../../lipschitz-continuity.md). For a feasible pair put $\phi_i=\min_j(d_{ij}-g_j)$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $|\phi_i-\phi_l|\leq d_{il}$, while $f_i\leq\phi_i$ and $g_i\leq-\phi_i$. Consequently

$$
\sum_i p_if_i+\sum_iq_ig_i\leq\sum_i(p_i-q_i)\phi_i.
$$

Conversely, any $1$-[Lipschitz](../../../../../../lipschitz-continuity.md) vector $\phi$ gives a feasible pair $(\phi,-\phi)$. Adding a constant leaves its objective unchanged, so impose $\phi_1=0$. The resulting feasible set is compact, and its maximum is $W_\varepsilon$.

For a maximizing vector, the [McShane extension theorem](../../../../../../mcshane-extension-theorem.md) has the following explicit proof in this situation. Define

$$
\phi(x)=\min_i\{\phi_i+d(x,x_i)\}.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) proves that this extension is $1$-[Lipschitz](../../../../../../lipschitz-continuity.md), and the discrete [Lipschitz condition](../../../../../../lipschitz-continuity.md) makes $\phi(x_i)=\phi_i$. Thus $(\phi,-\phi)$ is a continuous feasible pair. Because $|\phi(x)-\phi(r(x))|\leq\varepsilon$,

$$
m_d\geq\int\phi\,dP-\int\phi\,dQ\geq W_\varepsilon-2\varepsilon
\geq W-4\varepsilon.
$$

Letting $\varepsilon\downarrow0$, together with part i, proves **$m_d(P,Q)=W(P,Q)$**. The infimum defining $W$ is also attained: the set of [couplings](../../../../../../coupling.md) is a closed subset of the compact space of [probability measures](../../../../../../probability-measure.md) on $X\times X$, and integrating the continuous cost is continuous for the [weak-star topology](../../../../../../weak-star-topology.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
