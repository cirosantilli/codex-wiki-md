<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Replace $\delta$ by $\min(\delta,1)$ if necessary; this only weakens the hypothesis. We prove the result for finite [graphs](../../../../../graph-split.md) using a random proper partial [graph coloring](../../../../../graph-coloring.md), then a deterministic completion. All constants below may depend on this fixed positive $\delta$.

First record the [extension of a partial colouring by neighbour-colour savings](../../../../../extension-of-a-partial-colouring-by-neighbour-colour-savings.md). If a partial colouring uses colours from a palette of size $K$, let $R_v$ be the number of coloured neighbours of $v$, $D_v$ their number of distinct colours, and $S_v=R_v-D_v$ the [neighbour-colour saving](../../../../../neighbour-colour-saving.md). There are $K-D_v$ available colours and $d(v)-R_v$ uncoloured neighbours. Thus

$$
K-d(v)+S_v\ge1
$$

at every [vertex](../../../../../vertex-graph-theory.md) suffices for greedy completion: each subsequently coloured neighbour removes at most one available colour while reducing the uncoloured-neighbour count by one.

Call $v$ high-degree if $d(v)\ge(1-\delta/8)\Delta$. Its [graph neighbourhood](../../../../../graph-neighbourhood.md) has at least

$$
\binom{d(v)}2-(1-\delta)\binom\Delta2\ge\frac\delta4\Delta^2
$$

nonadjacent pairs for all sufficiently large $\Delta$. Assign independently to every [vertex](../../../../../vertex-graph-theory.md) one of $C=\lceil\Delta/2\rceil$ tentative colours. Erase the colour of every [vertex](../../../../../vertex-graph-theory.md) having a neighbour with the same tentative colour. The remaining colouring is proper; erasure is based on the original assignments and is not an iterative cascade.

For each $v$, define $A_v$ as the number of tentative colours assigned to at least one nonadjacent pair in its [graph neighbourhood](../../../../../graph-neighbourhood.md). Let $B_v$ count those same colours for which at least one neighbour of $v$ loses its colour. Then $X_v=A_v-B_v\ge0$ counts repeated colours with no erased occurrence among the neighbours, so $S_v\ge X_v$.

For a particular nonadjacent pair $u,w\in\Gamma(v)$, consider the event that both receive one colour and no [vertex](../../../../../vertex-graph-theory.md) of $(\Gamma(v)\cup\Gamma(u)\cup\Gamma(w))\setminus\{u,w\}$ receives that colour. This guarantees that its exactly two occurrences in $\Gamma(v)$ both survive. Its [probability](../../../../../probability.md) is at least

$$
\frac1C(1-1/C)^{3\Delta}\ge\frac{e^{-12}}\Delta.
$$

Here $C\ge\Delta/2$, $C\le\Delta$, and $\log(1-1/C)\ge-2/C$ for $C\ge2$. Different pairs cannot be counted by the same colour in this event, since each event specifies exactly two occurrences in the [graph neighbourhood](../../../../../graph-neighbourhood.md). Therefore

$$
\mathbb EX_v\ge\beta\Delta,\qquad \beta=\frac{\delta e^{-12}}4,
$$

for every high-degree [vertex](../../../../../vertex-graph-theory.md). This is the expected [colour savings from sparse neighbourhoods](../../../../../colour-savings-from-sparse-neighbourhoods.md).

We need simultaneous concentration, not just a positive expectation. A single tentative-colour change can affect $A_v$ or $B_v$ only in the old and new colour categories, so each function changes by at most two. A witness for $A_v\ge s$ fixes two [vertices](../../../../../vertex-graph-theory.md) for each of $s$ colours. A witness for $B_v\ge s$ fixes such a nonadjacent pair and an erased neighbour together with a same-coloured adjacent [vertex](../../../../../vertex-graph-theory.md), at most four [vertices](../../../../../vertex-graph-theory.md) per colour. Thus both are [certifiable functions](../../../../../certifiable-function.md) with [Lipschitz constant](../../../../../lipschitz-constant.md) $2$ and certificate parameter at most $4$. Both are bounded by $C\le\Delta$.

