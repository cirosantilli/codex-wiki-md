<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The assertion with the same $\varepsilon$ in the degree interval and the final colour bound is **false as printed**. Fix $r=2$, $\varepsilon=1/10$, let $G=K_{22m+1}$, and take $D=20m$. Every degree is $22m=(1+\varepsilon)D$, while every pair [hypergraph codegree](../../../../../hypergraph-codegree.md) is one. For any proposed $\delta>0$, choose $m$ large enough that $1\leq\delta D$. Nevertheless a [matching in a graph](../../../../../matching-graph-theory.md) contains at most $11m$ edges, whereas there are $(22m+1)11m$ edges in total. Thus every [edge coloring](../../../../../edge-coloring.md) requires at least $22m+1$ colours, exceeding $(1+\varepsilon)D=22m$. The obstruction persists with arbitrarily small relative [hypergraph codegree](../../../../../hypergraph-codegree.md).

The meaningful asymptotic target separates the output tolerance from the input regularity error. For fixed rank $r$ and target $\eta>0$, choose a sufficiently small $\delta=\delta(r,\eta)$ and require degrees in $[(1-\delta)D,(1+\delta)D]$ as well as pair [hypergraph codegrees](../../../../../hypergraph-codegree.md) at most $\delta D$. The [semi-random method](../../../../../semi-random-method.md) then gives $\chi'(G)\leq(1+\eta)D$. Here is the requested proof essay for that corrected conclusion, including its random rounds, tracking requirements and completion step.

A useful way to run all colour classes together is the [auxiliary matching construction for hypergraph edge colouring](../../../../../auxiliary-matching-construction-for-hypergraph-edge-colouring.md). Use $K=\lceil D\rceil$ initial colours. Create a task vertex for each original edge $e$, and a resource vertex $(v,c)$ for each original vertex and colour. An assignment $(e,c)$ is an $(r+1)$-edge consisting of its task and the resources $(v,c)$ for all $v\in e$. A [matching in a hypergraph](../../../../../matching-in-a-hypergraph.md) in this auxiliary system is a proper partial colouring: a task cannot get two colours, and two edges sharing $v$ cannot use the same resource $(v,c)$.

The auxiliary task degrees are $K$, resource degrees are $d_G(v)$, and its pair [hypergraph codegrees](../../../../../hypergraph-codegree.md) are at most $\max(1,\delta D)$. It is therefore nearly regular with small [hypergraph codegrees](../../../../../hypergraph-codegree.md). For $r\geq2$ and a nonempty original [hypergraph](../../../../../hypergraph-split.md), the [hypergraph codegree](../../../../../hypergraph-codegree.md) condition also forces $D\geq1/\delta$; taking $\delta$ small absorbs rounding and ensures a large working degree. Rank one is immediate by assigning distinct colours to edges at each vertex.

The extra balance condition is important. Let $S_v$ be the [set](../../../../../set-split.md) of tasks corresponding to edges through original vertex $v$. A [matching in a hypergraph](../../../../../matching-in-a-hypergraph.md) missing a small fraction of all tasks need not leave few tasks in each $S_v$. The [Rödl nibble](../../../../../rodl-nibble.md) must leave at most $\beta D$ unmatched tasks in **every** such star, where one may choose $\beta=\eta/(4r)$. This local requirement, rather than just a global almost-perfect [matching in a hypergraph](../../../../../matching-in-a-hypergraph.md), is what permits a cheap final edge colouring.

Run a [Rödl nibble](../../../../../rodl-nibble.md) on the auxiliary system, whose rank is $s=r+1$. In a round of working degree $D_j$, sample each surviving assignment independently with [probability](../../../../../probability.md) $\alpha/D_j$, for a small fixed $\alpha$. Accept the sampled assignments that meet no other sampled assignment. Delete every auxiliary vertex touched by any sampled assignment, including conflicted ones, before proceeding. The accepted assignments are a [matching in a hypergraph](../../../../../matching-in-a-hypergraph.md), and later assignments cannot reuse a consumed task or resource. Record each discarded but uncoloured task as waste; it must be counted in the final residual [graph](../../../../../graph-split.md).

For an auxiliary vertex of degree $(1\pm\xi)D_j$, the [probability](../../../../../probability.md) of remaining untouched is

$$
(1-\alpha/D_j)^{d_j(v)}
=e^{-\alpha}(1+O(\xi\alpha+1/D_j)).
$$

For an auxiliary edge through a surviving vertex, the other $s-1$ vertices survive with [probability](../../../../../probability.md) approximately $e^{-(s-1)\alpha}$. Their incident trial families overlap in at most $O_s(\delta D)$ trials by the [hypergraph codegree](../../../../../hypergraph-codegree.md) bound, so the overlap error in this product calculation is small. This leads to the degree trajectory

$$
D_{j+1}\approx D_j e^{-(s-1)\alpha},
$$

