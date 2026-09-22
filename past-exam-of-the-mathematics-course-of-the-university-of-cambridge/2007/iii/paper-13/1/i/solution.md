<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $p_i=\mathbb P(A_i)$. A [strong independence graph](../../../../../../dependency-graph-of-events.md) of maximum degree one consists of isolated vertices and disjoint pairs. For a component $C$, let $B$ be the event that all events outside $C$ are avoided. Each $A_i$, $i\in C$, is independent of $B$, since the outside vertices are all nonneighbors. The [union bound](../../../../../../boole-s-inequality.md) therefore gives

$$
\mathbb P\Bigl(B\cap\bigcap_{i\in C}A_i^c\Bigr)\geq\Bigl(1-\sum_{i\in C}p_i\Bigr)\mathbb P(B).
$$

Remove the components successively. If every $p_i<1/2$, all these factors are positive, including singleton components, so simultaneous avoidance has positive [probability](../../../../../../probability.md). Conversely, two complementary events of [probability](../../../../../../probability.md) $1/2$, joined by one edge, cover the sample space. Consequently **$\gamma(1)=1/2$**. The argument does not assume joint independence between entire two-event components.

For higher degrees use a [dependency-degree obstruction on a rooted tree](../../../../../../dependency-degree-obstruction-on-a-rooted-tree.md). Put $d=\Delta-1$ and choose

$$
p>p_*:=\frac{d^d}{(d+1)^{d+1}},\qquad p<1.
$$

On a finite rooted $d$-ary [tree](../../../../../../tree-graph-theory.md) take independent bits $B_v$ and define $A_v$ to mean that $B_v=1$ and every child bit is zero. The underlying [tree](../../../../../../tree-graph-theory.md) is a [strong independence graph](../../../../../../dependency-graph-of-events.md): the variables used by $A_v$ are disjoint from all variables used by its nonneighbors. Its maximum degree is at most $d+1$.

Give the leaves success probability $r_0=p$, and, working upwards, use

$$
r_{j+1}=\frac{p}{(1-r_j)^d}
$$

as long as this is less than one. This recursion must reach or exceed one after finitely many steps. Indeed,

$$
\max_{0\leq r\leq1}r(1-r)^d=\frac{d^d}{(d+1)^{d+1}}<p,
$$

so the iterates strictly increase. An infinite sequence staying below one would either converge to a fixed point, contradicting the displayed maximum, or tend to one, in which case its next iterate would exceed one. At the first offending step set the root success probability to one instead of the proposed value. Every nonroot event then has [probability](../../../../../../probability.md) exactly $p$; the root event has [probability](../../../../../../probability.md) $(1-r_j)^d\leq p$.

Every configuration contains an occurring event: start at the root, whose bit is one; if its event fails, descend to a child whose bit is one, and repeat. A finite [tree](../../../../../../tree-graph-theory.md) forces this descent to end at an occurring event. Thus avoidance is impossible. Given any $c>p_*$, choose $p\in(p_*,\min(c,1))$; all event [probabilities](../../../../../../probability.md) are strictly below $c$. This proves

$$
\boxed{\gamma(\Delta)\leq\frac{(\Delta-1)^{\Delta-1}}{\Delta^\Delta}\quad(\Delta\geq2).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
