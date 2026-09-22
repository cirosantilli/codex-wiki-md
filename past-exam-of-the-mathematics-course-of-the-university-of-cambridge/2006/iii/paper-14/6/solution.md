<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

We prove both inequalities, including the [BK inequality](../../../../../van-den-berg-kesten-inequality.md), for the inhomogeneous [product measure](../../../../../product-measure.md) in the question. Identify a configuration with its set of coordinates equal to one. An up-set is then an [increasing event](../../../../../increasing-event.md). For an [increasing event](../../../../../increasing-event.md) $A$, a set $S$ of open coordinates is a witness if the configuration with precisely $S$ open belongs to $A$: upward closure ensures that those coordinates alone force $A$, whatever the remaining coordinates do. The event $A\square B$ means that there are disjoint open witnesses $S,T$ for $A,B$ respectively.

First prove the [Harris' inequality](../../../../../harris-inequality.md) by induction on the number of coordinates. For the last coordinate, of parameter $p$, write $A_0\subseteq A_1$ and $B_0\subseteq B_1$ for the two sections in the remaining coordinates, and put $a_i=\mathbb P(A_i)$, $b_i=\mathbb P(B_i)$. Induction applied to each section gives

$$
\mathbb P(A\cap B)\geq(1-p)a_0b_0+p a_1b_1.
$$

Subtract the product of the marginal [probabilities](../../../../../probability.md) from the right-hand side:

$$
(1-p)a_0b_0+p a_1b_1-\bigl((1-p)a_0+p a_1\bigr)\bigl((1-p)b_0+p b_1\bigr)
=p(1-p)(a_1-a_0)(b_1-b_0)\geq0.
$$

The base case of zero coordinates is immediate. Thus

$$
\boxed{\mathbb P(A\cap B)\geq\mathbb P(A)\mathbb P(B).}
$$

For disjoint occurrence, first assume every coordinate parameter is at most $1/2$, and again use induction. Put $c_{ij}=\mathbb P(A_i\square B_j)$ on the remaining coordinates. The zero-section of $A\square B$ is exactly $A_0\square B_0$. The one-section is exactly

$$
(A_1\square B_0)\cup(A_0\square B_1).
$$

Indeed, the last open coordinate can belong to at most one of two disjoint witnesses. Assigning it to the $A$ witness leaves a witness for $A_1$ and a witness for $B_0$; assigning it to the $B$ witness gives the other event. If neither witness uses it, both descriptions still hold. Conversely, witnesses for either displayed event lift to disjoint witnesses by adding the last coordinate only to the appropriate one.

The intersection of the two displayed events contains $A_0\square B_0$, because the sections are increasing. Therefore

$$
\mathbb P(A\square B)\leq(1-p)c_{00}+p(c_{10}+c_{01}-c_{00})
=(1-2p)c_{00}+p c_{10}+p c_{01}.
$$

The coefficient $1-2p$ is nonnegative. Applying the induction hypothesis to each term gives

$$
\mathbb P(A\square B)\leq(1-2p)a_0b_0+p a_1b_0+p a_0b_1.
$$

The product of the marginal [probabilities](../../../../../probability.md) is exactly this last expression plus

$$
p^2(a_1-a_0)(b_1-b_0)\geq0.
$$

This proves the desired inequality whenever every parameter is at most $1/2$.

To remove that restriction, suppose first $p_i<1$ for every coordinate. Replace coordinate $i$ by the [logical disjunction](../../../../../logical-disjunction.md) of $m_i$ [independent](../../../../../independent-random-variables.md) [Bernoulli](../../../../../bernoulli-distribution.md) bits, each with parameter

$$
q_i=1-(1-p_i)^{1/m_i}.
$$

Choose $m_i$ large enough that $q_i\leq1/2$. Different blocks are [independent](../../../../../independent-random-variables.md), and their OR values have exactly the original distribution. Let $\widetilde A,\widetilde B$ be the inverse images of $A,B$ under this block-OR map; they are [increasing events](../../../../../increasing-event.md). If the OR configuration has disjoint witnesses $S,T$, choose one open bit from each block indexed by $S$ or $T$. The bits chosen for $S$ force $\widetilde A$, those for $T$ force $\widetilde B$, and the two bit sets are disjoint. Thus the inverse image of $A\square B$ is contained in $\widetilde A\square\widetilde B$. The small-parameter result proves

$$
\mathbb P(A\square B)
\leq\mathbb P(\widetilde A\square\widetilde B)
\leq\mathbb P(\widetilde A)\mathbb P(\widetilde B)
=\mathbb P(A)\mathbb P(B).
$$

Parameters equal to one follow by a [limit](../../../../../limit-of-a-function.md): [probabilities](../../../../../probability.md) of any fixed event on a finite cube are [polynomials](../../../../../polynomial-split.md) in the coordinate parameters, hence continuous. Zero parameters already cause no difficulty. We have obtained

$$
\boxed{\mathbb P(A\square B)\leq\mathbb P(A)\mathbb P(B).}
$$

For the [graph](../../../../../graph-split.md) application, take coordinates to be the [edges](../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../complete-graph.md). Let $A$ be the [increasing event](../../../../../increasing-event.md) that $x$ is connected by a [graph path](../../../../../path-in-a-graph.md) to $U$, and $B$ the corresponding event for $W$. Their [probabilities](../../../../../probability.md) are $\alpha,\beta$. A simple [graph path](../../../../../path-in-a-graph.md) from $U$ to $W$ through $x$ splits at $x$ into two [graph paths](../../../../../path-in-a-graph.md) with disjoint [edge](../../../../../edge-of-a-graph.md) sets. Those sets witness $A$ and $B$, so this [graph path](../../../../../path-in-a-graph.md) event is contained in $A\square B$. The [BK inequality](../../../../../van-den-berg-kesten-inequality.md) gives

$$
\boxed{\mathbb P(\text{a }U\text{--}W\text{ path through }x)\leq\alpha\beta.}
$$

On the other hand, if both $A$ and $B$ occur, concatenate an $x$-to-$U$ [graph path](../../../../../path-in-a-graph.md) and an $x$-to-$W$ [graph path](../../../../../path-in-a-graph.md) to obtain a walk from $U$ to $W$. Removing loops yields a simple [graph path](../../../../../path-in-a-graph.md), although it need not pass through $x$. Thus $A\cap B$ is contained in the unrestricted connection event, and the [Harris' inequality](../../../../../harris-inequality.md) gives

$$
\boxed{\mathbb P(\text{a }U\text{--}W\text{ path})\geq\mathbb P(A\cap B)\geq\alpha\beta.}
$$

The distinction between a simple [graph path](../../../../../path-in-a-graph.md) through $x$ and an unrestricted connection is essential: a walk may revisit an [edge](../../../../../edge-of-a-graph.md), so a through-$x$ walk would not in general provide disjoint witnesses.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