while the surviving fraction of task vertices is approximately $e^{-\alpha}$ per round. For a sampled assignment, a union bound over at most $s(1+O(\xi))D_j$ conflicting assignments gives collision [probability](../../../../../probability.md) at most $s\alpha(1+O(\xi))$. More explicitly, for a fixed task the expected number of ordered sampled conflict pairs having the first assignment through that task is at most

$$
(1+O(\xi))D_j\cdot s(1+O(\xi))D_j
\left(\frac\alpha{D_j}\right)^2=O_s(\alpha^2).
$$

This bounds its waste [probability](../../../../../probability.md). Thus productive deletion is first order in $\alpha$, and collision loss is second order.

The technical tracking step makes these [expected value](../../../../../expected-value.md) calculations locally simultaneous and keeps their errors from accumulating. Its requirements are: residual auxiliary degrees stay near their trajectory after controlled pruning; each original star has the predicted number of surviving tasks; and every star's total collision and pruning waste is small. The standard probabilistic tools enter at distinct points.

Within a fixed round, task-survival indicators are independent: trial families for different tasks are disjoint, even when their assignments share resources. Conditional [Chernoff bounds](../../../../../chernoff-bound.md) therefore control the number of surviving tasks in each star. Collision loss has short certificates consisting of pairs of selected intersecting assignments. The number selected through one resource has a binomial distribution of bounded mean. [Chernoff bounds](../../../../../chernoff-bound.md) truncate these numbers at a suitable logarithmic cutoff; after truncation one trial has only a logarithmically bounded effect on the certified collision count. A [certifiable function](../../../../../certifiable-function.md) concentration bound, or a corresponding exposure argument, then controls loss in each star. These rare local overload [events](../../../../../event.md) have polynomially bounded local dependency neighborhoods in the working degree, so the [Lovász local lemma](../../../../../lovasz-local-lemma.md) can select a simultaneous outcome independent of the total number of vertices.

Residual-degree counts require additional care because they are not sums of independent indicators. Two survival tests share at most a [hypergraph codegree](../../../../../hypergraph-codegree.md)'s worth of trials; expanding their joint [probabilities](../../../../../probability.md) bounds their covariance by the corresponding relative overlap. For a residual-degree count $Z$ with $D_j$ summands, overlapping summands and shared survival trials give a [variance](../../../../../variance-split.md) bound of the form

$$
\operatorname{Var}Z\leq C_s(D_j+\zeta D_j^2),\qquad
\zeta=\frac{\text{maximum current pair codegree}}{D_j}.
$$

[Chebyshev's inequality](../../../../../chebyshev-inequality.md) then bounds $\Pr(|Z-\mathbb EZ|>\xi D_j)$ by $C_s(D_j^{-1}+\zeta)/\xi^2$. This gives a small exceptional fraction when the relative [hypergraph codegree](../../../../../hypergraph-codegree.md) is sufficiently small; it does not by itself make every degree good. The tracking argument records and prunes these exceptional configurations, bounding their contribution to each star by codegree-weighted exposure and the same local-loss bookkeeping. [Markov's inequality](../../../../../markov-inequality.md) controls exceptional mass, and repeated conditional concentration controls the retained counts. One must not apply an independent [Chernoff bound](../../../../../chernoff-bound.md) directly to a residual degree or infer a uniform star bound just from a global expected loss. Keeping the pruning loss explicitly is the key distinction between a valid [Rödl nibble](../../../../../rodl-nibble.md) argument and those shortcuts.

Choose the parameters in this order: first $r,\eta$ and $\beta$; next $\alpha$ so small that $s\alpha\log(4/\beta)\ll\beta$; next

$$
T\approx\alpha^{-1}\log(4/\beta);
$$

and finally the initial regularity/[hypergraph codegree](../../../../../hypergraph-codegree.md) tolerance $\delta$ small enough for all $T$ tracking and pruning errors. This is a bounded number of rounds depending on the tolerances, not on the [graph](../../../../../graph-split.md) order. After $T$ rounds, the surviving task fraction is at most approximately $\beta/4$, while accumulated collision loss is $O_s(T\alpha^2)=O_s(\alpha\log(4/\beta))$. Reserving the remaining margin for tracking and pruning leaves at most $\beta D$ uncoloured edges at every original vertex. The working degree is still a fixed positive multiple of $D$, namely about $D e^{-r\alpha T}$, so the large-degree estimates remain applicable throughout.

Finally use a fresh palette on the residual original [hypergraph](../../../../../hypergraph-split.md). Its maximum degree is at most $\beta D$; an edge meets at most $r(\beta D-1)$ others. Greedy colouring therefore needs at most $r\beta D+1$ fresh colours. The total is at most

$$
K+r\beta D+1\leq D+2+\eta D/4\leq(1+\eta)D
$$

for sufficiently large $D$, already ensured by choosing $\delta$ small. This completes the passage from the locally balanced [Rödl nibble](../../../../../rodl-nibble.md) to the [hypergraph chromatic index](../../../../../hypergraph-chromatic-index.md) bound. The degree tolerance must be the small input parameter $\delta$; replacing it by the entire output allowance $\eta$ removes the slack and leads precisely to the complete-graph counterexample above.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