To see exactly what concentration follows, let an integer-valued $Z$ change by at most $L$ per coordinate and have certificates of size at most $rb$. For an input with $Z\ge b$, fix such a certificate $J$. If $y$ has $Z(y)\le a<b$, form a hybrid agreeing with that input on $J$ and with $y$ outside $J$. The hybrid has value at least $b$, so at least $(b-a)/L$ certificate positions differ from $y$. Equal weights on $J$ show that its [Talagrand convex distance](../../../../../talagrand-convex-distance.md) from $\{Z\le a\}$ is at least $(b-a)/(L\sqrt{rb})$. [Talagrand's convex distance inequality](../../../../../talagrand-s-convex-distance-inequality.md) therefore gives the [two-threshold concentration for certifiable functions](../../../../../two-threshold-concentration-for-certifiable-functions.md),

$$
\Pr(Z\le a)\Pr(Z\ge b)\le\exp\left[-\frac{(b-a)^2}{4L^2rb}\right].
$$

At an integer [median](../../../../../median.md) $m$, each median-side [probability](../../../../../probability.md) is at least $1/2$. Taking thresholds $m-t,m$ or $m,m+t$ and using $0\le Z\le\Delta$ gives

$$
\Pr(|Z-m|\ge t)\le4e^{-t^2/(64\Delta)}
$$

for $L=2,r=4$. Summing these tails gives $|\mathbb EZ-m|=O(\sqrt\Delta)$. For sufficiently large $\Delta$, depending on $\beta$, it follows that

$$
\Pr\bigl(|Z-\mathbb EZ|\ge\beta\Delta/4\bigr)
\le4e^{-\beta^2\Delta/4096}.
$$

Apply this to $A_v$ and $B_v$. Except with [probability](../../../../../probability.md) at most $8e^{-\beta^2\Delta/4096}$, $X_v\ge\mathbb EX_v-\beta\Delta/2\ge\beta\Delta/2$.

A bad event at $v$ depends only on tentative colours at distance at most two. It is independent of the entire collection of bad events at distance greater than four. Its [dependency graph of events](../../../../../dependency-graph-of-events.md) consequently has [maximum degree](../../../../../maximum-degree.md) at most $2\Delta^4$ for large $\Delta$. The [Lovász local lemma](../../../../../lovasz-local-lemma.md) now makes all high-degree [vertices](../../../../../vertex-graph-theory.md) good simultaneously: exponential decay beats this polynomial dependency bound.

The needed local-lemma step can be checked directly. If every bad-event [probability](../../../../../probability.md) is at most $x(1-x)^D$, induction on conditioning sets gives $\Pr(E\mid\text{avoiding specified other events})\le x$: split those events into non-neighbours of $E$, independent of it, and at most $D$ neighbours, whose avoidance [probability](../../../../../probability.md) is at least $(1-x)^D$ by the induction. Multiplying the resulting conditional avoidance [probabilities](../../../../../probability.md) makes total avoidance positive. Taking $x=1/(D+1)$ works whenever $ep(D+1)\le1$, since $(1-1/(D+1))^D\ge e^{-1}$. Our bound satisfies this criterion once $\Delta\ge\Delta_0(\delta)$.

Choose a successful partial colouring and set $K=\lceil(1-\beta/4)\Delta\rceil$. This contains the original palette. High-degree [vertices](../../../../../vertex-graph-theory.md) satisfy

$$
K-d(v)+S_v\ge\beta\Delta/4\ge1.
$$

Low-degree [vertices](../../../../../vertex-graph-theory.md) have $K-d(v)\ge(\delta/8-\beta/4)\Delta\ge1$ after increasing $\Delta_0$ if necessary. Greedy completion therefore gives $\chi(H)\le K$. Finally, for $\Delta\ge8/\beta$,

$$
\boxed{\chi(H)\le(1-\gamma)\Delta,\qquad
\gamma=\frac\beta8=\frac{\delta e^{-12}}{32}>0.}
$$

The constants are deliberately conservative; existence of a fixed positive improvement is the point. The same proof uses an external [maximum degree](../../../../../maximum-degree.md) bound, so if infinite locally finite [graphs](../../../../../graph-split.md) are allowed, every finite [subgraph](../../../../../subgraph.md) has this uniform colouring bound and compactness extends the colouring to the whole [graph](../../../../../graph-split.md).

For the stronger triangle-free result, the appropriate brief route is [semi-random palette refinement for triangle-free colouring](../../../../../semi-random-palette-refinement-for-triangle-free-colouring.md). Start with $K=C_0\Delta/\log\Delta$ colours and repeatedly make small tentative random assignments, retain conflict-free choices, and update the uncoloured [vertices](../../../../../vertex-graph-theory.md)' available lists. Triangle-freeness makes each [graph neighbourhood](../../../../../graph-neighbourhood.md) independent. Track list size and average residual neighbour congestion per colour, prune unusually congested colours, and use [concentration inequalities](../../../../../concentration-inequality.md) and the [Lovász local lemma](../../../../../lovasz-local-lemma.md) to preserve these invariants through the rounds. The ratio of residual congestion to list size decreases until a final completion using the [Lovász local lemma](../../../../../lovasz-local-lemma.md) or [greedy coloring](../../../../../greedy-coloring.md) succeeds. Average control and pruning are important: four-cycles are allowed, so assuming tight uniform concentration for every individual colour load would be unjustified. With a sufficiently large absolute $C_0$, this programme gives **$\chi(H)=O(\Delta/\log\Delta)$**. The one-round fixed-fraction saving proved above alone does not establish that logarithmic improvement.

To show the order is best possible, let $d\to\infty$ through integers and sample $G(n,d/n)$ with $n=d^7$. A [Chernoff bound](../../../../../chernoff-bound.md) and [union bound](../../../../../boole-s-inequality.md) give [maximum degree](../../../../../maximum-degree.md) at most $2d$ with [probability](../../../../../probability.md) tending to one. The expected triangle count is at most $d^3/6=o(n)$, so fewer than $n/2$ [vertices](../../../../../vertex-graph-theory.md) need be deleted to remove all triangles with high [probability](../../../../../probability.md). For $s=\lceil4n\log d/d\rceil$, the expected number of independent $s$-sets is at most

$$
\left(\frac{en}{s}\right)^s\exp\left[-\frac{d}{n}\binom s2\right]\longrightarrow0:
$$

its logarithm is at most $s[\log(ed/(4\log d))-2\log d+o(1)]$, which tends to minus infinity. The altered [triangle-free graph](../../../../../triangle-free-graph.md) thus has at least $n/2$ [vertices](../../../../../vertex-graph-theory.md) and [independence number](../../../../../independence-number.md) below $s$, giving $\chi\ge(c+o(1))d/\log d$ for an absolute positive $c$. Append a disjoint [star graph](../../../../../star-graph-theory.md) whose centre has [vertex degree](../../../../../degree-graph-theory.md) $2d$ if needed to make its [maximum degree](../../../../../maximum-degree.md) exactly $\Delta=2d$. This proves the [triangle-free chromatic lower bound at bounded maximum degree](../../../../../triangle-free-chromatic-lower-bound-at-bounded-maximum-degree.md), **$\chi=\Omega(\Delta/\log\Delta)$**, so the preceding order cannot be improved in general.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
